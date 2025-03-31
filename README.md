# Engine RUL Prediction: A Predictive Maintenance Approach

## Overview

This repository provides a comprehensive solution for predicting the Remaining Useful Life (RUL) of engines using sensor data. It implements traditional machine learning methods like Linear Regression and Random Forest, as well as a deep learning approach using LSTM networks. This project is aimed at enhancing predictive maintenance by accurately forecasting engine degradation and scheduling timely interventions.

## Project Structure

- **rul.py**: Main Python script that includes:
  - Data loading and preprocessing (handling multiple datasets)
  - Calculation of RUL for each engine instance
  - Model training and evaluation using Linear Regression, Random Forest, and LSTM networks
  - Visualization of actual vs. predicted RUL values
- **Data Files**:
  - Training datasets (e.g., `train_FD001.txt`, `train_FD002.txt`, etc.)
  - Test datasets (e.g., `test_FD001.txt`, `test_FD002.txt`, etc.)
  - Ground truth RUL files (e.g., `RUL_FD001.txt`, etc.)

## Features

- **Data Preprocessing:**  
  Cleans and preprocesses raw time-series data, including dropping features with zero variance and calculating RUL for each engine.

- **Machine Learning Models:**
  - **Linear Regression:** A baseline approach for predicting RUL.
  - **Random Forest:** Includes grid search for hyperparameter tuning to improve prediction accuracy.
  - **LSTM Neural Network:** Captures sequential dependencies in the data for improved time-series forecasting.

- **Visualization:**  
  Uses Matplotlib to create plots that compare actual vs. predicted RUL values, aiding in model evaluation and insights.

- **Evaluation Metrics:**  
  Measures performance using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).
