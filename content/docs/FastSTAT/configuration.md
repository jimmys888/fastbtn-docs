---
date: '2025-12-27T04:35:26Z'
draft: true
title: 'FastSTAT Configuration'
linkTitle: 'Configuration'
weight: 3
---

## Configuration

{{< cards >}}
{{< card title="FastSTAT General Settings" image="/images/faststat-01.png" >}}
{{< /cards >}}

### Indicator Position
You can choose one of the four chart corners to place *FastStat*. Personally, I like to place it at the *Right lower chart corner*, combined with *FastBTN* like this:
<a href="/images/faststat-02.png" target="_blank"><img src="/images/faststat-02.png" /></a>

<br>

### Neutral Color, Profit Color, and Loss Color
- Neutral Color (default: `Black`) is used for zero (0) values.
- Profit Color (default: `Blue`) is used for positive values (profit).
- Loss Color (default: `Red`) is used for negative values (loss).
![](/images/faststat-04.png)

---

### Distance
**X Distance**\
If you set the indicator position to *Right lower chart corner* or *Right upper chart corner*, this value represents the distance between **the right edge of the indicator and the right edge of the chart**.

If you set the indicator position to *Left lower chart corner* or *Left upper chart corner*, this value represents the distance between **the left edge of the indicator and the left edge of the chart**.

**Y Distance**\
If you set the indicator position to *Right lower chart corner* or *Left lower chart corner*, this value represents the distance between **the bottom of the indicator and the bottom of the chart**.

If you set the indicator position to *Right upper chart corner* or *Left upper chart corner*, this value represents the distance between **the top of the indicator and the top of the chart**.
![](/images/faststat-05a.png)

For example, in the image below, I set the indicator position to *Right lower chart corner* and set the X Distance to 75 and Y Distance to 50.
![](/images/faststat-05.png)

---

### Font Size and Font Family
Just like in *FastBTN*, you can change the font size and font family. Make sure you have the font family installed on your computer.

---

## Current Pair & Total (All Pairs)
There are 13 pieces of information that you can display on your chart, and you can choose which ones to show or hide.
![](/images/faststat-06.jpg)

Numbers 1 to 8 are for the **current pair** only, numbers 9 to 12 are for **all pairs**:
1. **Show Symbol**\
   Set this to `true` if you want to display the chart's symbol. This is useful for easily identifying which pair you're viewing when you have many charts open.
2. **Show Price**\
   Displays the current pair's price. If you're like me, I don't show MT5's quick trading buttons on the chart anymore since I already use *FastBTN*, and looking at the price on the right of chart hurts my eyes, then this is very useful. You can choose which price to show:
   ![](/images/faststat-06a.png)
   - Close price
   - Bid price
   - Ask price
   - Bid & Ask price *(default)*. It will shown in this format: **Bid_Price | Ask_Price** like this:
   ![](/images/faststat-06b.png)
3. **Show Profit in Pips**\
   Displays total profit or loss in pips for the current pair.
   {{< callout type="warning" >}}
   This shows the sum of pips per position, not lot-weighted pips. If you have mixed volumes, it may seem "off" or inconsistent compared to profit/loss in money.
   {{< /callout >}}
4. **Show Profit in Currency**\
   Displays total profit or loss in money amount for the current pair.
5. **Show Volume**\
   Displays total volume opened for the current pair.
6. **Show Spread**\
   Displays the spread for the current pair.
7. **Show Time to Bar Closure**\
   Shows how long until the next bar/candlestick appears.
8. **Server Time**\
   Displays the server's current time.
9. **Title**\
   You can change what to display as the title, such as "Total" or "All", etc.
10. **Show Total Profit of All Open Positions**\
    Displays the total profit (or loss) in **money amount** for all open positions. No option to show this in pips is available.
11. **Show Profit & Loss of All Open Positions**\
    **These will only be shown if `Show total profit of all open positions` is set to `true`**.\
    It will display:\
    • The sum of profits in money amount from profitable positions on all pairs. It starts with **P:**\
    • The sum of losses in money amount from losing positions on all pairs. It starts with **L:**
12. **Show Total Volume of All Open Positions**\
     Displays total volume for all open positions on all pairs.

 ---

## Modify Appearance
### Use Labels
Except for items number 1, 10, and 11 (see the screenshot above), you can use a label for each item like this:
![](/images/faststat-07.png)

Leave an item's *label* property **blank** if you don't want to use it.

<br>

### Change Color
![](/images/faststat-08.png)
You can change each item's color except for items number 10 and 11 (see the screenshot above). Items 10 and 11 will use **[Neutral Color, Profit Color, and Loss Color](#neutral-color-profit-color-and-loss-color)**.

If you set an item's `Use profit / loss color` property to `true`, then that item will also use **Neutral Color, Profit Color, and Loss Color**.

---

## BEP Line
![](/images/faststat-09.png)

Setting *Show BEP Line* to `true` will display a line at the Break Even Price.

<br>

### Line Color for Buy
This is the color shown if:
1. You have Buy positions only.
2. You have mixed positions (Buy & Sell) where the number of Buy positions exceeds the number of Sell positions.

<br>

### Line Color for Sell
This is the color shown if:
1. You have Sell positions only.
2. You have mixed positions (Buy & Sell) where the number of Sell positions exceeds the number of Buy positions.

<br>

### Line Color for Neutral
This is the color shown if you have mixed positions (Buy & Sell) where the number of Buy positions is the same as the number of Sell positions.

<br>

### Line Style
There are 5 options for the line style:
![](/images/faststat-10.png)
![](/images/faststat-11.png)

<br>

### Line Thickness
The default value is 2. You can increase it to make the line thicker and more visible.

### BEP Line Blocking FastBTN
If the BEP Line appears in front of FastBTN like this:
<a href="/images/faststat-12.png" target="_blank"><img src="/images/faststat-12.png" /></a>

That means you loaded *FastStat* **after** *FastBTN*.

Simply remove *FastBTN* from your chart and then reload it. The last indicator loaded will appear in front of previously loaded ones.

---

## Refresh Behavior
FastSTAT updates automatically when:
- Price changes
- Positions are opened or closed
- Market conditions update

No manual refresh is required.

---

{{< callout type="info" >}}
FastSTAT has minimal performance impact and is safe to use on multiple charts.
{{< /callout >}}