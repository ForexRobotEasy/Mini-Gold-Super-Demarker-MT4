# Mini Gold Super Demarker MT4

This code is a sample implementation of the Mini Gold Super Demarker trading strategy in MQL5. It uses three indicators - Moving Average, Force Index, and DeMarker - to identify overbought and oversold conditions in the market and execute trades accordingly.

## How it Works

1. The code starts by including the necessary libraries and indicators.

2. It defines input parameters for customizing the strategy:
   - `maPeriod`: Moving average period.
   - `forceIndexPeriod`: Force index period.
   - `demarkerPeriod`: DeMarker period.
   - `thresholdLevel`: Threshold level for overbought and oversold conditions.

3. Global variables are defined:
   - `lots`: Initial trade size.
   - `totalProfit`: Total profit.
   - `martingaleEnabled`: Enable/disable martingale technique.

4. The code initializes the indicators:
   - `ma`: Moving Average indicator.
   - `forceIndex`: Force Index indicator.
   - `demarker`: DeMarker indicator.

5. The custom `OnInit` function is called during initialization. It initializes the Moving Average, Force Index, and DeMarker indicators.

6. The custom `OnStart` function is called to start the strategy. It calculates the values of the indicators and checks for overbought and oversold conditions. Based on these conditions, it executes buy or sell orders.

7. The custom `OpenSellOrder` function is called to open a sell order. It defines the stop loss and take profit levels, and sends the order using the `OrderSend` function. If the order is successful, it updates the total profit and adjusts the trade size for martingale technique.

8. The custom `OpenBuyOrder` function is called to open a buy order. It defines the stop loss and take profit levels, and sends the order using the `OrderSend` function. If the order is successful, it updates the total profit and adjusts the trade size for martingale technique.

9. The custom `OnTrade` function is called to handle trade closure. If there are no open orders, it prints the total profit.

## Product Description

This code is a sample implementation of the Mini Gold Super Demarker trading strategy. It uses Moving Average, Force Index, and DeMarker indicators to identify overbought and oversold conditions in the market and execute trades accordingly.

Please note that ForexRobotEasy is not the official developer of this product. We only provide the sample code that can work as described in this product. For detailed reviews and trading results of this product, please visit [Forex Robot Easy](https://forexroboteasy.com/forex-robot-review/mini-gold-super-demarker-mt4-risky-forex-strategy-review/). To find the official developer of this product, please use MQL5.

For more information and to access the official version of this product, please visit [ForexRobotEasy](https://forexroboteasy.com/).
