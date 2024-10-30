# Algorithmic Intraday Trading in Cryptocurrencies:  a Machine Learning Framework for Breakout Strategy Optimization

——

Mantegh Sethi, Anita Xu, Kelvin Ampene

——

Submitted in partial fulfilment of the degree of Master of Science

WorldQuant University, LA, USA.

——

Email:
manteghsethi@outlook.com,
anitaxuzx@live.co.uk, 
ampenekelvin@gmail.com 

This project uses various Python libraries for data analysis, financial indicators, and machine learning. The following instructions will guide you through setting up the environment and installing dependencies.

## Prerequisites

This project uses Python 3.10. Make sure you have Python and `pip` installed. You can check your Python and pip versions by running:

```bash
python3 --version
pip --version
```

### Step 1: Install requirements
```bash
pip install -r requirements.txt
```

### Step 2.1: Download and extract TA-Lib dependencies for Linux
```bash
url_libta="https://anaconda.org/conda-forge/libta-lib/0.4.0/download/linux-64/libta-lib-0.4.0-h166bdaf_1.tar.bz2"
curl -L $url_libta | tar xj -C /usr/lib/x86_64-linux-gnu/ lib --strip-components=1
```

### Step 2.2: Install TA-Lib Python Package for Linux
```bash
url_ta="https://anaconda.org/conda-forge/ta-lib/0.4.19/download/linux-64/ta-lib-0.4.19-py310hde88566_4.tar.bz2"
curl -L $url_ta | tar xj -C /usr/local/lib/python3.10/dist-packages/ lib/python3.10/site-packages/talib --strip-components=3
```

### Step 2.1: Install TA-Lib using Homebrew for macOS
```bash
brew install ta-lib
```

### Step 2.2: Install the TA-Lib Python package for macOS
```bash
pip install ta-lib
```

### Step 3: Verify installation of packages
```bash
import talib
import pandas as pd
import matplotlib.pyplot as plt
import yfinance as yf
```

## Project Structure

# Intraday Cryptocurrency Trading Using Machine Learning

This project explores an automated intraday trading strategy for Bitcoin and Ethereum using machine learning models. It leverages advanced trading indicators and market sentiment to predict and act on price movements. Here’s an overview of how it works.

---

## 1. Data Collection and Processing

- **Data Sources**: Bitcoin and Ethereum data are collected at different time intervals (1, 5, 15, 30, and 120 minutes) to capture short-term price fluctuations.
- **Data Handling**: The data is cleaned, scaled, and transformed for consistency, focusing on key indicators like price, volume, and date.

---

## 2. Technical Indicators

Technical indicators are used to identify price trends and signals:
- **Moving Average Convergence Divergence (MACD)**: Highlights momentum by comparing different moving averages.
- **Relative Strength Index (RSI)**: Measures the speed and change of price movements to detect overbought or oversold conditions.
- **Money Flow Index (MFI)**: Combines price and volume data to gauge buying and selling pressure.

---

## 3. Sentiment Analysis

Sentiment from social media and market sentiment data, like the Crypto Fear and Greed Index, is integrated. This helps capture emotional trends, which often influence cryptocurrency markets.

---

## 4. Model Architecture

Three advanced machine learning models analyze price data:
- **CNN-LSTM**: Combines pattern recognition (CNN) and sequence prediction (LSTM) to understand both short- and long-term trends.
- **Bidirectional LSTM**: Looks at past and future data to make more robust predictions.
- **Encoder-Decoder LSTM**: Useful for multi-step forecasting, predicting price changes over longer periods.

---

## 5. Back-Testing and Results

The model's performance is tested on historical data to validate its profitability:
- **Back-testing**: Tests how well the models would have performed historically, highlighting potential profitability.
- **Results**: The strategy shows profitability in specific market conditions, although tuning is needed for varying conditions.

---

## 6. Conclusion

This project demonstrates the potential for machine learning in cryptocurrency trading. By combining technical indicators and sentiment data, it aims to predict and capitalize on intraday price movements. With continued tuning, the model offers a foundation for real-time trading in a volatile market.

---

This guide provides an overview of how the system collects, processes, and uses data to make informed trading decisions. Although complex behind the scenes, the approach is straightforward: blend market signals with sentiment for better timing and execution.









