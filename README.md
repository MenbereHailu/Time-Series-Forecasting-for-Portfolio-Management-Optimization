# KAIM Weak 11 Challenge

## Time Series Forecasting for Portfolio Management Optimization

### Project Overview
This project aims to enhance portfolio management strategies for Guide Me in Finance (GMF) Investments by leveraging advanced time series forecasting models. By predicting future stock prices, market trends, and associated risks, we provide data-driven insights to optimize asset allocation, enhance returns, and manage risks effectively.

#### Objectives
The project’s primary goals are to:
1. Preprocess and analyze historical financial data for key assets.
2. Develop and evaluate time series forecasting models to predict future stock prices, with a focus on Tesla (TSLA).
3. Forecast future market trends and assess their implications on portfolio strategy.
4. Optimize an investment portfolio based on the forecasted data to maximize returns and minimize risks.

### Data Sources and Assets
Data was sourced using the `YFinance` Python library, covering the period from January 1, 2015, to October 31, 2024, for the following assets:
- **Tesla (TSLA)**: Represents a high-risk, high-reward stock.
- **Vanguard Total Bond Market ETF (BND)**: Provides stability and low risk.
- **S&P 500 ETF (SPY)**: Offers moderate-risk market exposure.

The dataset includes daily metrics such as Open, High, Low, Close, Adjusted Close, and Volume.

### Project Structure

```bash

    ├── data/
    │   ├── raw/                 
    │   └── processed/
    ├── figures/
    ├── scripts/
    │   ├── main.py                 
    ├── notebooks/
    ├── src/
    │    ├── data/
    │       ├── data_loader.py                 
    │       └── data_preprocessing.py
    │       └── train_test_split.py
    │    ├── eda/
    │       ├── price_analysis.py                 
    │       └── trend_analysis.py
    │       └── visualize.py
    │    ├── forecasting/
    │       ├── arima_model.py                 
    │       └── lstm_model.py
    │       └── sarima_model.py
    │       ├── prophet_model.py                 
    │       └── model_evaluation.py
    │    ├── portfolio/
    │       ├── optimization.py                 
    │       └── performance_metrics.py
    │       └── risk_metrics.py
    │    ├── utils/
    │       ├── time_utils.py                 
    │       └── yfinance_loader.py
    │    ├── utils.py
    ├── tests/    
    ├── README.md                
    ├── requirements.txt  

```

### Steps and Key Insights

#### Task 1: Preprocess and Explore the Data
1. **Data Cleaning**: We handled missing values and ensured all columns were appropriately typed.
2. **Exploratory Data Analysis (EDA)**: 
   - We visualized historical closing prices, calculated daily percentage changes to analyze volatility, and identified significant anomalies.
   - **Key Insights**: TSLA exhibited high volatility with substantial returns over time, BND maintained stability, and SPY provided moderate risk diversification.


