- percentages stop loss with input to set %

    https://kodify.net/tradingview/orders/percentage-stop/
    longLossPerc = input(title="Long Stop Loss (%)",type=input.float, minval=0.0, step=0.1, defval=1) * 0.01
    longStopPrice  = strategy.position_avg_price * (1 - longLossPerc)

- trailing stoploss
    stop loss från vart den har peakat
    https://kodify.net/tradingview/orders/percentage-trail/
    longTrailPerc = input(title="Trail Long Loss (%)",type=input.float, minval=0.0, step=0.1, defval=3) * 0.01

        // Determine trail stop loss prices
    longStopPrice = 0.0

    longStopPrice := if (strategy.position_size > 0)
        stopValue = close * (1 - longTrailPerc)
        max(stopValue, longStopPrice[1])
    else
        0
