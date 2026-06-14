# Strategy Research & Optimization

The objective of this project was not to test a single strategy configuration, but to systematically optimize an intraday gap-breakout strategy.

## Parameters Tested

### Gap Thresholds

* 0.5%
* 1.0%
* 1.5%
* 2.0%

### Risk-Reward Ratios

* 0.5
* 1.0
* 1.5
* 2.0

### Time-Based Exits

* 11:00 AM
* 12:00 PM
* 1:00 PM
* 2:00 PM

Total Parameter Combinations Tested:

4 Gap Thresholds × 4 Risk-Reward Ratios × 4 Exit Times = 64 Backtests

## Evaluation Metrics

Each configuration was evaluated using:

* Total Profit (PnL)
* Win Rate
* Expectancy
* Profit Factor
* Trade Count
* Maximum Drawdown
* Sharpe Ratio

## Key Findings

### Gap Threshold

A 1% opening gap produced significantly higher-quality trades than a 0.5% gap.

Although 0.5% generated more trades and higher aggregate PnL, the expectancy per trade was lower.

### Risk-Reward Ratio

A Risk-Reward Ratio of 1.5 consistently outperformed both 1.0 and 2.0 configurations.

### Exit Time

A 1:00 PM time-based exit produced the highest expectancy among tested configurations.

## Best Configuration

* Gap Threshold = 1%
* Risk-Reward Ratio = 1.5
* Time Exit = 1:00 PM

## Final Backtest Results

* Trades: 129
* Win Rate: 56.59%
* Total Profit: 1079.55 Points
* Expectancy: 8.37 Points per Trade
* Sharpe Ratio: 3.63

## Comparison 
<img width="605" height="344" alt="image" src="https://github.com/user-attachments/assets/0eda0b60-b742-45fa-9c2c-65a17a2a8a20" />

## Results

    ## Equity Curve
       <img width="584" height="277" alt="image" src="https://github.com/user-attachments/assets/ab55243b-0018-4aea-96da-d48ee1d11a69" />

    ## Monthly Returns
       <img width="584" height="308" alt="image" src="https://github.com/user-attachments/assets/bba95ddc-ef1f-4a3a-b071-333cab15d293" />


