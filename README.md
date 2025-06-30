# Time-series_walmart_dataset

**README.md – Walmart Time Series Forecasting (Department 29)**

---

# Walmart Weekly Sales Forecasting – Department 29

Forecasting Walmart's weekly sales using various time series models, machine learning, deep learning, and deployment with Streamlit.

## Project Overview

This project aims to forecast weekly sales for Walmart's Department 29 using classical and modern time series approaches. It involves exploratory analysis, model comparison, and real-time deployment via a Streamlit web app.

## Dataset

* Source: Cleaned Walmart dataset
* Department: 29 (assigned)
* Period: Feb 2010 – Oct 2012
* Features: Date, Weekly\_Sales, IsHoliday, Temperature, Fuel\_Price, CPI, Unemployment

## Time Series Analysis

* Trend and seasonality detected
* Stationarity tested with Augmented Dickey-Fuller (ADF)
* ACF/PACF analysis

## Models Applied

### Exponential Smoothing:

* Naive Forecast
* Simple & Moving Average
* Single Exponential Smoothing (SES)
* Holt Linear Trend
* Holt-Winters Additive

### ARIMA Family:

* ARIMA
* SARIMA
* SARIMAX (with external regressors)

### Machine Learning:

* Random Forest Regressor
* Gradient Boosting
* XGBoost
* Linear Regression

### Deep Learning:

* Artificial Neural Network (ANN)
* Long Short-Term Memory (LSTM)

### Innovation:

* Prophet (by Facebook)
* N-BEATS (deep time series model)

## Model Evaluation

| Model         | MAE  | RMSE | MAPE  | R²    |
| ------------- | ---- | ---- | ----- | ----- |
| Holt-Winters  | 338  | 491  | 7.5%  | 0.90  |
| Prophet       | 398  | 498  | 10.4% | -0.49 |
| Random Forest | 398  | 490  | 10.7% | -0.45 |
| XGBoost       | 419  | 514  | 10.9% | -0.59 |
| ANN           | 674  | 764  | 17.2% | -2.52 |
| SARIMAX       | 4430 | 5353 | 96.1% | N/A   |

**Best Model:** Holt-Winters (Additive)

## Deployment

The best model (Holt-Winters) was deployed using Streamlit.
Users can select the number of weeks to forecast, and the app returns predicted sales values with visualizations.

**Live Demo:** [Streamlit App](https://your-streamlit-app-link.streamlit.app)

## Tech Stack

* Python
* Pandas, NumPy
* Statsmodels, Scikit-learn, XGBoost
* TensorFlow/Keras
* Facebook Prophet
* Streamlit
* Git & GitHub

## What I Learned

* Time Series analysis and model selection
* Forecasting evaluation metrics (MAE, RMSE, MAPE, R²)
* Deep learning for sequential data
* Streamlit deployment and GitHub integration
* End-to-end data science pipeline

## Author

**Fayrouz Mohamed**
[GitHub](https://github.com/fayrouzmgalal) | [LinkedIn](https://www.linkedin.com/in/fayrouz-mohamed-556a6b241)

---

\#️⃣ Keywords: Time Series, Walmart Sales Forecasting, Holt-Winters, Machine Learning, Streamlit, Python
