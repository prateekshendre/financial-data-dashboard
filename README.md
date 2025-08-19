# Financial Data Dashboard

Track portfolio performance, risk, and trends with Python for compute and Power BI for presentation.

## What this does
* Pulls daily prices for selected tickers
* Computes returns, rolling volatility, drawdowns, and Sharpe
* Exports clean CSVs for a Power BI dashboard

## Data
* Source: yfinance
* Example tickers: AAPL, MSFT, TSLA, AMZN, SPY

## Methods
* Python pandas for cleaning and feature creation
* Metrics: daily and cumulative returns, rolling stdev, drawdown, Sharpe

## Project layout
* data  CSV exports for Power BI
* notebooks  Jupyter workbooks
* visuals  screenshots for the README and LinkedIn
* src  optional helpers if you prefer scripts
* requirements.txt

## How to run
1. Create a virtual environment
2. pip install pandas numpy matplotlib yfinance plotly
3. Run the notebook notebooks portfolio_analysis.ipynb
4. Export data metrics.csv and prices.csv into the data folder
5. Build the Power BI dashboard using those CSVs

## Dashboard ideas
* Portfolio vs SPY cumulative return
* Risk return scatter by ticker
* Rolling volatility line chart
* Sharpe table

## Next steps
* Add sector weights and factor tilts
* Add simple forecast with moving average crossover
# financial-data-dashboard
Python + Power BI dashboard for portfolio performance and risk analysis
