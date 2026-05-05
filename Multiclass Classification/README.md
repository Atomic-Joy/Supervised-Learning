# 🌸 Iris Multiclass Classification Project

## Overview

This project demonstrates a complete **Machine Learning pipeline** for **Multiclass Classification**, which is a type of supervised learning where the model predicts one label from more than two possible classes. In this case, the model learns patterns from labeled data to distinguish between multiple categories based on input features. using the Iris dataset.\

---

## Objective

To classify iris flowers into three species based on their features and develop a machine learning model for accurate prediction

---

## Dataset

* **Dataset:** Iris Dataset
* **Features:**

  * Sepal length
  * Sepal width
  * Petal length
  * Petal width
* **Target Classes:**

  * Setosa
  * Versicolor
  * Virginica

---

## Workflow

### 🔹 Data Loading

* Loaded using `sklearn.datasets`
* Converted into Pandas DataFrame

### 🔹 Exploratory Data Analysis (EDA)

* Dataset info & statistics
* Pairplot visualization for feature relationships

### 🔹 Data Preprocessing

* Train-test split (80-20)
* Feature scaling using `StandardScaler`

### 🔹 Model Training

* Algorithm: **Random Forest Classifier**
* Trained on scaled training data

### 🔹 Evaluation

* Accuracy Score
* Classification Report
* Confusion Matrix

### 🔹 Visualization

* Pairplot (feature relationships)
* Confusion Matrix heatmap
* Feature Importance bar chart

---

## Model Used

* **RandomForestClassifier**

  * Handles multiclass problems well
  * Robust to overfitting
  * Provides feature importance

---

## Results

* Accuracy: 100%
* Strong class separation
* Minimal misclassification

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
