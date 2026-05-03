# 🏠 Energy Efficiency Prediction — Portfolio Project

## 🚀 Project Summary

Built a **machine learning regression system** to predict building energy efficiency using the **Energy Efficiency Dataset**. This approach is used because the target variables, heating and cooling loads, are continuous numerical values, making regression models suitable for capturing relationships between building features and energy consumption. By training on historical data, the model learns patterns that help estimate energy requirements for new building designs, enabling better planning and optimization of energy efficiency.

The model estimates:

* Heating Load (Y1)
* Cooling Load (Y2)

based on architectural design features.

---

## 🎯 Objective

To analyze how structural parameters of buildings impact energy consumption and develop a predictive model to optimize energy efficiency.

---

## 🧠 Approach

### 🔹 Data Analysis

* Performed **EDA** using correlation heatmaps and regression plots
* Identified key features influencing energy load

### 🔹 Feature Engineering

* Cleaned and structured dataset
* Applied **feature scaling (StandardScaler)**

### 🔹 Model Development

Implemented and compared:

* Linear Regression (baseline)
* Random Forest Regressor
* Gradient Boosting Regressor

### 🔹 Evaluation

Used:

* R² Score (Coefficient of Determination): Measures how well the model explains the variance in the target variable (higher is better, max = 1).
* MAE (Mean Absolute Error): Calculates the average absolute difference between predicted and actual values.
* RMSE (Root Mean Squared Error): Measures the square root of the average squared differences, giving higher weight to large errors.
* Cross-validation: A technique to evaluate model performance by splitting data into multiple training and validation sets to ensure generalization.

---

## 📊 Key Results

* Achieved **R² score up to ~0.95+** using ensemble models
* Tree-based (Random Forest, Gradient Boosting) models significantly outperformed linear regression
* Identified **Surface Area & Overall Height** as major contributors

---

## 📈 Visual Insights

* Strong correlation between building geometry and energy load
* Residual analysis confirmed low bias and stable predictions
* Feature importance helped interpret model decisions

---

## 🛠️ Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn

---

## 💡 Impact

* Demonstrates ability to build **end-to-end ML pipelines**
* Shows understanding of **model comparison & evaluation**
* Highlights skills in **data visualization and interpretation**

---
