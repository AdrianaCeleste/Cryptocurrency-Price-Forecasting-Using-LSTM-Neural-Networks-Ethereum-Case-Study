# Cryptocurrency Price Forecasting Using LSTM Neural Networks: Ethereum Case Study

## Executive Summary

This project applies a **Long Short-Term Memory (LSTM)** neural network to forecast Ethereum cryptocurrency prices using historical hourly market data. The workflow covers the complete data science lifecycle, including data preprocessing, exploratory data analysis (EDA), feature engineering, model development, evaluation, and future price forecasting.

The model achieved an **R² score of 0.995**, demonstrating excellent predictive performance for short-term Ethereum price forecasting.

---

## Business Problem

Cryptocurrency markets are highly volatile and influenced by multiple factors, making accurate price prediction a complex challenge.

Traditional forecasting methods often struggle to capture the nonlinear and sequential nature of financial time series. This project explores whether a deep learning model can learn historical price patterns to improve short-term forecasting accuracy for Ethereum.

---

## Methodology

The project followed these steps:

- Imported and cleaned historical Ethereum hourly price data.
- Performed Exploratory Data Analysis (EDA).
- Removed unnecessary features and verified data quality.
- Created time-based features from the datetime index.
- Generated sliding windows of **240 hours** for supervised learning.
- Normalized the data using **MinMaxScaler**.
- Built an **LSTM Neural Network** with TensorFlow/Keras.
- Evaluated the model using **R²**.
- Generated a **30-day (720-hour)** recursive forecast.

---

## Skills & Technologies

### Programming & Libraries

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- TensorFlow / Keras
- Scikit-learn

### Data Science Skills

- Time Series Forecasting
- Deep Learning
- LSTM Neural Networks
- Data Cleaning
- Feature Engineering
- Exploratory Data Analysis (EDA)
- Data Visualization
- Model Evaluation

---

## Results

- Successfully trained an LSTM model for Ethereum price forecasting.
- Achieved an **R² score of 0.995** on the test dataset.
- Training loss decreased consistently, indicating stable learning.
- Generated **720 hourly predictions** (30-day forecast).
- Predicted prices closely followed the actual market behavior during testing.

---

## Recommendations

- Include additional features such as:
  - Technical indicators (RSI, MACD, Moving Averages)
  - Bitcoin price
  - Trading volume trends
  - Market sentiment
  - Macroeconomic variables

- Perform hyperparameter optimization.

- Evaluate the model using additional metrics:
  - RMSE
  - MAE
  - MAPE

- Apply Time Series Cross Validation to improve model robustness.

---

## Next Steps

Future improvements include:

- Compare the LSTM model with:
  - GRU
  - Transformer Networks
  - XGBoost
  - Prophet
  - ARIMA

- Develop a real-time forecasting application using **Streamlit**.

- Connect to live cryptocurrency APIs for continuous predictions.

- Expand the model to forecast multiple cryptocurrencies (Bitcoin, Solana, Binance Coin, etc.).

- Build an interactive dashboard using **Power BI** or **Tableau**.

---

## Model Performance

| Metric | Result |
|---------|--------|
| Model | LSTM |
| Forecast Horizon | 30 Days (720 Hours) |
| Window Size | 240 Hours |
| Loss Function | Mean Squared Error (MSE) |
| Optimizer | Adam |
| R² Score | **0.995** |
