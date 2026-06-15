# Wildfire Intensity Classification using Machine Learning

This project explores a machine learning classification workflow for predicting wildfire fire intensity levels using environmental, weather, satellite-derived, and geographic features.

The project was completed as part of my Computational Machine Learning coursework and has been converted into a portfolio-friendly version. The original processed assessment dataset is not included in this repository due to assessment data-use restrictions.

## Project Overview

The goal was to classify wildfire events into four fire intensity levels:

* Low
* Moderate
* High
* Extreme

This is a supervised multi-class classification problem. The input features include location, detection time, season, region, country, fire type, satellite information, brightness temperature, confidence level, temperature, wind speed, precipitation, and humidity.

## Methods Used

The workflow included:

* dataset inspection
* missing value handling
* exploratory data analysis
* categorical and numerical preprocessing
* train-validation splitting
* model development and comparison
* hyperparameter tuning
* model evaluation using accuracy and macro F1-score
* discussion of limitations and professional responsibilities

Three models were compared:

* Decision Tree
* Support Vector Machine
* Neural Network

## Key Findings

The dataset was imbalanced, with Moderate and High fire events appearing more frequently than Low and Extreme events. Because of this, macro F1-score was important alongside accuracy, as it gives equal importance to each class.

Brightness temperature was an important feature because stronger fires are expected to produce stronger thermal signals. However, no single feature fully separated the four classes, so the models needed to combine multiple environmental, geographic, and satellite-derived variables.

## Model Selection

The Support Vector Machine achieved the highest validation accuracy, but the Neural Network achieved the highest validation macro F1-score. Since the task involved imbalanced classes and minority classes such as Low and Extreme were important, the Neural Network was selected as the final model.

The selected model used:

* one hidden layer with 50 neurons
* learning rate = 0.0005

## Responsible Use

This type of model should be treated as a decision-support tool, not as a replacement for expert wildfire assessment. In real-world use, predictions should be reviewed alongside satellite imagery, weather forecasts, local knowledge, and emergency service judgement.

## Skills Demonstrated

* Python
* pandas
* NumPy
* scikit-learn
* Decision Tree
* Support Vector Machine
* Neural Network
* classification
* preprocessing
* missing value handling
* hyperparameter tuning
* accuracy and macro F1-score evaluation
* responsible AI discussion

## Data Availability

The processed assessment dataset is not included in this repository because it was provided only for coursework use. This repository is intended to document the machine learning workflow and project learning outcomes without redistributing restricted data.
