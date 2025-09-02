Financial Data Dashboard

Quick summary
Project compares daily performance and risk of selected assets. Python does the data work. Visuals are produced with Seaborn and Matplotlib. Results export as images and CSVs for sharing and for a Power BI dashboard if needed.

What this does
1. Fetches daily prices using yfinance
2. Cleans and aligns time series with pandas
3. Computes daily returns, cumulative returns, rolling volatility, and drawdowns
4. Normalizes series to an index start 100 for clean comparison
5. Exports cleaned CSVs and publication ready PNG images

Data
Source: yfinance
Sample tickers used: BTC-USD, SPY, GLD, TLT

Key methods
pandas for ETL and feature creation
numpy for numeric ops
seaborn and matplotlib for plots
yfinance for price fetch

Repository layout
data
  raw.csv or readme describing how to regenerate raw data
notebooks
  01_explore_and_normalize.ipynb
  02_plots_and_exports.ipynb
scripts
  plot_performance.py
plots
  normalized_performance.png
  correlation_heatmap.png
requirements.txt
README.md

How to run locally
1. Create and activate a Python virtual environment
2. Install dependencies
   pip install -r requirements.txt
3. Run the notebook notebooks/01_explore_and_normalize.ipynb to generate cleaned CSVs in data
4. Run the script scripts/plot_performance.py to generate PNGs in plots

Repro command
python scripts/plot_performance.py --input data/prices.csv --out plots/normalized_performance.png

Suggested next visuals to add
1. Normalized performance line chart that starts all series at 100
2. Correlation heatmap of daily returns
3. Rolling 30 day correlation BTC versus SPY
4. Drawdown chart per asset
5. Snapshot table of cumulative return and annualized volatility

License
Add a short license line if you want public sharing
