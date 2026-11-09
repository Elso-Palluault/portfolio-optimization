# Portfolio Optimization with Mean-Variance Analysis

Building a diversified portfolio of 8 exchange-traded funds (US, developed and emerging equities, Treasuries, corporate bonds, gold, real estate) using modern portfolio theory, in Python (pandas, NumPy, SciPy, matplotlib, yfinance).

**Status: complete.**

## Steps
- [x] Step 1: Data download (2015-2025), daily returns, annualized return and volatility, return per unit of risk
- [x] Step 2: Covariance and correlation matrices
- [x] Step 3: Portfolio return and volatility
- [x] Step 4: Random portfolio simulation
- [x] Step 5: Minimum variance and maximum Sharpe ratio portfolios
- [x] Step 6: Comparison with a benchmark (weights estimated on 2015-2020, tested on 2021-2025 against SPY and an equal-weight portfolio)

## Key findings
- Over 2015-2025, gold (GLD) delivered the best return per unit of risk (0.84), slightly ahead of US equities (SPY, 0.80), while long-term Treasuries (TLT) ranked last (0.02) after the 2022 interest rate hikes.
- Over the full period, the maximum Sharpe portfolio combines gold (55.5%) and US equities (44.5%), with a Sharpe ratio of 0.97, against 0.49 for an equal-weight portfolio.
- Weights estimated on 2015-2020 relied on Treasuries instead and underperformed SPY out of sample (Sharpe ratio of 0.38 against 0.75), as the 2022 rate hikes made bonds fall together with equities.
- Even the minimum variance portfolio suffered a maximum drawdown of -19.5% in 2021-2025: low volatility does not guarantee small losses when correlations change.

Data: Yahoo Finance, adjusted daily closing prices. Educational project.
