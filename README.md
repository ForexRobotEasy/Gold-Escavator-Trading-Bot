# Gold Escavator Trading Bot

This code is a sample of a trading bot developed by Forex Robot Easy Team. The bot is designed to trade the GBPUSD currency pair based on predefined trading criteria. 

## How it Works

The trading bot uses the MetaTrader 4 platform and the MQL4 programming language. It includes necessary libraries and defines constants for the trading parameters. 

The `CalculateLotSize` function is used to calculate the lot size based on the risk percentage defined by the user. It takes into account the account balance, equity, margin, and free margin to determine the maximum lot size and the available lot size.

The `IsTradingHour` function checks if the current hour is within the specified trading hours. This helps to ensure that trades are only executed during the desired time frame.

The `BuyTrade` and `SellTrade` functions are used to execute buy and sell trades respectively. They calculate the lot size, entry price, stop loss, and take profit levels based on the predefined parameters. If the trade is executed successfully, a text object is created on the chart to indicate the entry type (buy or sell).

The `OnInit` function initializes the trading bot by creating a timeseries object and setting the expert magic number.

The `OnTick` function is called on each tick of the price. It checks if the current hour is within the trading hours and not the same as the last trade hour. If these conditions are met, it checks for buy or sell signals based on the RSI indicator. If a signal is detected, the corresponding trade function is called.

The `OnDeinit` function is called when the trading bot is removed from the chart. It cleans up any resources used by the bot.

## Product Description

Gold Escavator Trading Bot is an automated trading system developed by Forex Robot Easy Team. It is designed to trade the GBPUSD currency pair using a predefined set of trading criteria. The bot aims to generate profits by taking advantage of market trends and fluctuations.

Key Features:
- Trades the GBPUSD currency pair
- Uses the RSI indicator for buy and sell signals
- Implements a risk management strategy based on account balance and equity
- Automatically adjusts stop loss and take profit levels for open trades
- Works within specified trading hours

Please note that Forex Robot Easy is not the official developer of this product. We are only providing a sample code that can work as described in the product. For detailed reviews and trading results, please visit the official developer's website [here](https://forexroboteasy.com/forex-robot-review/gold-escavator-bot-review-65-roi-on-gbpusd-forex-trading/). To find the official developer of this product, please use the MQL5 platform.
