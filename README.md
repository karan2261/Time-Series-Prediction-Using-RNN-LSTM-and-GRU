# Time-Series-Prediction-Using-RNN-LSTM-and-GRU
A time-series project using RNN, LSTM, and GRU for analyzing the performance of each models.

## Overview
This project focuses on time-series forecasting using three neural network architectures: SimpleRNN, LSTM, and GRU. The primary goal is to predict stock closing prices using a dataset of 10 years of historical stock data.

## Features
- **Data Preprocessing**:
  - Normalization of numerical features using MinMaxScaler.
  - Creation of sequences for time-series modeling.
  - Handling of date column for proper sequence alignment.
- **Model Training**:
  - SimpleRNN, LSTM, and GRU models trained with varying sequence lengths (10, 60, 120 days).
  - Custom evaluation using metrics such as Mean Squared Error (MSE), Mean Absolute Error (MAE), R-squared (R²), Mean Absolute Percentage Error (MAPE), and Symmetric Mean Absolute Percentage Error (sMAPE).
- **Visualization**:
  - Performance comparison using bar plots of key metrics across all models and sequence lengths.

## Dataset
- Historical stock price data spanning 10 years.
- Key features include `Open`, `High`, `Low`, `Close`, and `Volume`.

## Workflow
1. **Data Preprocessing**:
   - Convert the `Date` column to datetime format.
   - Normalize numerical features for consistent scaling.
   - Generate sequences for time-series modeling.
2. **Model Training**:
   - Train SimpleRNN, LSTM, and GRU models for 10, 60, and 120-day sequence lengths.
   - Validate models using 20% of the training data.
3. **Evaluation**:
   - Compute metrics (MSE, MAE, R², MAPE, sMAPE) for each model and sequence length.
   - Compare models based on performance metrics.
4. **Visualization**:
   - Generate comparative bar plots for metrics across all models and sequence lengths.

## Results
- **Best Performing Model**: GRU consistently outperformed SimpleRNN and LSTM across most metrics and sequence lengths.
