# Stat131: Time Series and Prediction, Final Project:

## 📈 USD/EUR Exchange Rate Forecasting with ARMA-GARCH
This project models and forecasts the weekly returns and volatility of the USD/EUR foreign exchange rate using time series techniques. Using data from FRED (2009–2025), we preprocess the series into weekly log returns and evaluate multiple time series models, ultimately selecting an ARMA(0,1) + GARCH(2,1) model with Student-t errors.

## 🔍 Key Highlights
- Data Source: FRED DEXUSEU daily rates, aggregated into weekly averages
- Preprocessing: Log-differenced to capture weekly return rates (825 observations)
- Modeling Strategy: Evaluated ARIMA, GARCH, IGARCH, and random walk alternatives
- Final Model: ARMA(0,1) for short-term autocorrelation + GARCH(2,1) for volatility clustering
- Diagnostics: Residual analysis, McLeod-Li, Ljung-Box, and normality tests
- Findings: Volatility is highly persistent; returns show marginal serial correlation but are indistinguishable from zero on average—supporting weak-form market efficiency
- Forecast Horizon: 10-week forecasts show slow volatility decay, highlighting "volatility regimes"

## 📊 Tools Used
- R (forecasting, time series analysis)
- ACF/PACF, EACF, McLeod-Li, Portmanteau tests
