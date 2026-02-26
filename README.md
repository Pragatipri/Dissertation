# Hybrid Machine Learning Model for Retail Sales Forecasting #
### MSc Data Science Dissertation – Kingston University (2025–2026) ###
Author: Pragati Priya

## Project Overview 

This dissertation presents the development of a hybrid retail sales forecasting model combining:

Facebook Prophet (trend + seasonality modelling)

XGBoost (residual error correction)

The objective is to improve forecasting accuracy for retail financial planning by reducing bias, capturing structural changes, and modelling non-linear patterns that traditional statistical models fail to detect.

The hybrid model achieved a ~9% improvement in RMSE compared to standalone baseline models.

## Business Motivation

Retail financial planning relies heavily on accurate sales forecasts. However:

Human forecasts are subject to cognitive bias (optimism bias, anchoring, overconfidence)

Traditional time-series models struggle with non-linearity and regime changes

Retail sales behaviour shifts due to promotions, seasonality, and market shocks

This project demonstrates how combining machine learning approaches can produce more robust forecasts for decision-making.

## Hybrid Model Architecture

### Step 1 – Prophet Baseline Model

Captures:

Trend

Yearly seasonality

Change points

Provides interpretable components

### Step 2 – Residual Extraction

Residuals computed as:

Residual = Actual Sales – Prophet Forecast

### Step 3 – XGBoost Residual Correction

Trained on:

Lag features

Rolling statistics

Time-based features

Learns non-linear patterns missed by Prophet

### Final Forecast
Final Forecast = Prophet Prediction + XGBoost Residual Prediction

## Evaluation Metrics

Models were evaluated using:

RMSE (Root Mean Squared Error)

MAE (Mean Absolute Error)

MAPE (Mean Absolute Percentage Error)

MPE (Mean Percentage Error)

The hybrid model reduced RMSE by approximately 9%, demonstrating improved predictive stability.

## Key Experiments Conducted

ARIMA vs SARIMA comparison

Log transformation vs differencing

ADF stationarity testing

ACF/PACF lag selection

Prophet and XGBoost hyperparameter tuning

Multiple time splits were explored within each standalone model 

Hybrid residual modelling

## Academic Context

This project was completed as part of the MSc Data Science programme at Kingston University.

The research explores:

Forecast model comparison

Human vs machine decision limitations

Bias reduction in financial planning

Practical implementation of ML in retail environments

## Contact

If you’d like to discuss this project, collaboration opportunities, or retail forecasting applications:

📧 pragati0228@gmail.com

🔗 https://www.linkedin.com/in/pragati-priya/
