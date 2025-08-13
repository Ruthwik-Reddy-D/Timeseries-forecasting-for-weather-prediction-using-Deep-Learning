Timeseries Weather Forecasting using Deep Learning
**Author:** Ruthwik Reddy Devarapalli
**Date Created:** 2025-5-13
**Description:** This document describes the process and methodology for performing time series forecasting for weather prediction using LSTM deep learning models.
Introduction
Weather forecasting is an inherently challenging problem due to the complex, non-linear nature of atmospheric patterns. This project leverages the Jena Climate Dataset to forecast future temperature values using Long Short-Term Memory (LSTM) neural networks. The work focuses on effective preprocessing, temporal windowing, and evaluation to achieve accurate forecasts.
Dataset
Source: Max Planck Institute for Biogeochemistry (https://www.bgc-jena.mpg.de/wetter/)
Location: Jena, Germany
Time Period: January 10, 2009 – December 31, 2016
Frequency: Recorded every 10 minutes
Features: 14 weather parameters including temperature, pressure, humidity, and wind speed.
Methodology
1. Data Preprocessing: Loading dataset, parsing datetime, handling missing values, scaling features using MinMaxScaler.
2. Windowing: Creating input sequences of fixed length for multi-step forecasting.
3. Model Architecture: LSTM layers followed by Dropout and Dense layers, optimized with Adam and evaluated using Mean Squared Error.
4. Training & Evaluation: Training over multiple epochs with validation sets, measuring RMSE and MAE.
Results
The LSTM model successfully captures both seasonal and short-term patterns in the climate data. RMSE and MAE values indicate good performance, though further improvement is possible with hyperparameter tuning, feature engineering, and alternative architectures such as GRU or CNN-LSTM.
Future Work
- Explore GRU and Transformer-based architectures.
- Incorporate additional meteorological datasets for better generalization.
- Deploy the forecasting model as a real-time web application using Flask or FastAPI.
