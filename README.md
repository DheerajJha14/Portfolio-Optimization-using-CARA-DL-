# Portfolio Optimization Using LSTM and CARA Utility

This project implements a portfolio optimization framework using a deep learning approach with an LSTM model trained to maximize a CARA (Constant Absolute Risk Aversion) utility function. The model predicts asset weights dynamically based on historical price and return data of ETFs.

## Features

- Load and preprocess historical ETF price data.
- Calculate and standardize returns and prices.
- Create input sequences combining price and return data for LSTM input.
- Define a custom PyTorch Dataset and DataLoader for training.
- Implement an LSTM model predicting portfolio weights with a softmax output.
- Use a CARA utility-based loss function for training.
- Evaluate portfolio performance with financial metrics such as Sharpe Ratio, Sortino Ratio, Alpha, Beta, Maximum Drawdown.
- Visualize cumulative returns of individual ETFs and the optimized portfolio.

## Requirements

- Python 3.7+
- pandas
- numpy
- torch (PyTorch)
- matplotlib
- seaborn
- scipy

## Usage

1. Place your ETF CSV files (with `Date` and `Close` columns) in the project folder.  
   Example files: `VTI.csv`, `AGG.csv`, `DBC.csv`, `VIX.csv`

2. Run the main script:  
   ```bash
   python your_script.py
