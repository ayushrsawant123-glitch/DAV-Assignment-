# DLF Stock Price Time Series Analysis & Forecasting

## Overview
This project analyzes DLF's daily historical stock data using an ARIMA time-series model to forecast the next 30 days of closing prices. By evaluating stationarity and ACF/PACF metrics, it successfully predicts a stable, sideways market trend.

## Features
* **Data Preprocessing:** Converts dates, cleans numerical strings, and handles missing values via forward-fill techniques.
* **Exploratory Data Analysis:** Visualizes historical trends and conducts the Augmented Dickey-Fuller (ADF) test to evaluate stationarity.
* **Autocorrelation Analysis:** Generates ACF and PACF plots on differenced data to determine optimal model parameters.
* **ARIMA Modeling:** Fits an ARIMA(1, 1, 1) model to the historical time series data.
* **Forecasting:** Predicts and visualizes the closing prices for the next 30 business days alongside historical data.
### Screenshots
   <img width="1111" height="606" alt="Closing Price Trend" src="https://github.com/user-attachments/assets/6b598f6e-8e35-41f9-9fcc-e18206508416" />
   <img width="1105" height="319" alt="Autocorrelation and Partial Correlation" src="https://github.com/user-attachments/assets/c940d1f7-c7b6-4597-b6b4-97d48d931464" />
   <img width="739" height="569" alt="Closing Price Forecast" src="https://github.com/user-attachments/assets/e0f6bdb1-4240-409d-8512-453b584b2c89" />


## Prerequisites
To run this project, you will need Python installed on your system along with the following libraries:
* pandas
* numpy
* matplotlib
* statsmodels

## Installation
1. Open your terminal in VS Code.
2. Ensure the dataset `Quote-Equity-DLF-EQ-16-03-2025-16-03-2026.csv` is located in the same directory as your Python script.
3. Install the required dependencies by running:
   ```bash
   pip install pandas numpy matplotlib statsmodels
### Usage
To execute the analysis and view the forecasts, run the main Python script from your VS Code terminal:

python main.py

The script will output the ADF statistics and the ARIMA model summary directly to the terminal console. It will also sequentially display three graphical plots:

Historical Closing Price Trend

Autocorrelation (ACF) and Partial Autocorrelation (PACF) Plots

30-Day Price Forecast
### Results & Interpretation
* Expected Trend: Stability (Sideways Movement)

* Conclusion: The time series analysis confirms the stock data exhibits non-stationary, random-walk behavior typical of efficient financial markets. After differencing, the ARIMA forecast projects a flat trend hovering around the 528-530 INR mark for the upcoming 30 days. This indicates near-term price stability based strictly on historical momentum.
