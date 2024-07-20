# Student Grades Prediction

This repository contains the code and analysis for predicting student final grades using various factors. The project involves data loading, preprocessing, exploratory data analysis (EDA), model training, and model evaluation.

## Table of Contents
- [Introduction](#introduction)
- [Data Loading and Preprocessing](#data-loading-and-preprocessing)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Model Training](#model-training)
- [Model Evaluation](#model-evaluation)
- [Conclusion](#conclusion)

## Introduction
The goal of this project is to predict student final grades using a linear regression model. The dataset contains various demographic and behavioral features that could influence academic performance.

## Data Loading and Preprocessing
Start by loading the data and merging two datasets (math and Portuguese classes) to form a combined dataset. The data is then cleaned by removing unnecessary columns and handling missing values.

## Exploratory Data Analysis (EDA)
During the EDA phase, analyze the data to understand relationships between different variables and the final grades. Some key analyses include:
1. **Gender Comparison**: Comparing final grades between male and female students.
2. **Study Time vs Final Grades**: Analyzing the impact of study time on final grades.
3. **Failures vs Final Grades**: Exploring how the number of failures impacts students' final grades.
4. **Alcohol Consumption vs Final Grades**: Analyzing the effect of alcohol consumption on academic performance.
5. **Absences vs Final Grades**: Observing the impact of student absences on their final grades.

## Model Training
A linear regression model is trained using the preprocessed data. The dataset is split into training and testing sets, and the model is trained on the training set.

## Model Evaluation
The model's performance is evaluated using various metrics:
- **Mean Absolute Error (MAE)**: Measures the average magnitude of the errors.
- **Mean Squared Error (MSE)**: Measures the average of the squares of the errors.
- **Root Mean Squared Error (RMSE)**: The square root of the average of squared differences.
- **R² Score**: Represents the proportion of the variance for the dependent variable that's explained by the independent variables.

### Performance Metrics:
- **Mean Absolute Error (MAE)**: 4.353454844747764e-15
- **Mean Squared Error (MSE)**: 3.487374317853227e-29
- **Root Mean Squared Error (RMSE)**: 5.905368262678732e-15
- **R² Score**: 1.0

### Evaluation and Commentary
The model shows almost perfect performance metrics with an R² score of 1.0 and error metrics (MAE, MSE, RMSE) close to zero. This indicates that the model's predictions almost perfectly match the actual values.

These results can usually occur due to the following reasons:
1. **Model Overfitting**: The model has fit the training data excessively well and is predicting the test data perfectly. In this case, the model may not generalize well to real-world data.
2. **Data Structure Issue**: There might be an extremely obvious relationship between the independent and dependent variables in the dataset, or there might be an error in the data.
3. **Model Accuracy**: The model genuinely performs exceptionally well on the training and test data.

### R² Score and Error Metrics:
- **Mean Absolute Error (MAE)**: Measures the average magnitude of the errors in a set of predictions, without considering their direction. Being close to 0 indicates that the model's predictions are very accurate.
- **Mean Squared Error (MSE)**: Measures the average of the squares of the errors—that is, the average squared difference between the estimated values and what is estimated. Being close to 0 indicates that the model is not making large errors.
- **Root Mean Squared Error (RMSE)**: The square root of the average of squared differences between prediction and actual observation. Being close to 0 indicates that the errors are small and the model performs well.
- **R² Score**: A statistical measure that represents the proportion of the variance for a dependent variable that's explained by an independent variable or variables in a regression model. An R² score of 1.0 indicates that the model explains all the variance and fits perfectly.


