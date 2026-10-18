# Stock Price Forecasting Experiment with LSTM Networks

> **Learning notebook / early data science project.** This repository is preserved to show experimentation with sequence models; it is not an investment tool.

A Google Colab notebook that downloads historical Alphabet (`GOOGL`) market data with `yfinance` and experiments with a bidirectional LSTM for next-step price forecasting.

## What the notebook does

1. Download daily `GOOGL` data beginning in January 2018.
2. Explore historical price trends.
3. Create scaled rolling sequences for a neural network.
4. Split the sequence chronologically into training and testing periods.
5. Train a multi-layer bidirectional LSTM in TensorFlow/Keras.
6. Plot predictions against observed values on the test period and full history.

## Repository guide

- `StockMarket.ipynb` — complete Colab workflow, including data download, preprocessing, model definition, training, and visual comparison

[Open the notebook in Google Colab](https://colab.research.google.com/github/kasteway/Stock_Prediction/blob/main/StockMarket.ipynb)

## Tools

Python, pandas, NumPy, yfinance, scikit-learn preprocessing, TensorFlow/Keras, and Matplotlib.

## What this project demonstrates

- Preparing time-ordered sequences for neural networks
- Scaling features and reversing transformations for interpretation
- Building and training a recurrent model
- Visualizing predictions against a chronological holdout period

## Limitations

The notebook does not preserve a benchmark comparison or final test metric, so no claim of predictive advantage is made. It also does not account for transaction costs, survivorship bias, corporate actions beyond the downloaded series, or the non-stationary nature of markets. Visual fit alone is not evidence of a profitable strategy. A rigorous extension would add naïve baselines, walk-forward validation, error metrics, uncertainty estimates, and leakage checks.
