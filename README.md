# CopyMaster mt5

This code is a sample implementation of the CopyMaster mt5 software, developed by the Forex Robot Easy Team. It provides trade copying functionality between two MetaTrader 5 terminals, allowing users to replicate trades from a master terminal to a slave terminal.

## Trade Copying Function

The `TradeCopying` function establishes a connection between the master and slave terminals using the `ConnectTerminals` function. It then retrieves trades from the master terminal using the `GetTrades` function and replicates them to the slave terminal if the trade is successful (profitable).

## Customizable Copying Options Function

The `CustomizableCopyingOptions` function allows users to customize various parameters for the trade copying process. It takes in an array of currency pairs, an order size, and a maximum drawdown value. It selects the specified currency pairs for copying using the `SelectCurrencyPairs` function, sets the order size using the `SetOrderSize` function, and limits losses using the specified maximum drawdown value with the `LimitLosses` function. Additionally, it enables the option to copy only profitable trades using the `CopyOnlyProfitableTrades` function.

## Main Function

The `OnStart` function is the main entry point of the code. It demonstrates the usage of the CopyMaster mt5 software by calling the `TradeCopying` function with the names of the master and slave terminals. It then sets up customizable copying options by specifying currency pairs, order size, and maximum drawdown values and calling the `CustomizableCopyingOptions` function.

For detailed reviews and trading results of the official CopyMaster mt5 product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/copymaster-mt5-review-and-download-the-ultimate-forex-software-for-copying-trades/). Note that ForexRobotEasy is not the official developer of this product and only provides a sample code that can work as described in the product. To find the official developer of this product, please refer to MQL5.
