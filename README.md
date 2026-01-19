# Multi-Asset-Worst-Of-Autocallable-Pricer

This project features a Monte Carlo pricing engine for a complex Equity Derivative (Worst-Of Autocall) on a basket of stocks (AAPL, GOOG, TSLA, MSFT). The model captures path-dependency and correlation dynamics between underlyings.

Product Specifications
Underlyings: Multi-asset basket (Worst-Of logic).

Technical Implementation
Stochastic Model: Multi-Asset Geometric Brownian Motion (GBM) in a risk-neutral framework.
Correlation: Cholesky Decomposition applied to the historical covariance matrix.
Performance: 1,000,000 paths simulated using NumPy vectorization for high computational efficiency.

Data: Automated historical data retrieval via yfinance API.

Analysis: The valuation accounts for the asymmetric risk-return profile and the correlation risk embedded in the "Worst-Of" mechanism.

The initial parameters can be modified to price different types of Autocallable 
