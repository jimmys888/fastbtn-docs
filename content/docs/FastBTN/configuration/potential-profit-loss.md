---
date: '2025-12-27T04:48:06Z'
draft: true
title: 'Potential Profit & Loss'
weight: 12
next: /docs/fastbtn/shortcut-keys.md
---

When you have TP & SL set, you may want to see the potential TP and SL you may get:
- Potential TP: the amount of money you'll get if all positions that have TP hit the TP
- Potential SL: the amount of money you'll lose if all positions that have SL hit the SL
![](/images/potential-01.png)

To show this information on your chart, set `Show?` to `true`. You can choose on which corner you want it displayed. You can change the title, title color, background color, etc. Just play around with it.

It helps you quickly understand how much you could gain or lose based on your current settings and open positions.

---

## Show for All Pairs?
When you set `Show for All Pairs?` to `true`, then you will also see the total potential TP and total potential SL from all open positions that have TP and SL. Just like the example above.

If you set it to `false`, then you will only see the potential TP and potential SL from current pair.
![](/images/potential-02.png)

---

## Number of Positions
This shows the number of positions that have TP and SL. Take a look at this example:
![](/images/potential-03.png)

It shows:
- `TP: 3   SL: 3   Total: 3`\
  This means on current pair (BTC/USD), there are 3 total open positions, 3 of them (all) have TP and 3 of them (all) have SL.
- `TP: 6   SL: 5   Total: 7`\
  This means that on all pairs:
  - There are 7 total open positions
  - 6 of them have TP, 3 on current pair (BTC/USD), 3 on other pairs
  - 5 of them have SL, 3 on current pair (BTC/USD), 2 on other pairs
  - 1 position doesn't have TP, 2 positions don't have SL

{{< callout type="info" >}}
  **Tips**\
  To show current pair on the **Current Pair Title**, use 4 dollar signs ($$$$). For example, on BTC/USD chart, if you enter ***$$$$*** then it will show as ***BTCUSD***.

  This is useful when you save *FastBTN* settings and load it on another pair, it will automatically show that pair's symbol so you don't have to enter the symbol manually on each pair.
{{< /callout >}}

If you only have open positions on 1 pair, the info displayed for current pair and all pairs will be the same.
![](/images/potential-04.png)

---

## Important Notes
- Values are estimates, not guarantees
- Broker execution conditions can affect final results
- The feature does not place or close trades