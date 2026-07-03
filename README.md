# Stock-analysis

Early (2024) collection of equity-trading experiments in Python — my first pass
at a full pipeline from data to strategy ideas.

## What's here

| File | Purpose |
|---|---|
| `data_fetching.py` | Price data via yfinance; macro series via FRED (`FRED_API_KEY` env var) |
| `feature_engineering.py` | Technical features for modelling |
| `machine_learning_analysis.py` | ML models on engineered features |
| `reinforcement_learning.py` + `ppo_trained_model.zip` | PPO agent experiment |
| `backtesting.py`, `risk_management.py` | Simple backtest and position-risk helpers |
| `options_analysis.py`, `technical_*.py` | Options and technical-indicator utilities |
| `ui.py`, `user_interface.py` | Prototype UI |

## Setup

```bash
pip install yfinance pandas numpy scipy scikit-learn fredapi
export FRED_API_KEY=your_key   # free at fred.stlouisfed.org
```

## Honest status

This is exploratory student work: single-split evaluations, no transaction
costs, no significance testing. For how I evaluate strategies now — walk-forward,
costs, bootstrap inference — see
[dc-ml-trading](https://github.com/jarvisss007/dc-ml-trading).
