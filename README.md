BuySell Strategy 5min

📈 General Idea:
Works on a 5-minute chart.

It buys when the price is low and starting to strengthen based on EMA, midpoint of yesterday’s range, and positive RSI momentum.

It sells when a profit target, stop loss, or certain dynamic conditions are met.

⚙️ Key Inputs:
EMA Period: 30

RSI Period: 14

RSI Threshold for change: 10%

Take Profit: +20% from buy price

Stop Loss: -7% from buy price

🛒 Buy Conditions:
Not already in a trade (in_position == false).

Price is below or at the EMA.

Price is below the midpoint of yesterday’s high/low or cheaper than last buy price.

Yesterday's range is wide enough (≥ 7% move).

RSI is increasing strongly (change ≥ RSI threshold).

✅ When all these are true → BUY full equity at current price.

💵 Sell Conditions:
Stop Loss: Price drops 7% below buy price.

Take Profit: Price rises 20% above buy price.

Dynamic Sell:

Price moves above EMA.

And price is above midpoint or higher than last buy price.

And RSI is increasing strongly.

✅ In all cases → Sell everything.

🛠️ Other Details:
Tracks yesterday's high/low and today's high/low separately.

Uses a fixed position size based on total equity.

Draws labels on the chart for buys, sells, stop losses, and dynamic sells.

Plots the EMA on the chart (yellow line).

Charges a 0.1% commission per trade.
