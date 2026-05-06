# MultiLabel Classification Project

## Overview

This project demonstrates a complete Machine Learning pipeline for **Multilabel Classification**, which is a type of supervised learning where a single instance can belong to multiple classes simultaneously. The model learns patterns from labeled data and predicts multiple output labels for each sample using a `.arff` dataset.

---

## Objective

To build a multilabel classification model capable of predicting multiple target labels from input features and evaluate its performance using visualization and classification metrics.

---

## Dataset

* **Dataset Type:** `.arff`
* **Task:** Multilabel Classification
* **Input Features:** Multiple numerical/categorical attributes
* **Target:** Multiple labels per instance

---

## Workflow

### 🔹 Data Loading

* Loaded `.arff` dataset using `scipy.io.arff`
* Converted into Pandas DataFrame

### 🔹 Data Cleaning

* Decoded byte-string columns
* Converted categorical features into numeric values using `pd.factorize()`

### 🔹 Exploratory Data Analysis (EDA)

* Dataset information
* Label distribution visualization
* Feature correlation heatmap

### 🔹 Data Preprocessing

* Converted target labels using `pd.get_dummies()`
* Train-test split (80-20)
* Feature scaling using `StandardScaler`

### 🔹 Model Training

* Algorithm: **Random Forest Classifier**
* Wrapped using `MultiOutputClassifier`
* Used `class_weight='balanced'` for handling class imbalance

### 🔹 Evaluation

* Hamming Loss
* Subset Accuracy
* Classification Report
* Multilabel Confusion Matrix

### 🔹 Visualization

* Label distribution chart
* Correlation heatmap
* Confusion matrix heatmaps
* Feature importance bar chart

---

## Model Used

* **MultiOutputClassifier**

  * Converts single-output classifiers into multilabel classifiers

* **RandomForestClassifier**

  * Handles complex datasets efficiently
  * Reduces overfitting using ensemble learning
  * Provides feature importance scores

---

## Results

* Successfully trained multilabel classification model
* Generated predictions for multiple labels
* Visualized feature relationships and model performance
* Improved minority class handling using balanced class weights

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* SciPy