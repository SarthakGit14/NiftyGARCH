# NiftyGARCH

A quantitative trading framework for Nifty 50 stocks that combines **EGARCH volatility forecasting**, **risk-adjusted stock selection**, **EMA-based trading signals**, and **portfolio hedging** to evaluate systematic trading strategies.

## Overview

NiftyGARCH forecasts stock volatility using EGARCH(1,1) models and ranks Nifty 50 stocks based on a custom risk-return scoring function. Selected stocks are traded using an EMA-based strategy and backtested against the Nifty 50 benchmark. An extended implementation also evaluates the effect of correlation-based hedging on portfolio performance.

## Features

- Historical Nifty 50 data collection using Yahoo Finance
- EGARCH(1,1) volatility forecasting
- Risk-adjusted stock ranking
- EMA-based trading strategy
- Portfolio backtesting
- Correlation-based hedging
- Interactive performance visualization
- Benchmark comparison with Nifty 50

## Repository Structure

```
NiftyGARCH/
│── NiftyGARCH.ipynb          # Main trading strategy
│── EGARCH+Hedging.ipynb      # Hedged portfolio strategy
│── NiftyGARCH_Report.pdf     # Project report
│── README.md
│── requirements.txt
```

## Methodology

1. Download historical prices of Nifty 50 stocks.
2. Forecast volatility using rolling EGARCH models.
3. Estimate expected returns.
4. Rank stocks using a custom risk-adjusted score.
5. Select the highest-ranked stocks.
6. Generate buy/sell signals using EMA bands.
7. Backtest portfolio performance.
8. Evaluate a hedged version using a correlated asset.

## Technologies

- Python
- Pandas
- NumPy
- yfinance
- ARCH
- Statsmodels
- Plotly
- Matplotlib

## Results

The strategy successfully identified high-performing stocks using volatility-aware selection and generated returns that outperformed the Nifty 50 benchmark during the evaluation period.

## Future Improvements

- Dynamic hedge ratio estimation
- Portfolio optimization
- Transaction cost modelling
- Walk-forward validation
- Machine learning-based return prediction

## Disclaimer

This project is intended solely for educational and research purposes and should not be considered investment advice./