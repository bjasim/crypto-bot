# Binance Trading Bot README

## Description

This Python script is a simple Binance trading bot that monitors the RSI (Relative Strength Index) of the ETH/USDT trading pair and executes buy/sell orders based on RSI signals. It uses the Binance WebSocket API for real-time data and the TA-Lib library for RSI calculation.

## Features

- Monitors the ETH/USDT trading pair on Binance.
- Calculates RSI (Relative Strength Index) based on historical candlestick data.
- Executes buy orders when RSI is below a certain threshold (oversold).
- Executes sell orders when RSI is above a certain threshold (overbought).

## Requirements

To run this script, you need:

- Python 3.x installed on your system.
- Binance API Key and Secret obtained from your Binance account.
- TA-Lib library installed (`pip install TA-Lib`).

## Installation

1. Clone or download this repository to your local machine.


## Configuration

1. Open the `config.py` file and replace `API_KEY` and `API_SECRET` with your Binance API Key and Secret.

```python
API_KEY = "your_api_key"
API_SECRET = "your_api_secret"
```

Configure other parameters in the script such as RSI thresholds, trade symbol, and quantity.
```python
RSI_PERIOD = 14
RSI_OVERBOUGHT = 70
RSI_OVERSOLD = 30
TRADE_SYMBOL = 'ETHUSDT'
TRADE_QUANTITY = 0.05
```

## Usage
Run the Python script in your terminal or preferred Python environment.
```
python binance_trading_bot.py
```
The script will connect to the Binance WebSocket API and start monitoring the ETH/USDT trading pair.

## Implementation
The script uses the Binance WebSocket API to receive real-time candlestick data.
It calculates the RSI (Relative Strength Index) using TA-Lib library.
Based on RSI signals, it executes buy and sell orders using Binance API.
All configuration parameters can be customized in the config.py file.

