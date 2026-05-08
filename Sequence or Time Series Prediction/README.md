# 🚦 Metro Interstate Traffic Volume Forecasting Project

## Overview

This project demonstrates a complete **Deep Learning pipeline** for **Time-Series Forecasting / Sequence Prediction**, which is a subtype of supervised learning where previous sequential observations are used to predict future values. In this project, an improved LSTM model learns traffic patterns and weather conditions to forecast future traffic volume using the Metro Interstate Traffic Volume dataset.

---

## Objective

To predict future traffic volume based on historical traffic and weather-related data using deep learning techniques for accurate time-series forecasting.

---

## Dataset

* **Dataset:** Metro Interstate Traffic Volume Dataset

* **File Used:**

  * `Metro_Interstate_Traffic_Volume.csv`

* **Features:**

  * Traffic volume
  * Temperature
  * Rainfall
  * Snowfall
  * Cloud coverage
  * Hour
  * Day of week
  * Month

* **Target Variable:**

  * Future traffic volume

---

## Workflow

### 🔹 Data Loading

* Loaded traffic dataset using Pandas
* Selected important traffic and weather-related features

### 🔹 Exploratory Data Analysis (EDA)

* Dataset information & statistics
* Traffic trend visualization
* Correlation heatmap
* Feature relationship analysis

### 🔹 Feature Engineering

* Converted `date_time` into datetime format
* Extracted:

  * Hour
  * Day of week
  * Month

### 🔹 Data Preprocessing

* Missing value handling
* Train-test split (80-20)
* Feature scaling using `MinMaxScaler`
* Sequence generation for time-series forecasting

### 🔹 Model Training

* Algorithm: **Stacked LSTM Neural Network**
* Trained on sequential traffic data
* Added dropout layers to reduce overfitting
* Used early stopping for better training

### 🔹 Evaluation

* Mean Absolute Error (MAE)
* Mean Squared Error (MSE)
* Root Mean Squared Error (RMSE)

### 🔹 Visualization

* Traffic volume trend plot
* Correlation heatmap
* Training vs validation loss plot
* Actual vs predicted traffic volume plot

---

## Model Used

* **LSTM (Long Short-Term Memory)**

  * Learns sequential and temporal patterns effectively
  * Suitable for time-series forecasting tasks
  * Captures long-term dependencies in sequential data
  * Performs well on traffic forecasting problems

---

## Results

* MAE: 242.74
* MSE: 133441.00
* RMSE: 365.29

The model achieved strong forecasting performance and successfully captured important traffic patterns from historical sequential data.

---

## Technologies Used

* Python
* NumPy
* Pandas
* Matplotlib
* Seaborn
* Scikit-learn
* TensorFlow / Keras
* Jupyter Notebook