# Small to Big EA MT5

## Overview
The Small to Big EA MT5 is a powerful forex tool developed by Forex Robot Easy Team. This Expert Advisor (EA) is designed to execute trades based on trend analysis. It opens buy and sell orders with specified lot sizes, take profit levels, and stop loss levels. The EA can be customized with input parameters to suit individual trading preferences.

## Features
- Trend-based trading strategy
- Customizable lot size, take profit, and stop loss levels
- Automatic buy and sell order execution
- Real-time account balance, equity, and profit monitoring
- Enable/disable trading option

## Input Parameters
- **LotSize**: Specifies the lot size for each trade. Default is 0.01.
- **TakeProfit**: Sets the take profit level in pips. Default is 50.
- **StopLoss**: Defines the stop loss level in pips. Default is 30.

## How It Works
1. The EA initializes and retrieves the initial account balance, equity, and profit.
2. Trading is enabled by default.
3. On each tick, the EA checks if trading is enabled. If not, it exits the function.
4. The EA then checks for a trend using the *CheckTrend()* function.
5. If a trend is detected, the EA opens a buy order and a sell order simultaneously.
6. The buy order is opened at the current ask price with stop loss and take profit levels calculated based on the input parameters.
7. The sell order is opened at the current bid price with corresponding stop loss and take profit levels.
8. The EA prints the status of the order opening process, indicating success or any error encountered.

## Custom Functions
- **OnInit()**: Custom initialization function that retrieves the initial account balance, equity, and profit. It also enables trading.
- **OnDeinit(const int reason)**: Custom deinitialization function that disables trading when the EA is stopped or removed.
- **OnTick()**: Custom trading function that executes trades based on trend analysis. It checks if trading is enabled, then opens buy and sell orders according to the trend.
- **CheckTrend()**: Custom trend checking function that implements the trend analysis logic. This function should be customized based on individual trading strategies.

## Product Description
The Small to Big EA MT5 is a powerful forex tool developed by Forex Robot Easy Team. This Expert Advisor (EA) uses a trend-based trading strategy to execute buy and sell orders automatically. With customizable input parameters such as lot size, take profit, and stop loss levels, traders can tailor the EA to their specific trading preferences.

By analyzing market trends, the Small to Big EA MT5 identifies potential trading opportunities and opens buy and sell orders accordingly. This allows traders to take advantage of market movements and potentially maximize profits. The EA also provides real-time monitoring of account balance, equity, and profit, giving traders valuable insights into their trading performance.

Please note that ForexRobotEasy is not the official developer of this product. We only provide a sample code that demonstrates how the EA can work as described. To find the official developer of this product, please refer to MQL5.

For detailed reviews and trading results of this product, visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/small-to-big-ea-mt5-review-powerful-forex-tool-at-launch-price/).
