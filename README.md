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
