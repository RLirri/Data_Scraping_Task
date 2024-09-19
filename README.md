# Week2 - Task about Data Scraping

## Overview
This tasks of data scraping involves developing a potential final project titled **GAN-Enhanced Quantitative Trading Strategy**. The core objective is to gather high-quality financial data, apply advanced technical indicators, and leverage **Generative Adversarial Networks (GANs)** to predict stock market trends. The data collection process utilizes the Yahoo Finance API via the `yfinance` Python library to fetch both stock summary information and historical data, which are essential for building the trading model.

## Features

### 1. Data Collection:
The project uses **Yahoo Finance API** (`yfinance`) to scrape real-time stock summary data and historical price data for multiple stock symbols. The data collected includes:
- **Stock Ticker**
- **Current Price**
- **Previous Close**
- **Open Price**
- **52 Week Range**
- **Market Cap**
- **Volume**

Additionally, historical OHLCV (Open, High, Low, Close, Volume) data is gathered for use in model training.

### 2. Technical Indicators:
Calculate key technical indicators such as:
- **Simple Moving Average (SMA)**
- **Exponential Moving Average (EMA)**

These indicators are essential for quantitative trading strategies and provide features to be used in the GAN model for trend prediction.

### 3. Multi-threading:
To efficiently fetch data for multiple stock symbols, the program uses **multi-threading**. This allows concurrent fetching of stock data, improving performance and reducing execution time.

### 4. Error Handling & Logging:
The project incorporates error handling with extensive logging to monitor the scraping process, ensuring smooth execution. Each stage of the process (from fetching data to saving files) is tracked for possible errors and issues.

## Task Project Structure

### Files:
- **stock_summary.csv**: A CSV file containing real-time stock summary data for selected symbols.
- **symbol_historical_data.csv**: Historical OHLCV data for each stock symbol, with technical indicators like SMA and EMA added.
- **main.py**: The main Python script that performs data scraping, calculates indicators, and saves data.
- **README.md**: This file provides an overview of the project and instructions on how to use the code.


## How to Use

### Prerequisites:
1. **Python 3.x** is required to run the scripts.
2. Install the necessary dependencies:
   ```bash
   pip install yfinance pandas
