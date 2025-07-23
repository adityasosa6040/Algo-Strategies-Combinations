# Algo-Strategies-Combinations
# Algorithmic Trading Strategy Backtester for Nifty 50

![Python](https://img.shields.io/badge/Python-3.x-blue.svg)
![License](https://img.shields.io/badge/License-MIT-green.svg)
[![Open Source](https://badges.frapsoft.com/os/v1/open-source.svg?v=103)](https://opensource.org/)

A comprehensive Python framework for backtesting algorithmic trading strategies on India's Nifty 50 index constituents.

---

## Table of Contents
- [Features](#features)
- [Usage](#usage)
- [Implemented Strategies](#implemented-strategies)
- [Performance Metrics](#performance-metrics)
- [Sample Output](#sample-output)
- [Disclaimer](#disclaimer)
- [Technologies Used](#technologies-used)
---

## Features

📈 **Dynamic Data Loading**  
Automatically fetches the latest Nifty 50 constituents from Wikipedia

🔄 **Historical Price Data**  
Downloads stock data from Yahoo Finance (yfinance)

🔍 **Interactive Stock Selection**  
Choose any Nifty 50 stock for analysis through CLI interface

📊 **Four Trading Strategies**:
1. Moving Average Crossover (50-day & 200-day)
2. Mean Reversion (RSI-based)
3. Statistical Arbitrage (Pairs Trading)
4. Machine Learning (Random Forest Classifier)

📉 **Performance Analytics**:
- Cumulative Return
- Annualized Volatility
- Sharpe Ratio

📊 **Visualization**  
2x2 plot comparing strategy performance over time

---

## Usage

The script will:
1. Download Nifty 50 constituents
2. Present an interactive stock selection menu
3. Run all four strategies on selected stock
4. Display performance metrics and visualizations

---

## Implemented Strategies

| Strategy                | Type           | Indicators Used                         |
|------------------------|----------------|------------------------------------------|
| Moving Average Crossover | Trend-following | 50-day & 200-day MA                     |
| Mean Reversion (RSI)     | Counter-trend   | RSI (14-period)                          |
| Statistical Arbitrage    | Pairs trading   | Cointegration test, Z-score              |
| Machine Learning         | Predictive      | Random Forest, Lagged Returns            |

---

## Performance Metrics

| Metric                 | Description                                      |
|------------------------|--------------------------------------------------|
| **Cumulative Return**  | Total strategy return over backtest period       |
| **Annualized Volatility** | Standard deviation of returns (risk measure)   |
| **Sharpe Ratio**       | Risk-adjusted return (return per unit of risk)   |

---

## Sample Output

```text
Selected Stock: RELIANCE.NS

Machine Learning Model Accuracy: 72.5%

Strategy Performance Comparison:
+------------------------+-------------------+---------------------+---------------+
| Strategy               | Cumulative Return | Annualized Volatility | Sharpe Ratio  |
+------------------------+-------------------+---------------------+---------------+
| Moving Average         | 45.2%             | 18.7%               | 1.42          |
| Mean Reversion (RSI)   | 32.1%             | 15.3%               | 1.18          |
| Statistical Arbitrage  | 28.7%             | 12.9%               | 1.05          |
| Machine Learning       | 51.3%             | 20.1%               | 1.58          |
+------------------------+-------------------+---------------------+---------------+
```

---

## Disclaimer

⚠️ **Important Notice**  
This project is for **educational purposes only**. Past performance does not guarantee future results. Trading involves substantial risk of loss. The authors are not responsible for any financial losses incurred by using this software.

---

## Technologies Used

- Python 3
- Pandas (Data manipulation)
- NumPy (Numerical operations)
- yfinance (Market data)
- scikit-learn (Machine Learning)
- statsmodels (Statistical tests)
- Matplotlib / Seaborn (Visualization)

---
