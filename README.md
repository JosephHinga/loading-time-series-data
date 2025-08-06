# loading-time-series-data
🌡️ Time Series Forecasting of Daily Minimum Temperatures
📌 Introduction
This project applies time series analysis and forecasting techniques to predict the daily minimum temperatures in Sydney, Australia. Using 10 years of historical data, the project demonstrates the process of exploratory data analysis, model building, evaluation, and forecasting.

The project is designed as part of my data science portfolio to highlight my expertise in:

Time series modeling (ARIMA & SARIMA)

Data preprocessing and analysis

Statistical testing for stationarity

Forecasting evaluation with industry-standard metrics

 ## Problem Statement ## 
Accurate daily temperature forecasting is vital in agriculture, energy planning, transportation, and climate research.
The dataset exhibits strong seasonality and requires specialized models capable of capturing periodic cycles and underlying patterns.

The goal is to build a model that produces accurate forecasts while providing insights into seasonal and trend components.

## Dataset ##
Name: Daily Minimum Temperatures – Sydney, Australia

Source: Kaggle

Period Covered: January 1981 – December 1990

Size: 3,650 daily observations

Features:

Date: Daily calendar date (datetime index)

Temp: Daily minimum temperature in Celsius (°C)

🔎 Exploratory Data Analysis
Key insights from the data:

Trend: Long-term average remained relatively stable.

Seasonality: Clear yearly cycles (warmer summers, colder winters).

Distribution: Temperatures ranged from ~5°C to ~25°C.

Stationarity Test: Augmented Dickey-Fuller (ADF) test confirmed non-stationarity, requiring differencing.

Visualizations included:

Time series plots of 10 years of temperatures

Seasonal decomposition (trend, seasonality, residuals)

Rolling averages and moving statistics

Autocorrelation (ACF) and Partial Autocorrelation (PACF) plots

## Methodology ##
1. Data Preprocessing
Converted Date to datetime and set as index

Ensured no missing values

Applied differencing to achieve stationarity

Generated plots for exploratory analysis

2. Modeling
Baseline Models

Naïve Forecast

Moving Average

Advanced Models

ARIMA (AutoRegressive Integrated Moving Average)

SARIMA (Seasonal ARIMA) with yearly seasonality

3. Evaluation Metrics
RMSE (Root Mean Squared Error)

MAE (Mean Absolute Error)

MAPE (Mean Absolute Percentage Error)

📊 Results
Best Performing Model: SARIMA

Performance Metrics:

RMSE: Value obtained from model evaluation

MAE: Value obtained from model evaluation

Visualization: SARIMA forecasts closely aligned with actual observed temperatures, capturing seasonal cycles effectively.

📌 Key Insights
Sydney’s minimum temperatures show a clear yearly cycle.

SARIMA outperforms simpler baseline models by leveraging seasonal differencing.

Proper stationarity checks and ACF/PACF analysis are crucial for parameter selection in ARIMA models.

🚀 Future Work
Incorporate deep learning models such as LSTM/GRU for advanced forecasting.

Add exogenous variables (humidity, rainfall, wind speed) for multivariate forecasting.

Build a Streamlit dashboard for interactive real-time predictions.

🛠️ Tech Stack
Python: Pandas, NumPy

Visualization: Matplotlib, Seaborn

Time Series Modeling: Statsmodels (ARIMA, SARIMA)

Evaluation: Scikit-learn metrics

Environment: Jupyter Notebook

👨‍💻 Author
Joseph Mwangi
📧 your.email@example.com
🔗 [Your GitHub or LinkedIn Profile]