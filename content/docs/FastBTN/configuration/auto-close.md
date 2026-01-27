---
date: '2025-12-27T04:47:09Z'
draft: true
title: 'Auto Close When Target Reached'
weight: 8
---

## Overview
{{< callout type="warning" >}}
Auto Close features depend on MetaTrader 5 running continuously. Any missed execution due to platform downtime is the user’s responsibility.
{{< /callout >}}

Auto Close works in the background while FastBTN is running. This feature will close all positions on the current pair or on all pairs when the total profit target you set is reached. It helps to gain profits without you needing to monitor the chart constantly. When enabled, FastBTN continuously checks your open positions.

Please consider your positions' Take Profit (TP) when using this feature, as the TP may not be reached. For example, if you have 5 open positions on XAU/USD, each with a TP of $10, and you use the *Auto Close When Target Reached* feature and set the *Target Profit* for the current pair to $100, then the $100 will never be reached because your positions' TP will limit your total profit to $50.

Likewise, if you set the *Target Profit* for the current pair to $25, your positions' TP of $50 (5 positions × $10 each) will never be reached because as soon as the total XAU/USD profit reaches $25, all XAU/USD positions will be closed.

Therefore, it's better not to use this feature when you want to set TP for each position, and vice versa.

Only Target **Profit** is supported; Target Loss is not supported.

{{< callout >}}
  **Important! Please Read**\
  When you have many open positions and the target you set is reached, you may not see the total profit being exactly the same as the target you set. This is due to the fast price movement in forex.

For example, if you set a total profit target of $100 for XAU/USD and you have 10 open XAU/USD positions, when the total profit reaches $100 and FastBTN closes all 10 positions, FastBTN will close them one by one.

Depending on the server and internet speed, there will be delays between closing each position, and the price may move up or down during these delays. So you may end up with more or less than $100.
{{< /callout >}}

---

## Requirement
Auto Close works **only while MetaTrader 5 is open and running**. This means:
- MT5 must remain open
- FastBTN must stay attached to the chart
- AutoTrading must remain enabled

If MetaTrader 5 is closed, minimized incorrectly, or your computer is turned off, **Auto Close will not function**. If you cannot keep your computer running at all times, you can use a **Virtual Private Server (VPS)** that allows:
- MetaTrader 5 to run 24/7
- Auto Close to work continuously

---

## Auto Close Current Pair
This will close all positions on the current pair when the target you set for the current pair is reached.

Example:\
On XAU/USD, you set:
- `Enable auto-close on current pair` = `true`
- `Target profit` = 100

Then, no matter how many open Buy and Sell positions you have on XAU/USD, when the combined total XAU/USD profit reaches $100, all of those open positions will be closed.

---

## Auto Close All Pairs
This will close all positions on **all pairs** when the target you set for all pairs is reached.

Please set this feature on only one pair. If you set this feature on more than one pair, they may contradict each other. For example, if you set this to $100 on XAU/USD and $50 on BTC/USD, then whenever the total profit from all pairs reaches $50, all positions will be closed, and you will never reach $100.

---

## Interaction with Manual Actions
Auto Close works alongside manual trade management:
- You can still close trades manually using Close buttons
- Auto Close does not prevent manual intervention

This allows you to combine automation with full manual control.

---

## Important Notes
Because Auto Close can close trades automatically:
- Only Target Profit is supported, **Target Loss is not supported**.
- Make sure the target profit value is set correctly
- Test Auto Close behavior on a demo account first

Incorrect Auto Close settings may result in trades closing earlier than expected.