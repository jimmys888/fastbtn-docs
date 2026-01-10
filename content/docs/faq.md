---
date: '2025-12-27T04:34:53Z'
draft: true
title: 'FAQ'
weight: 97
---

## FAQ – FastBTN

### What is FastBTN?

FastBTN is a **button-based trading Expert Advisor for MetaTrader 5**.  
It allows you to open, manage, and close trades quickly using on-chart buttons, with optional automation features such as Auto TP/SL, Auto Close, and Lock Profit.

It is designed to make trading **faster, safer, and more consistent**.

---

### Does FastBTN work on MetaTrader 4 (MT4)?
No.  
FastBTN is designed **exclusively for MetaTrader 5 (MT5)** and will not work on MT4.

---

### Is FastBTN fully automated?
No.  
FastBTN is primarily a **manual trade management tool** with optional automation features.

You remain in control of:
- When trades are opened
- When trades are closed
- Which features are enabled

Automation features are optional and configurable.

---

### Can FastBTN open trades automatically by itself?
No. 
FastBTN opens trades only when:
- You click a button
- You use a keyboard shortcut

It does **not** open strategy-based or random trades on its own.

---

### Does FastBTN manage trades on all symbols?

FastBTN operates on the **current chart symbol** by default.

Some features (such as **Close All in Profit / Close All Except Current Pair**) intentionally affect **other symbols**, and this behavior is clearly explained in the documentation.

---

### Does FastBTN features also work on pending orders?
No.

FastBTN only works on open positions.

---

### Can I use FastBTN on multiple charts at the same time?

Yes.

You can attach FastBTN to multiple charts, for example:
- Different symbols
- Different strategies
- Different Magic Numbers

Using unique Magic Numbers is recommended in this case.

---

### Does Auto Close work if MT5 is closed?

No.

Auto Close and other automated features work **only while MetaTrader 5 is running**.

If MT5 is closed or your computer is turned off, automated features will not function.  
If you need 24/7 operation, using a **VPS (Virtual Private Server)** is strongly recommended.

---

### Can I save my FastBTN settings?

Yes.

FastBTN supports:
- Saving settings using `.set` files
- Combining everything into a **chart template**
- Loading complete setups in one click

This makes it easy to reuse your preferred configurations.

---

### Is FastBTN safe to use on a live account?
Yes.

However, as with any trading tool:
- Always test on a **demo account first**
- Understand each feature before enabling it
- Use proper risk management

---

### Does FastBTN guarantee profits?

No.

FastBTN is a **trading tool**, not a trading strategy.  
It helps with execution and trade management, but **profits are never guaranteed**.

Your results depend on:
- Market conditions
- Your trading strategy
- Risk management
- Broker execution

---

## FAQ – FastSTAT

### What is FastSTAT?

FastSTAT is a **trading statistics indicator for MetaTrader 5**.

It displays useful information directly on the chart, such as:
- Current profit or loss
- Volume of open positions
- Buy and Sell position summary
- Symbol-specific trading data

FastSTAT is designed to provide **clear visibility**, not trade execution.

---

### Is FastSTAT free?

Yes.  
**FastSTAT is completely free**.

You can use it without purchasing or using FastBTN.

---

### Can I use FastSTAT without FastBTN?

Yes.

FastSTAT can be used **independently** and works even if FastBTN is not installed.  
It will display statistics for your manual trades or trades opened by other EAs.

---

### Does FastSTAT open or close trades?

No.

FastSTAT is **informational only**.  
It does not:
- Open trades
- Close trades
- Modify positions

It only displays trading statistics on the chart.

---

### Does FastSTAT work on MetaTrader 4 (MT4)?

No.  
FastSTAT is designed **exclusively for MetaTrader 5 (MT5)**.

---

### Can I customize FastSTAT?

Yes.

FastSTAT allows you to customize:
- Which statistics are displayed
- Text size and colors
- Panel position on the chart

All settings can be saved and reused using standard MT5 methods.

---

### Does FastSTAT require MT5 to be running?

Yes.

Like all MT5 indicators, FastSTAT works only while MetaTrader 5 is open and running.  
If MT5 is closed, FastSTAT will not update or display data.
