# ml_projects
This repository showcases all my personal machine/deep learing projects and their source code

# mRNA Degradation

<p align="center">
<img src="https://www.promegaconnections.com/wp-content/uploads/2021/05/MayBlog-RNA-TW.jpg" width="800">
</p>

## Overview
This project was based on the Kaggle competition [OpenVaccine: COVID-19 mRNA Vaccine Degradation Prediction](https://www.kaggle.com/competitions/stanford-covid-vaccine) that happened in 2020. The mRNA vaccines were the fastest vaccine candidates for COVID-19, but problems were arised when researchs noticed that the RNA molecules seem to degrade almost spotaneously. These vaccines needed super stable messenger RNA molecule to be designed. That's where this project comes into play. The goal of this project is to design and implement a deep learning model that can that can predict whether an RNA molecule will degrade or not.

## Key challenges
- Predicting a continous output with a sequence input
- The training sequence/predictions lengths differ from the test sequence lengths
- Data is stored in a JSON file where the each of the 5 prediction parameters was a list of numbers


# Paddy Leaf Classification

<p align="center">
<img src="http://prod-upp-image-read.ft.com/c588b2a0-fbbe-11e8-b03f-bc62050f3c4e" width="800">
</p>

## Overview
This project was based on the Kaggle Competition [Paddy Doctor: Paddy Disease Classification](https://www.kaggle.com/competitions/paddy-disease-classification). Paddy is the raw grain of rice before the removal of husk. It is farmed in tropical climates, but mainly in Asian countries. If paddy cultivation is left unsupervised, diseases and pests can cause yield loss of 70%. The aim of this project is design a deep learning classification model to classify whether a paddy leaf has  disease and if it does which disease.

## Key challenges
- Images from the dataset were not the same size
- Experimenting to find best data augmentations for each model
- Selecting suitable architectures for model
- Ensembling the strongest models to achieve highest score

# Retinal Optical Coherence Tomography

<p align="center">
<img src="https://i.imgur.com/fSTeZMd.png" width="800">
</p>

## Overview
This project was based on Retinal OCT (Optical Coherent Tomography). This is an imaging technique used to capture high-resolution cross sections of the retinas of living patients. Approximately 30 million OCT scans are performed each yearm and the analysis and interpertation of these images takes up a significant amount of time. By building a deep learning model to classify between different:

- Choroidal neovascularization (CNV) with neovascular membrane (white arrowheads) and associated subretinal fluid (arrows)
- Diabetic macular edema (DME) with retinal-thickening-associated intraretinal fluid (arrows)
- Multiple drusen present in early AMD
- Normal retina

I managed to get an accuracy of 99.9% on the test dataset!

## Key challenges
- Building the model with PyTorch and creating a training function to process both validation and training steps
- Transfer learning using ResNet18
