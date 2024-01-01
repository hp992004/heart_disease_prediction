# Heart Disease Prediction Model

## Overview

This repository contains a machine learning model for predicting the presence or absence of heart disease based on certain features. The model utilizes logistic regression and is implemented in Python using popular data science libraries.

## Table of Contents

- [Introduction](#introduction)
- [Dataset](#dataset)
- [Data Preprocessing](#data-preprocessing)
- [Model Training](#model-training)
- [Model Evaluation](#model-evaluation)
- [Results](#results)
  - [Feature Importance](#feature-importance)
  - [Insights from Model Coefficients](#insights-from-model-coefficients)
- [Conclusion](#conclusion)

## Introduction

Cardiovascular diseases are a major global health concern, and early detection can significantly improve outcomes. This project aims to develop a predictive model for heart disease using a dataset with various health-related features.

## Dataset

- **Source**: [Heart_Disease_Prediction.csv]
- **Columns**: The dataset includes features such as age, sex, cholesterol levels, etc.

### Data Summary

- **Shape**: The dataset comprises X rows and Y columns.
- **Columns**: A detailed list of columns, including information about the target variable.
- **Missing Data**: No missing values were observed in the dataset.
- **Duplicate Data**: There were no duplicate records in the dataset.

## Data Preprocessing

- **Separating Variables**: The dataset was divided into independent variables (X) and the target variable (y).
- **Train-Test Split**: 80% of the data was used for training, and 20% for testing the model.
- **Feature Scaling**: StandardScaler was applied to standardize the feature values.

## Model Training

- **Model**: Logistic Regression was chosen for its simplicity and interpretability.
- **Training**: The model was trained on the training set using the fit method.

## Model Evaluation

- **Predictions**: The model made predictions on the test set using the predict method.
- **Metrics**:
  - **Accuracy Score**: 0.9074
  - **Precision**: 0.9
  - **Recall**: 0.8571
  - **F1 Score**: 0.878
- **Confusion Matrix**: The confusion matrix revealed [31 true negatives, 2 false positives, 3 false negatives, 18 true positives].

## Results

### Feature Importance

- **Insights from Model Coefficients**:

  Understanding the impact of each feature on the prediction can provide valuable insights into the factors contributing to heart disease.

  - **Age**: The positive coefficient for age suggests that as age increases, the likelihood of heart disease also increases. Age appears to be a significant predictor.

  - **Sex**: The coefficient for sex indicates the influence of gender on heart disease prediction. Further analysis may be needed to understand the specific role of gender in this context.

  - **Cholesterol Levels**: Elevated cholesterol levels contribute positively to the prediction, aligning with existing medical knowledge linking high cholesterol to heart issues.

  - **Resting Blood Pressure**: The coefficient for resting blood pressure indicates its impact on heart disease prediction. Understanding the threshold values is crucial for interpretation.

  - **Max Heart Rate**: A negative coefficient suggests an inverse relationship between maximum heart rate and the likelihood of heart disease. This warrants deeper exploration.

  - **Exercise-Induced Angina**: Presence of exercise-induced angina shows a negative impact, indicating a potential protective effect against heart disease during physical activity.

  - **Chest Pain Type**: Different types of chest pain may have varying impacts on heart disease prediction. The coefficients provide insights into their relative significance.

  These insights can guide healthcare professionals in assessing and interpreting the risk factors for heart disease, contributing to more informed decision-making.

## Conclusion

In conclusion, the model demonstrated promising results with a high accuracy of 90.74%. Further refinement and feature engineering could enhance its predictive capabilities.
