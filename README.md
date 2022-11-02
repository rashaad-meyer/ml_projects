# ml_projects
This repository showcases all my personal machine/deep learing projects and their source code

# mRNA Degradation

## Overview
This project was based on the Kaggle competition [OpenVaccine: COVID-19 mRNA Vaccine Degradation Prediction](https://www.kaggle.com/competitions/stanford-covid-vaccine) that happened in 2020. The mRNA vaccines were the fastest vaccine candidates for COVID-19, but problems were arised when researchs noticed that the RNA molecules seem to degrade almost spotaneously. These vaccines needed super stable messenger RNA molecule to be designed. That's where this project comes into play. The goal of this project is to design and implement a deep learning model that can that can predict whether an RNA molecule will degrade or not.

## Key challenges
- Predicting a continous output with a sequence input
- The training sequence/predictions lengths differ from the test sequence lengths
- Data is stored in a JSON file where the each of the 5 prediction parameters was a list of numbers
