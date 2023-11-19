# Undefeated Triangle MT4 - ReadMe

This code represents the Undefeated Triangle MT4 forex trading system developed by the Forex Robot Easy Team. It is an advanced forex trading system that aims to generate profits by trading on the AUDCAD, AUDNZD, and NZDCAD currency pairs.

## Developer's Site

For detailed reviews and trading results of this product, please visit [forexroboteasy.com](https://forexroboteasy.com/forex-robot-review/undefeated-triangle-mt4-review-advanced-forex-trading-system/). Please note that ForexRobotEasy is not the official developer of this product. We only provide this sample code that demonstrates how the product can work as described. To find the official developer of this product, please use MQL5.

## Program Description

The Undefeated Triangle MT4 trading system is an expert advisor (EA) designed to run on the MetaTrader 4 platform. It utilizes a grid trading strategy to open and manage orders on the AUDCAD, AUDNZD, and NZDCAD currency pairs.

### Input Parameters

The following input parameters can be adjusted to customize the trading system:

- LotSize: The size of each trading lot (default: 0.01)
- TakeProfit: The desired take profit level in pips (default: 100.0)
- StopLoss: The desired stop loss level in pips (default: 50.0)
- MaxOrders: The maximum number of orders allowed to be opened at a time (default: 10)

### Initialization

Upon initialization, the trading system is initialized and ready to start trading.

### OnTick()

This function is executed on every tick of the market. It performs the following actions:

1. Checks for existing orders.
2. Closes orders that have reached the take profit level or the stop loss level.
3. Opens new orders if the maximum number of orders has not been reached and there is sufficient balance.

### Closing Orders

Existing orders are closed based on their type (buy or sell) and their profit/loss level. If an order has reached the take profit level, it is closed at the current market bid/ask price. If an order has reached the stop loss level, it is closed at the current market bid/ask price.

### Opening Orders

New orders are opened on the AUDCAD, AUDNZD, and NZDCAD currency pairs. The grid levels for opening these orders are calculated based on the take profit and stop loss levels. The opening prices for the orders are determined by adding/subtracting the grid level from the current market bid/ask price.

### OnDeinit()

This function is executed when the trading system is deinitialized.

## Disclaimer

Please note that this code is a sample provided by ForexRobotEasy and may not be the exact code used in the official Undefeated Triangle MT4 trading system. To obtain the official code and access the complete functionality of the product, please visit the developer's site mentioned above.
