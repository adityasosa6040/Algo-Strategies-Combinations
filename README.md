# Algo-Strategies-Combinations

Algorithmic Trading Strategy Backtester for Nifty 50
This project provides a Python-based framework for backtesting and evaluating various algorithmic trading strategies on stocks from India's Nifty 50 index. It allows users to interactively select a stock and analyze the performance of four different trading models: Moving Average Crossover, Mean Reversion (RSI), Statistical Arbitrage (Pairs Trading), and a Machine Learning-based approach using a Random Forest Classifier.
The primary goal of this tool is to provide a clear, side-by-side comparison of how different strategies would have performed on a specific stock over a historical period, complete with performance metrics and graphical visualizations.
Key Features
Dynamic Data Loading: Automatically fetches the latest list of Nifty 50 constituents from Wikipedia.
Historical Price Data: Downloads historical stock data from Yahoo Finance (yfinance).
Interactive Stock Selection: Prompts the user to choose a stock from the downloaded Nifty 50 list to run the analysis on.
Multiple Trading Strategies: Implements four distinct and popular trading strategies:
Moving Average Crossover: A classic trend-following strategy using 50-day and 200-day moving averages.
Mean Reversion: A strategy based on the Relative Strength Index (RSI) to identify overbought and oversold conditions.
Statistical Arbitrage: A pairs trading model that identifies cointegrated stocks and trades on the divergence of their price spread.
Machine Learning: A predictive model using a Random Forest Classifier to forecast price direction based on lagged returns.
Performance Analytics: For the selected stock, it calculates and displays a performance summary table comparing all strategies on key metrics:
Cumulative Return: The total percentage gain or loss.
Annualized Volatility: A measure of the strategy's risk.
Sharpe Ratio: The risk-adjusted return, indicating the return per unit of risk taken.
Visualization: Generates a 2x2 plot showing the equity curve (portfolio value over time) for each of the four strategies, allowing for easy visual comparison.
How to Use
Installation:
Ensure you have Python installed. Then, install the required libraries:
pip install yfinance pandas numpy matplotlib seaborn statsmodels scikit-learn lxml


Execution:
Run the script from your terminal:
python your_script_name.py


Select a Stock:
The script will first download all the necessary data. It will then display a numbered list of available Nifty 50 stocks. Enter the number corresponding to the stock you wish to analyze and press Enter.
Analyze Results:
The script will:
Run all four trading strategies on the historical data of your selected stock.
Print the accuracy of the Machine Learning model.
Print a performance comparison table in your terminal.
Display a plot visualizing the portfolio growth for each strategy.
Technologies Used
Python 3
Pandas: For data manipulation and analysis.
NumPy: For numerical operations.
yfinance: To download historical market data from Yahoo Finance.
scikit-learn: For implementing the Machine Learning (Random Forest) model.
statsmodels: For the cointegration test used in the Statistical Arbitrage strategy.
Matplotlib & Seaborn: For data visualization and plotting.
Disclaimer: This project is for educational and informational purposes only. The trading strategies and backtesting results are based on historical data and are not indicative of future results. Trading in financial markets involves substantial risk, and you should not use this code for making real investment decisions without consulting a qualified financial advisor.
