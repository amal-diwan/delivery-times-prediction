# Predicting Food Delivery Time using Machine Learning

## Overview

This project focuses on predicting **food delivery time (in minutes)** using machine learning models. It simulates a real-world problem faced by food delivery platforms where inaccurate time estimates can negatively impact user experience.

This notebook demonstrates a **complete end-to-end ML pipeline**, including:

* Data preprocessing
* Exploratory Data Analysis (EDA)
* Feature engineering
* Model training & comparison
* Feature importance analysis

## Problem Statement

Food delivery apps need to estimate how long an order will take to reach customers. Poor predictions lead to:

* Customer dissatisfaction
* Reduced trust in the platform

**Goal:** Build a machine learning model that predicts delivery time based on order details, distance, traffic, and environmental factors.

## Machine Learning Approach

* **Type:** Supervised Learning
* **Problem:** Regression
* **Target Variable:** `Delivery_Time_min`

### Features Used:

* Distance (`Distance_km`)
* Preparation time
* Courier experience
* Traffic intensity
* Peak hour indicator
* Weather conditions
* Time of day
* Vehicle type
* Engineered feature: Distance × Traffic interaction

## Project Workflow

### 1. Data Preprocessing

* Handled missing values
* Scaled numerical features using `StandardScaler`
* Encoded categorical features using `OneHotEncoder`
* Built preprocessing pipeline using `ColumnTransformer`


### 2. Exploratory Data Analysis (EDA)

* Analyzed distribution of delivery time
* Studied impact of distance and traffic
* Identified key influencing variables

### 3. Feature Engineering

* Created interaction features
* Improved model performance by capturing relationships between variables

### 4. Model Training

Implemented and compared:

* Linear Regression
* Random Forest Regressor
* Gradient Boosting Regressor

Used **Scikit-learn Pipelines** for clean and reproducible workflows.

### 5. Model Evaluation

Evaluated models using:

* MAE (Mean Absolute Error)
* RMSE (Root Mean Squared Error)
* R² Score

Compared results to select the best-performing model.

### 6. Feature Importance

* Extracted feature importance from Random Forest
* Identified key drivers of delivery time

## Tools

* Python
* Pandas & NumPy
* Matplotlib & Seaborn
* Scikit-learn

## Key Insights

* Distance and traffic are the strongest predictors
* Feature engineering improves accuracy
* Ensemble models outperform linear models


## Future Improvements

* Hyperparameter tuning
* Try XGBoost / LightGBM
* Deploy with Streamlit or Flask
* Use real-time traffic & weather data

