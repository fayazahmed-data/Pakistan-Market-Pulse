# 📈 Pakistan Market Pulse: Economic Shifts & Equity Correlations (2020–2025)

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-Data_Analysis-150458.svg)
![yfinance](https://img.shields.io/badge/yfinance-Market_Data-green.svg)
![License](https://img.shields.io/badge/License-MIT-lightgrey.svg)

## 📌 Project Overview
This repository contains a quantitative financial analysis of the Pakistan Stock Exchange (PSX) covering the period from **January 1, 2020, to December 31, 2025**. 

Using the `Pakistan Market Pulse.ipynb` notebook, this project tracks a diversified portfolio of 10 heavyweight local equities alongside the macroeconomic benchmark of the US Dollar to Pakistani Rupee exchange rate (USD/PKR). The goal is to mathematically illustrate how domestic inflation, currency devaluation, and sector-specific fundamentals shaped market performance over five volatile years.

## ⚙️ Key Features & Methodology
1. **Moving Averages & Trend Detection:** Calculates 50-day and 200-day Simple Moving Averages (SMA) to identify bullish "Golden Cross" and bearish "Death Cross" signals.
2. **Base-100 Normalization:** Removes nominal price scale distortion (e.g., comparing a PKR 6,000 stock to a PKR 30 stock) to track true percentage-based portfolio growth.
3. **Macroeconomic Correlation Matrix:** Computes the Pearson correlation coefficient between individual stock sectors and the USD/PKR exchange rate.

---

## 📊 Visual Insights & Economic Shifts

### 1. The Macro Correlation Matrix
This heatmap illustrates the hidden interconnectedness of the PSX and how different sectors react to currency shocks.

*(Note: Rename your correlation matrix file to `correlation_matrix.png` or update the link below)*

![Correlation Matrix](Pakistan%20Market%20Pulse/correlation-matrix.png)

**Key Findings:**
* **The Tech Hedge (SYS.KA vs USD):** Systems Ltd exhibits a positive correlation (**0.53**) with the US Dollar. As an IT exporter earning in dollars but spending in rupees, it acts as a structural hedge against local currency devaluation.
* **The "Flock" Economy:** Traditional heavy-industry sectors (Fertilizer, Power, Banking) move in near lockstep (correlations of **0.85 to 0.96**), driven largely by systemic inflation rather than independent growth.
* **The Pharma Squeeze (SEARL.KA):** Searle Company shows a severe negative correlation (**-0.74**) with the Dollar. Relying on imported raw materials while facing strict local price controls, pharma margins are crushed when the PKR devalues.

### 2. Normalized Price Trends (Base-100)
By indexing all stocks to a starting value of 100, we can accurately compare the true return on investment across vastly different asset classes.

*(Note: Rename your line chart file to `normalized_trend.png` or update the link below)*

![Normalized Price Trend](Pakistan%20Market%20Pulse/relative-stock-performance.png)

**Key Findings:**
* Highlights which specific equities outperformed the broader macroeconomic headwinds.
* Demonstrates the volatility of individual assets compared to the smoothed-out performance of the heavily correlated traditional sector group.

---

## 🚀 Installation & Usage

To run this notebook locally and fetch the latest market data, follow these steps:

1. **Clone the repository:**
   ```bash
   git clone https://github.com/fayazahmed-data/Pakistan-Market-Pulse.git
   cd pakistan-market-pulse

2. **Install the required dependencies:**

   Ensure you have Python installed, then run:
   ```bash
   pip install pandas numpy matplotlib seaborn yfinance

4. **Run the Jupyter Notebook:**
   ```bash
   jupyter notebook "Pakistan Market Pulse.ipynb"

## 📂 Data Sources
**Equities Data:** Karachi Stock Exchange tickers via Yahoo Finance (.KA suffix).

**Currency Data:** US Dollar to Pakistani Rupee (PKR=X) via Yahoo Finance.

**Note:** The KSE-100 benchmark index ticker on Yahoo Finance is currently unstable, so macro comparisons rely on the USD/PKR exchange rate as the primary economic anchor.

### 📝 License
This project is open-source and available under the MIT License.
