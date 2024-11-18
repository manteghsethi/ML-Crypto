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









