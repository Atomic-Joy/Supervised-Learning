# 🍷 Wine Quality Ordinal Prediction Project

## Overview

This project demonstrates a complete **Machine Learning pipeline** for **Ordinal / Rating Prediction**, which is a type of supervised learning where the model predicts ordered target values. In this case, the model learns patterns from physicochemical properties of wine to predict wine quality ratings using the Wine Quality dataset.

---

## Objective

To predict wine quality ratings based on chemical properties and develop a machine learning model for accurate ordinal prediction.

---

## Dataset

* **Dataset:** Wine Quality Dataset
* **Files Used:**

  * `winequality-red.csv`
  * `winequality-white.csv`

* **Features:**

  * Fixed acidity
  * Volatile acidity
  * Citric acid
  * Residual sugar
  * Chlorides
  * Free sulfur dioxide
  * Total sulfur dioxide
  * Density
  * pH
  * Sulphates
  * Alcohol
  * Wine type

* **Target Variable:**

  * Quality rating (3–8)

---

## Workflow

### 🔹 Data Loading

* Loaded red and white wine datasets using Pandas
* Combined both datasets into a single DataFrame

### 🔹 Exploratory Data Analysis (EDA)

* Dataset information & statistics
* Wine type distribution
* Wine quality distribution
* Correlation heatmap

### 🔹 Data Preprocessing

* Label encoding for wine type
* Train-test split (80-20)
* Feature scaling using `StandardScaler`

### 🔹 Model Training

* Algorithm: **XGBoost Regressor**
* Trained on scaled training data

### 🔹 Evaluation

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)
* R² Score

### 🔹 Visualization

* Wine type distribution plot
* Wine quality distribution plot
* Correlation heatmap
* Actual vs Predicted plot
* Feature importance chart
* Residual error plot
* Prediction error distribution

---

## Model Used

* **XGBoost Regressor**

  * Handles complex relationships effectively
  * High prediction performance
  * Reduces overfitting
  * Works well on structured/tabular datasets

---

## Results

* MAE: 0.4501
* RMSE: 0.6074
* R² Score: 0.5005

The model achieved good baseline performance for ordinal prediction and successfully captured important patterns in wine quality data.

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* XGBoost
* Jupyter Notebook