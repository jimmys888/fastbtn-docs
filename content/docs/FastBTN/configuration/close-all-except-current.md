---
draft: true
title: 'Close All Pairs Except Current Pair'
weight: 9
---

## Overview
{{< callout type="error" >}}
  **Warning**\
  Please be extra careful when using this button as the action will be executed immediately without any confirmation!
{{< /callout >}}

The **Close All Except Current** button will quickly close positions on **all other pairs**, while keeping all positions on the **current pair** untouched. This is a fast way to reduce exposure across your account while keeping your focus symbol running.

For example, if you are currently on **XAU/USD** and you trigger this feature:
- All open positions on other pairs (EUR/USD, GBP/USD, BTC/USD, etc.) will be closed immediately
- All open positions on **XAUUSD** will remain open

You may not need this button at all or rarely need it. I find it useful when for example I have a couple of profitable Buy positions on XAU/USD and other losing positions on other pair. I can see that the total profit on XAU/USD already exceeds total loss of all other pairs, and I believe that XAU/USD is still bullish. So I want to keep my XAU/USD positions and close all other positions on other pairs. This button does just this.

---

## Enable / Disable Button
When you disable it by setting the **Enable Button?** option to `false`, the button will disappear from the chart.

---

## Put in its own row?
If you set this option to `true`, then this button will be placed below [Lock Profit](/docs/configuration/lock-profit.md) button, like this:
![](/images/close-all-except-current-01.png)

If you set this option to `false`, then this button will be placed at the right of the *Lock Profit* button, like this:
![](/images/close-all-except-current-02.png)

---

## Other Button's Properties
For more information about the button's text, color, font etc, please refer to [Button Appearance](/docs/configuration/buttons-appearance.md).

{{< callout type="info" >}}
  **Tips**\
  To show current pair on the button's text, use 4 dollar signs ($$$$). For example, if on XAU/USD you enter ***Close All Except $$$$*** then it will show as ***Close All Except XAUUSD***.

  This is useful when you save *FastBTN* settings and load it on another pair, it will automatically show that pair's symbol so you don't have to enter the symbol manually on each pair.
{{< /callout >}}

---

## Important Notes
- This feature affects **multiple symbols**, not only the current symbol
- It will close both Buy and Sell positions on other symbols
- Always confirm you are on the correct chart symbol before using it
- Execution depends on broker conditions (spread, slippage, market speed)
- Test the behavior on a demo account first

Once positions are closed, the action cannot be undone.