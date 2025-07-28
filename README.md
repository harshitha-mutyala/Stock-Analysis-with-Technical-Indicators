# Technical Stock Analysis Strategy

This is a Python project using historical stock data to generate basic buy/sell signals. The strategy is tested on Microsoft (MSFT) stock over a 6-month period.

## What the Project Does:
- Retrieves stock data using `yfinance`
- Calculates key indicators:
  - SMA (Simple Moving Average)
  - EMA (Exponential Moving Average)
  - RSI (Relative Strength Index)
- Detects buy/sell signals using SMA/EMA crossovers and RSI thresholds
- Simulates a basic backtest with $10,000 starting capital
- Visualizes signals and portfolio growth using `matplotlib`

## Tools Used:
- Python
- `Pandas`
- `Matplotlib`
- `yfinance`

## Results:
Crossover strategy: +5.27% return  
Combined (RSI + crossover): No trades triggered (overly strict filter)

## Limitations:
- No handling of transaction costs
- No stop-loss or risk management
- Combined signal logic was too conservative

## Future Improvements:
- Add transaction cost modelling
- Support partial trade or capital allocation
- Incorporate additional indicators (e.g., MACD, Bollinger Bands) 
- Tune RSI thresholds for better signal frequency

## Run It:
Open the notebook in Jupyter and follow the prompt to enter a stock ticker (e.g. `MSFT`).
The notebook will generate:
- Indicator plots
- Buy/sell signal visualizations
- Backtested portfolio performance
- Final return summary

