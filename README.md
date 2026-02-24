
# Pairs Trading — Statistical Arbitrage
A market-neutral pairs trading system built in Python.

## Results (2019–2024)
| Metric | Value |
|---|---|
| Total Return | +80.7% |
| CAGR | 14.0% |
| Sharpe Ratio | 1.80 |
| Max Drawdown | −22.8% |
| Win Rate | 58.3% |

## How it works
- Engle-Granger cointegration test to screen pairs
- Rolling OLS hedge ratio (120-day window)
- Z-score signals: entry ±2σ, exit ±0.5σ, stop ±3.5σ
- Portfolio of 3 pairs: KO/PEP, GS/MS, HD/LOW
- Transaction costs included

## Install
pip install yfinance statsmodels pandas numpy matplotlib seaborn
python pairs_trading_v3.py
