# Global-Air-Pollution-AQI-Classification
Machine learning project for classifying global air quality categories using pollutant-specific AQI indicators with Decision Tree, SVM, and XGBoost.

# Global Air Pollution - AQI Category Classification

## 📌 Project Overview

This project develops a machine learning classification system for predicting Air Quality Index (AQI) categories using pollutant-specific air-quality indicators.

The project uses Python and compares multiple supervised machine learning algorithms to determine which model provides the most effective classification performance.

The main algorithms evaluated are:

- Decision Tree
- Support Vector Machine (SVM)
- XGBoost

The project follows an end-to-end machine learning pipeline including data preprocessing, exploratory data analysis, feature selection, model training, evaluation, cross-validation, and model comparison.

---

## 🎯 Problem Statement

Air pollution is a major environmental concern, and raw air-quality measurements can be difficult for users to interpret.

The objective of this project is to develop a machine learning model that can classify overall air quality into predefined AQI categories based on pollutant-specific air-quality indicators.

---

## 🎯 Objectives

- Analyze a global air pollution dataset.
- Clean and preprocess the dataset.
- Perform exploratory data analysis.
- Identify relevant pollutant-related features.
- Train multiple machine learning classification models.
- Compare model performance using standard evaluation metrics.
- Analyze classification errors using confusion matrices.
- Identify important features affecting predictions.
- Validate model performance using 5-fold cross-validation.
- Select the best-performing model.

---

## 📊 Dataset

The dataset contains global air-quality observations with information related to:

- Country
- City
- AQI value
- AQI category
- CO AQI
- Ozone AQI
- NO2 AQI
- PM2.5 AQI

### Target Variable

`aqi_category`

### Selected Features

The following pollutant-specific AQI values are used as input features:

- `co_aqi_value`
- `ozone_aqi_value`
- `no2_aqi_value`
- `pm2.5_aqi_value`

The overall `aqi_value` is intentionally excluded from the model inputs because the target AQI category is directly derived from overall AQI. Excluding it helps reduce target leakage and makes the classification problem more meaningful.

---

## 🔄 Machine Learning Pipeline

```text
Data Collection
       ↓
Data Understanding
       ↓
Data Cleaning
       ↓
Missing Value Handling
       ↓
Exploratory Data Analysis
       ↓
Feature Selection
       ↓
Target Encoding
       ↓
Train/Test Split
       ↓
Model Training
       ↓
Model Evaluation
       ↓
Cross-Validation
       ↓
Model Comparison
       ↓
Best Model Selection
