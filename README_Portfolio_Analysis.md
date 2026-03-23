# Portfolio Analysis of Five Market Leaders

This project analyses a five-asset portfolio using historical Yahoo Finance data for:

- NVDA
- GLD
- JPM
- XOM
- SPY

## What the notebook covers
- data collection with `yfinance`
- daily log returns
- annualised return and volatility
- correlation and covariance analysis
- Monte Carlo simulation of 10,000 random portfolios
- portfolio optimisation:
  - minimum variance portfolio
  - maximum Sharpe ratio portfolio
- risk metrics:
  - 95% historical 1-day VaR
  - maximum drawdown
  - beta versus SPY

## Key improvement over the earlier version
The notebook fixes a major return-scaling issue in the Monte Carlo simulation.  
Annual portfolio returns are **not** multiplied by 252 twice.

## Tools used
- Python
- pandas
- numpy
- matplotlib
- scipy
- yfinance

## Notes
- `GLD` and `SPY` are ETFs, so this is best described as a **multi-asset portfolio analysis** rather than a pure stock-only study.
- A 2% annual risk-free rate is used for Sharpe ratio calculations.
- Results depend on the selected historical sample period and should not be treated as investment advice.

## Files
- `Portfolio Analysis of Five Market Leaders Using Python.ipynb` — cleaned and improved analysis notebook
