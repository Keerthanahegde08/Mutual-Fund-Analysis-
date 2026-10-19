# Mutual-Fund-Analysis-

A Python project that helps an investor build a diversified, risk-aware investment plan using Nifty 50 stock data. It measures risk and return, picks the best risk-adjusted stocks, builds a portfolio, and projects how a monthly SIP (Systematic Investment Plan) could grow over 1, 3, 5 and 10 years.

## What the project does

- Cleans and prepares daily closing price data
- Calculates return, volatility, Sharpe ratio and Sortino ratio for each stock
- Selects the top 10 stocks based on high return and low risk
- Builds conservative, balanced and aggressive portfolios
- Compares the portfolio with an equal-weight benchmark
- Projects SIP growth with a 10% yearly increase in the monthly amount
- Runs a Monte Carlo simulation to show the range of possible outcomes

## Dataset

Daily closing prices of 49 Nifty 50 stocks from 1 Jan 2024 to 30 May 2025 (348 trading days), stored in `nifty50_closing_prices.csv`.

## Files

- `MF_Investment_plan_final_results.ipynb` - full analysis with results
- `app.py` - optional Streamlit dashboard
- `nifty50_closing_prices.csv` - dataset
- `requirements.txt` - Python libraries needed


## Key results

- Selected stocks: BHARTIARTL, ICICIBANK, DIVISLAB, SUNPHARMA, M&M, APOLLOHOSP, MARUTI, HDFCBANK, BAJFINANCE, EICHERMOT
- Portfolio return: 30.9% a year, against 12.4% for the benchmark
- Volatility: 14.6%, about the same as the benchmark (14.8%)
- Sharpe ratio: 1.49, against 0.41 for the benchmark
- SIP projection (Rs 1,00,000 lump sum + Rs 5,000 a month, rising 10% a year): about Rs 19.3 lakh after 10 years at a 12% expected return, on Rs 10.6 lakh invested
- Monte Carlo (10 years): median Rs 18.3 lakh, with a 1.9% chance of ending below the amount invested

## Limitations

- Only about 1.4 years of data, so the figures are noisy
- Stocks are chosen using the same period they are evaluated on, so past performance looks better than it can be expected to be
- The benchmark is an equal-weight average of the stocks, not the official Nifty 50 index
- The data is stocks, not mutual fund NAVs, so expense ratios are not included

