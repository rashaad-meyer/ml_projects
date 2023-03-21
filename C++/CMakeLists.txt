# CMakeList.txt : CMake project for HelloTorch, include source and define
# project specific logic here.
#
cmake_minimum_required(VERSION 3.8)

set(CMAKE_PREFIX_PATH "C:\\dev\\libs\\libtorch-debug\\libtorch")
find_package(Torch REQUIRED)
set(CMAKE_CXX_FLAGS "${CMAKE_CXX_FLAGS} ${TORCH_CXX_FLAGS}")

# Add source to this project's executable.
add_executable (HelloTorch "HelloTorch.cpp" "HelloTorch.h")

target_link_libraries(HelloTorch "${TORCH_LIBRARIES}")
set_property(TARGET HelloTorch PROPERTY CXX_STANDARD 14)

if (CMAKE_VERSION VERSION_GREATER 3.12)
  set_property(TARGET HelloTorch PROPERTY CXX_STANDARD 20)
endif()



if (MSVC)
  file(GLOB TORCH_DLLS "${TORCH_INSTALL_PREFIX}/lib/*.dll")
  add_custom_command(TARGET HelloTorch
                     POST_BUILD
                     COMMAND ${CMAKE_COMMAND} -E copy_if_different
                     ${TORCH_DLLS}
                     $<TARGET_FILE_DIR:HelloTorch>)
endif (MSVC)

# TODO: Add tests and install targets if needed.
