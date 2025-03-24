# Quantitative-Financial-Modeling-of-Multi-Asset-Strategies-with-Monte-Carlo-Portfolio-Optimization 🚀

A Python-based portfolio construction engine that utilizes technical trading strategies like Moving Average Crossovers and Bollinger Bands, coupled with Monte Carlo simulations and Mean-Variance Optimization, to maximize Sharpe ratio while controlling for beta risk.

## 📈 Project Overview

This project was built as part of the BUDT 758i course at the University of Maryland. The objective was to:
- Implement technical strategies for 12 instruments (equities, bonds, commodities, and currencies)
- Construct a diversified 8-asset portfolio with constraints on Sharpe (>1.0) and Beta (≤0.5)
- Optimize portfolio weights using Monte Carlo simulations (5000 iterations)
- Evaluate and visualize performance, risk, and correlation metrics

## ⚙️ Strategies Implemented

- **BMK-MA**: Base instrument
- **MAFlat**: Moving Average crossover strategy (flat when bearish)
- **MAShort**: Moving Average crossover strategy (short when bearish)
- **BB**: Bollinger Band-based trading strategy

All technical strategies are parameterized and tested for:
- Uniform parameter usage across strategies to avoid overfitting
- Portfolio beta and Sharpe constraints

## 🧠 Key Features

- ✅ Wrapper function to combine Moving Average and Bollinger Band outputs
- ✅ Strategy selection logic and rationale
- ✅ Sensitivity analysis for optimal parameters
- ✅ Mean-Variance Optimization with 5000 Monte Carlo samples
- ✅ Portfolio performance statistics: Sharpe, beta, max drawdown
- ✅ Visualization of efficient frontier and portfolio risk-return profiles

## 📊 Tools & Libraries

- `pandas`, `numpy` for data manipulation
- `matplotlib`, `seaborn` for plotting
- `scipy.optimize`, `cvxpy` (optional) for optimization
- `sklearn` for beta regression
- `jupyter notebook` for interactive coding

## 🔍 Notable Results

- **Best Portfolio Sharpe**: 1.45  
- **Portfolio Beta to SPY**: 0.38  
- **Max Drawdown Reduced** by ~25% compared to benchmarks  
- **Diversification Strategy**: Mix of equities, bonds, commodities, and forex

## 📈 Visuals

Efficient Frontier with Minimum Volatility and Maximum Sharpe Portfolios:
![Efficient Frontier](plots/efficient_frontier.png)
