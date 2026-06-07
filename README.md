Deriv Trading Bot

Automated trading bot designed for the Deriv platform, built to identify trading opportunities, manage risk, and execute trades based on predefined strategy rules.

Overview

This bot automates the trading process by:

Monitoring market conditions in real time
Identifying valid trade setups
Executing trades automatically
Managing risk through stop-loss and take-profit rules
Logging trade activity for performance review
Features

✅ Automated trade execution

✅ Real-time market analysis

✅ Risk management controls

✅ Trade logging and reporting

✅ Customizable trading parameters

✅ Fast execution through Deriv API

Trading Strategy

The bot uses the following strategy:

Detects market structure changes.
Identifies liquidity sweeps.
Waits for confirmation through an Inverse Fair Value Gap (IFVG).
Enters trades in the direction of the anticipated move.
Targets buy-side or sell-side liquidity.
Applies predefined risk management rules.

Note: Past performance does not guarantee future results. Always test strategies on a demo account before using real funds.

Requirements
Python 3.10+
Deriv API Token
Internet connection
Python Libraries
pip install websocket-client
pip install pandas
pip install numpy
pip install requests

Or:

pip install -r requirements.txt
Installation

Clone the repository:

git clone https://sanjaeduncan03-art/deriv-trading-bot.git

Navigate to the project folder:

cd deriv-trading-bot

Install dependencies:

pip install -r requirements.txt
Configuration

Create a configuration file:

API_TOKEN=your_deriv_api_token
APP_ID=your_app_id
ACCOUNT_TYPE=demo
RISK_PERCENT=1
TRADE_AMOUNT=10
Parameters
Parameter	Description
API_TOKEN	Deriv API token
APP_ID	Deriv application ID
ACCOUNT_TYPE	Demo or Real
RISK_PERCENT	Percentage risk per trade
TRADE_AMOUNT	Fixed stake amount
Running the Bot

Start the bot:

python main.py

Expected output:

Connecting to Deriv...
Connection established.
Monitoring market...
Trade signal detected.
Executing trade...
Project Structure
deriv-trading-bot/
│
├── main.py
├── strategy.py
├── risk_manager.py
├── deriv_api.py
├── logger.py
├── config.py
├── requirements.txt
└── README.md
Risk Management

The bot includes:

Maximum daily loss limit
Fixed percentage risk per trade
Consecutive loss protection
Position sizing controls

Example:

risk_per_trade = account_balance * 0.01
Logging

Trade activity is stored for analysis:

logs/
├── trades.log
├── errors.log
└── performance.log

Information logged includes:

Entry price
Exit price
Profit/Loss
Timestamp
Signal type
Backtesting

Before live trading:

Test on a demo account.
Review historical performance.
Optimize parameters.
Validate risk settings.
Disclaimer

This software is provided for educational and research purposes only. Trading financial markets carries significant risk and may result in loss of capital. Users are responsible for their own trading decisions and use this software at their own risk.

Contributing

Contributions are welcome.

Fork the repository
Create a feature branch
Commit your changes
Submit a pull request
License

MFT License

Copyright (c) 2026

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the software, subject to the conditions of the MIT License.

Author: NAKI MF
Platform: Deriv
Version: 1.0.0
Status: Development / Testing / Production (choose one)
