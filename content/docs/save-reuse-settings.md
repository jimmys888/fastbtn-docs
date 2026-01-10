---
draft: true
title: "Saving & Reusing Settings"
weight: 7
---

## Overview

FastBTN (Expert Advisor) and FastSTAT (indicator) both offer many configurable options.  
To avoid setting everything up repeatedly, MetaTrader 5 (MT5) provides three powerful features:

1. **EA setting files (`.set`)**
2. **Indicator setting files (`.set`)**
3. **Chart templates (`.tpl`)**

When used together, you can load **FastBTN + FastSTAT with all settings applied in one click**.

This guide explains the recommended workflow step by step.

---

## Saving FastBTN (EA) Settings

FastBTN uses input parameters for:
- Lot size
- Button visibility
- Auto TP / SL
- Lock Profit / Hedging
- Auto-close rules
- And more

Once configured, these inputs can be saved for reuse.

### Save FastBTN Settings
1. Attach **FastBTN** to a chart.
2. Press **F7** (or right-click → *Expert List → Properties*).
3. Open the **Inputs** tab.
4. Adjust all FastBTN parameters as desired.
5. Click **Save…**
6. Name the file, for example:
   - `FastBTN_XAUUSD.set`
   - `FastBTN_Scalping.set`
7. Click **OK**

MT5 saves this as a `.set` file containing **only FastBTN’s inputs**.

### Load FastBTN Settings
1. Attach FastBTN to a chart.
2. Press **F7** (or right-click → *Expert List → Properties*).
3. Open **Inputs**.
4. Click **Load…**
5. Select the desired `.set` file.
6. Click **OK**

---

## Saving FastSTAT (Indicator) Settings

FastSTAT has its own configurable options such as:
- Displayed statistics
- Colors and fonts
- Panel position

These can also be saved separately.

### Save FastSTAT Settings
1. Attach **FastSTAT** to a chart.
2. Press **Ctrl + I** (Indicators List).
3. Select **FastSTAT** → **Properties**.
4. Adjust parameters, colors, and layout.
5. Click **Save…**
6. Name the file, for example:
   - `FastSTAT_Default.set`
   - `FastSTAT_Minimal.set`
7. Click **OK**

### Load FastSTAT Settings
1. Add FastSTAT to a chart.
2. In the settings window, click **Load…**
3. Select the saved `.set` file.
4. Click **OK**

---

## Creating a Full FastBTN + FastSTAT Template (Recommended)

Even with saved `.set` files, loading everything manually still takes time.

A **chart template** allows MT5 to load:
- FastBTN
- FastBTN settings
- FastSTAT
- FastSTAT settings
- Chart colors and layout  
**all at once**.

### Create a FastBTN + FastSTAT Template
1. Open a clean chart.
2. Attach **FastBTN**.
3. Load the desired **FastBTN `.set` file**.
4. Attach **FastSTAT**.
5. Load the desired **FastSTAT `.set` file**.
6. Adjust chart appearance (candles, grid, scale).
7. Right-click on the chart.
8. Select **Template → Save Template…**
9. Name it, for example:
   - `FastBTN_FastSTAT_Full.tpl`
10. Click **Save**

---

## Loading the Template (One-Click Setup)

To instantly recreate your full trading setup:

1. Open any chart.
2. Right-click on the chart.
3. Select **Template → Load Template**.
4. Choose your saved `.tpl` file.

MT5 will automatically:
- Load FastBTN
- Apply FastBTN settings
- Load FastSTAT
- Apply FastSTAT settings
- Restore the chart layout

No additional steps required.

---

## Recommended Workflow

**Best practice when using FastBTN and FastSTAT:**

- Use **`.set` files** for:
  - Different strategies
  - Different symbols
  - Parameter backups
- Use **templates (`.tpl`)** for:
  - Daily trading
  - Fast deployment
  - Consistent layouts

Think of it like this:

- **`.set` files** → parameter presets  
- **`.tpl` files** → complete trading workspace

---

## Important Notes

- Templates work **only in MT5**, not MT4.
- AutoTrading must still be **enabled**.
- If FastBTN or FastSTAT is not installed, the template cannot load them.
- Templates are stored in: `MQL5/Profiles/Templates`

---

## Summary

By combining:
- FastBTN `.set` files
- FastSTAT `.set` files
- MT5 chart templates

you can:
- Save time
- Avoid configuration mistakes
- Switch strategies instantly
- Maintain consistent trading setups

This is the **recommended workflow** for all FastBTN and FastSTAT users.

