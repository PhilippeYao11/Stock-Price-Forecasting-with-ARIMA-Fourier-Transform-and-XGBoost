# 📈 Stock Price Forecasting with ARIMA, Fourier Transform, and XGBoost

This project aims to explore and forecast stock price movements using a combination of statistical, signal processing, and machine learning techniques.

We focus on a real-world dataset of banking sector stock prices and progressively build a complete analysis pipeline, from raw data exploration to predictive modeling.

---

## 🚀 Project Overview

- **Data Source**: Historical stock prices from multiple banks (e.g., Goldman Sachs, Citigroup, Morgan Stanley).
- **Period Analyzed**: From 2006-01-02 to 2018-05-04 (~3216 days).

### Workflow:

1. **Data Cleaning and Preparation**
   - Selection of "Close" prices.
   - Handling missing data and resampling.
   
2. **Technical Indicators Engineering**
   - Moving Averages (MA7, MA21)
   - MACD
   - Bollinger Bands
   - Exponential Moving Average (EMA)
   - Momentum and Log-Momentum

3. **Exploratory Signal Analysis**
   - Fourier Transform to analyze dominant frequency components.
   - Visualization of stock cycles at different levels of Fourier approximation.

4. **Statistical Modeling**
   - ARIMA(5,1,0) modeling of the stock price series.
   - Forecasting future prices with a rolling prediction strategy.
   - Evaluation using MSE (Mean Squared Error).

5. **Machine Learning Modeling**
   - Feature selection from technical indicators.
   - Training XGBoost Regressor for stock price prediction.
   - Feature Importance analysis to interpret model behavior.

---

## 📊 Key Results

- **ARIMA model** achieved low forecasting errors with simple autoregressive terms.
- **Fourier Transform** revealed dominant cycles in the stock movements.
- **XGBoost** identified **Momentum** as the most important technical indicator for forecasting.
- Comparative analysis between classical statistical methods and modern machine learning models.

---

## 🛠️ Libraries Used

- `numpy`, `pandas`
- `matplotlib`, `seaborn`
- `scikit-learn`
- `statsmodels`
- `xgboost`

