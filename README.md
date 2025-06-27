# AlgoTrading-ML-Automation

A mini algo-trading prototype using RSI & DMA strategy, ML-based predictions, and Google Sheets automation.

## 📌 Overview
This project implements an automated trading system prototype that:

- Fetches historical stock data for NIFTY 50 stocks from Yahoo Finance.
- Applies a technical trading strategy combining RSI and moving average crossovers.
- Uses basic machine learning models to predict next-day stock price movement.
- Logs trades and performance metrics automatically to Google Sheets.
- Calculates and displays trade PnL and win ratio for performance analysis.

## ⚙️ Features

- **Technical Indicators:** RSI (14-day), 20-day & 50-day moving averages.
- **Trading Signals:** Buy when RSI < 30 and 20DMA crosses above 50DMA.
- **Machine Learning:** Logistic Regression and Decision Tree classifiers on RSI, MACD, and volume.
- **Automation:** Google Sheets integration for live trade logs and PnL summaries.
- **Modular Code:** Functions organized for data fetching, indicator calculation, signal generation, ML modeling, and Google Sheets updates.

## 🧠 Machine Learning Details

- Input features: RSI, MACD (and its components), and trading volume.
- Target: Binary classification of next-day price movement (up/down).
- Models implemented: Logistic Regression and Decision Tree.
- Achieved around 60% accuracy with Decision Tree.

## 📤 Google Sheets Automation

- Trade signals and related metrics logged in "Trade Log" sheet.
- Summary tab includes total trades, wins, win ratio, and net PnL.
- Enables real-time monitoring and performance tracking.

## 📚 Setup & Usage

1. Clone this repository.
2. Install required Python packages:

```bash
pip install yfinance ta gspread oauth2client scikit-learn pandas matplotlib
