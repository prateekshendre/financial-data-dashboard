# 📊 Financial Data Dashboard

Track **portfolio performance, risk, and trends** with Python for computation and Seaborn/Matplotlib for visualization.
Exports clean CSVs and plots for sharing and future dashboarding (e.g., Power BI).

---

## 🚀 What This Project Does

* **Fetches** daily asset prices via `yfinance`
* **Cleans & aligns** data with `pandas`
* **Computes** daily returns, cumulative returns, rolling volatility, and drawdowns
* **Normalizes** assets to start at 100 for comparison
* **Exports** publication-ready plots and CSV files

---

## 📂 Data

* **Source:** Yahoo Finance (`yfinance`)
* **Assets used:**

  * Bitcoin (**BTC-USD**)
  * US Equities (**SPY**)
  * Gold (**GLD**)
  * US Treasuries (**TLT**)

---

## 🛠 Methods & Tools

* **pandas** – data wrangling
* **numpy** – numeric ops
* **yfinance** – financial data fetch
* **matplotlib & seaborn** – plots
* **Jupyter Notebook** – analysis workflow

---

## 📁 Repository Layout

```

financial-data-dashboard/
│
├── data/                   # Cleaned CSVs
│   ├── prices.csv
│   └── returns.csv
│
├── notebooks/              # Jupyter notebooks
│   └── dashboard_analysis.ipynb
│
├── plots/                  # Exported PNG visuals
│   ├── normalized_performance.png
│   ├── correlation_heatmap.png
│   ├── rolling_corr_btc_spy.png
│   ├── drawdowns.png
│   └── summary_table.png
│
├── README.md               # Project overview
├── LICENSE                 # License info
└── .gitignore              # Ignore rules


```

---

## 🖼 Key Visuals

1. **Normalized Performance** – BTC vs SPY vs GLD vs TLT (index = 100 start)
2. **Correlation Heatmap** – asset return correlations
3. **Rolling 30d Correlation** – BTC vs SPY dynamics
4. **Drawdowns** – peak-to-trough performance per asset
5. **Summary Table** – returns and volatility snapshot

*All plots saved in `/plots` as high-res PNGs for LinkedIn and reports.*

---

## ⚡ How to Run Locally

1. Clone repo

   ```bash
   git clone https://github.com/your-username/financial-data-dashboard.git
   cd financial-data-dashboard
   ```
2. Create a virtual environment

   ```bash
   python -m venv venv
   source venv/bin/activate   # or venv\Scripts\activate on Windows
   ```
3. Install dependencies

   ```bash
   pip install -r requirements.txt
   ```
4. Run notebooks to generate data + plots

   ```bash
   jupyter lab
   ```

---

## 📌 Example Command

Generate normalized performance plot from script:

```bash
python scripts/plot_performance.py --input data/prices.csv --out plots/normalized_performance.png
```

---

## 🔮 Next Steps

* Add **sector weights** & factor analysis
* Extend **rolling metrics** (volatility, Sharpe)
* Add **forecast overlays** with moving averages

---

## 📜 License

MIT License
