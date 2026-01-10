---
date: '2025-12-27T04:35:26Z'
draft: true
title: 'Getting Started'
weight: 3
next: "/docs/configuration/general.md"
---

## Installation

{{% steps %}}

### Extract file
Extract the fastbtn.zip file (or open it with Windows Explorer). You will get the *FastBTN.ex5* file.

### Copy file
Copy *FastBTN.ex5* by pressing `Ctrl + C`, or right-click on the file and select `Copy`.

### Open data folder
In MT5, click `File` → `Open Data Folder`, or simply press `Ctrl + Shift + D`.
   ![](/images/install-01.png)

### Paste file in the right location
A Windows Explorer window containing your MT5 data will open.
   ![](/images/install-02.png)
   Double-click on `MQL5`.
   ![](/images/install-03.png)
   Double-click on `Experts`.
   ![](/images/install-04.png)
   Then paste *FastBTN.ex5* here by pressing `Ctrl + V`, or right-click on a blank space and select `Paste`.
   ![](/images/install-05.png)

### Reload
Close and reopen MT5.

### Open Navigator
If not already open, click `View` → `Navigator` or press `Ctrl + N` to open the Navigator.
   ![](/images/install-06.png)

### Confirm
You should see ***FastBTN*** listed under *Expert Advisors*.
   ![](/images/install-07.png)

### Done
You've successfully copied *FastBTN.ex5* to the correct location.
{{% /steps %}}
---

## Enable Algo Trading
1. Click `Tools` → `Options` or press `Ctrl + O`.
   ![](/images/install-08.png)
2. Click on **`Expert Advisors`** and make sure **`Allow algorithmic trading`** is checked.
   ![](/images/install-09.png)
3. Click OK.

---
## Attaching FastBTN to a Chart

1. Make sure **Algo Trading** is enabled in MT5.
2. Open the chart where you want to use FastBTN.
3. Drag **FastBTN** from the Navigator onto the chart, or double-click it.
4. The EA settings window will appear.
5. Click **OK** to attach the EA.

Once attached, FastBTN buttons will appear on the chart.
![](/images/install-10.png)

---

## Editing Configuration

To edit FastBTN’s settings after it is already running:

### Method 1: Keyboard Shortcut
- Press **`F7`** while the chart is active.

### Method 2: Manual Steps
1. Right-click on the chart and select **Expert List**, or press `Alt + X`.

   ![](/images/edit-01.png)

2. Make sure the correct chart is selected, then click **Properties**.

   ![](/images/edit-02.png)

3. The FastBTN settings window will open.
4. Click the **Inputs** tab to change configuration options.

---

## Logging and Messages

- FastBTN can display messages or logs related to its actions.
- The logs can be found **Experts** tabs
- Logs can help with troubleshooting or verifying EA behavior

If something does not work as expected, checking the logs is a good first step.

---

## Recommended First Setup

For best results when starting out:

- Test FastBTN on a **demo account**
- Use default settings first
- Enable features gradually as you become familiar with them
- Save your settings once you find a setup you like

You can later reuse your preferred setup using saved settings and chart templates.

---

{{< callout type="info" >}}
**Tip**  
If you place the FastBTN buttons on the right side of the chart and they overlap the candles, you can enable **Shift Chart from the Right Border** to create extra space so price bars remain fully visible.

See: [Shift Chart from the Right Border](/docs/fastbtn/shift-chart.md)

![](/images/shift-01.png)
{{< /callout >}}


{{< callout type="info" >}}
**Important Notice**  
Before using FastBTN or FastSTAT on a live account, please make sure you:

- Understand how all features work
- Test everything on a demo account
- Read and accept the [Disclaimer](/docs/disclaimer/)

You are fully responsible for all trading activity.
{{< /callout >}}
