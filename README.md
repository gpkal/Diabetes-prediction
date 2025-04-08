# Diabetes prediction: a supervised learning approach

A machine learning classification system to predict diabetes risk based on behavioral risk factors.

## Overview

This project implements various supervised learning models to predict diabetes diagnoses based on behavioral and health risk factors. Using the [Knime Analytics Platform](https://www.knime.com/), we developed binary classification models and compared their performance to identify the most reliable solution for supporting medical diagnosis and prevention activities.

## Dataset

The dataset consists of 40,108 observations and 18 features including:
- Demographic data (Age, Sex)
- Health indicators (BMI, Cholesterol levels, Blood pressure)
- Lifestyle factors (Physical activity, Diet, Alcohol consumption)
- Medical history (Heart disease, Stroke)
- General health assessments

## Methodology

**Data Preprocessing**
- Correlation analysis using Spearman coefficient
- Class balance verification (51% diabetes, 49% non-diabetes)
- Feature transformation including BMI discretization according to WHO standards
- Discretization of mental and physical health variables

**Model Development**
Various classification methods were implemented and compared:
- Heuristic models: Random Forest, Gradient Boosted Trees, XGBoost
- Regression models: Logistic Regression
- Separation models: Multi-Layer Perceptron (MLP)
- Probabilistic models: Bayesian Network

**Evaluation Approach**
- 80%-20% training/test set split with stratified sampling
- 10-fold cross-validation
- Feature selection using wrapper methods
- Parameter optimization for selected models

## Implementation

The project was developed using Knime Analytics Platform with the following workflow:
1. Training.knwf - Preprocessing, model training and comparison
2. Deployment.knwf - Model deployment and optimization
3. Data App.knwf - Interactive visualization and prediction interface

---
Project by Giorgia Prina, Simone Massardi and Enrico Mannarino
*Machine Learning course project, 2022-2023*  
*Master Degree in Data Science - University of Milano-Bicocca*
