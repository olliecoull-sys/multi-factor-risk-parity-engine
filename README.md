# Multi-Factor Hierarchical Risk Parity Engine

An institutional-grade systematic asset allocation framework built in Python that mitigates parameter estimation error using data-driven covariance shrinkage and modern tree clustering.

## Features
- **Data Pipeline:** Ingests daily adjusted closing price history for core factor proxy ETFs (Beta, Size, Value, Momentum, Quality).
- **Covariance Optimization:** Deploys a Ledoit-Wolf shrinkage estimator to strip statistical noise and stabilize empirical asset dependencies.
- **Tree-Clustering Allocation:** Avoids quadratic matrix inversion failures via Hierarchical Risk Parity (HRP) quasi-diagonalization and recursive bisection.
- **Out-of-Sample Backtesting:** Implements a strict walk-forward simulation using rolling historical windows to analyze strategy degradation under realistic market friction.

## Strategy Performance Overview
*Tip: Run the notebook in Google Colab to generate your specific performance statistics and insert them here.*

## Installation & Execution
1. Open Google Colab or your local Jupyter environment.
2. Clone or download this repository.
3. Install dependencies: `pip install yfinance PyPortfolioOpt scikit-learn scipy matplotlib seaborn`
4. Execute the cells sequentially to run the backtest framework.
