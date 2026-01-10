---
date: '2025-12-27T04:45:47Z'
draft: true
title: 'Buy & Sell Buttons'
weight: 3
---

## Overview
FastBTN provides 5 buttons to **Buy** and 5 buttons to **Sell**, but you don't have to use them all. To disable a button, simply set the button's lot size to 0 (zero). You can customize each button individually.

---

## Behavior
When you click a Buy or Sell button:
- A market order is sent immediately
- The order uses the current chart symbol
- Trade parameters such as lot size, TP, and SL are applied based on your settings

Because these buttons execute trades instantly, it is important to configure them carefully.

{{< callout type="warning" >}}
**Important**\
FastBTN will send the Buy / Sell order **immediately without any confirmation**, as it is intended to open trade quickly. Please use with caution.
{{< /callout >}}

You can control whether Buy and Sell buttons are shown on the chart. Typical options include:
- Showing both Buy and Sell buttons
- Showing only Buy buttons
- Showing only Sell buttons
- Hiding both buttons completely

These options are useful if:
- You only trade in one direction
- You want to prevent accidental trades
- You are testing other features without opening new positions
  
---

## Buy & Sell Buttons Settings
{{< cards >}}
  {{< card link="/images/buy-sell-buttons-01.png" title="Buy & Sell Buttons Settings" image="/images/buy-sell-buttons-01.png"  method="Resize" options="1000x q80 webp" >}}
{{< /cards >}}

<br>

### Hide Buy & Sell Buttons if Disabled
When you don't use all 5 buttons, you may want to disable some of them. The disabled buttons can still be shown on your chart or be hidden. Set this option to `true` to hide disabled Buy & Sell buttons.

<br>

### If Hidden, Distribute Shown Buttons Evenly
When you disable and hide some buttons, do you want the shown buttons to fill the row? If yes, set this to `true`. This setting only works when *Hide Buy & Sell buttons if disabled* is set to `true`.

<br>

### Some Examples
Here are some examples to make this clearer. Pleae remember that to disable a button, you just need to enter 0 (zero) as its lot size.

<table>
  <thead>
    <tr>
      <th colspan="2">Example 1</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Disabled Buy Buttons</td>
      <td>4, 5</td>
    </tr>
    <tr>
      <td>Disabled Sell Buttons</td>
      <td>None</td>
    </tr>
    <tr>
      <td>Hide Buy & Sell buttons if disabled</td>
      <td><code>true</code></td>
    </tr>
    <tr>
      <td>If hidden, distribute shown buttons evenly</td>
      <td><code>true</code></td>
    </tr>
    <tr>
       <td colspan="2">
         Result:
         <img src="/images/buy-sell-buttons-example-01.png" />
       </td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th colspan="2">Example 2</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Disabled Buy Buttons</td>
      <td>4, 5</td>
    </tr>
    <tr>
      <td>Disabled Sell Buttons</td>
      <td>None</td>
    </tr>
    <tr>
      <td>Hide Buy & Sell buttons if disabled</td>
      <td><code>true</code></td>
    </tr>
    <tr>
      <td>If hidden, distribute shown buttons evenly</td>
      <td><code>false</code></td>
    </tr>
    <tr>
       <td colspan="2">
         Result:
         <img src="/images/buy-sell-buttons-example-02.png" />
       </td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th colspan="2">Example 3</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Disabled Buy Buttons</td>
      <td>4, 5</td>
    </tr>
    <tr>
      <td>Disabled Sell Buttons</td>
      <td>None</td>
    </tr>
    <tr>
      <td>Hide Buy & Sell buttons if disabled</td>
      <td><code>false</code></td>
    </tr>
    <tr>
      <td>If hidden, distribute shown buttons evenly</td>
      <td><code>false / true</code> (no effect)</td>
    </tr>
    <tr>
       <td colspan="2">
         Result:
         <img src="/images/buy-sell-buttons-example-03.png" />
       </td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th colspan="2">Example 4</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Disabled Buy Buttons</td>
      <td>1, 3, 5</td>
    </tr>
    <tr>
      <td>Disabled Sell Buttons</td>
      <td>2, 4</td>
    </tr>
    <tr>
      <td>Hide Buy & Sell buttons if disabled</td>
      <td><code>true</code></td>
    </tr>
    <tr>
      <td>If hidden, distribute shown buttons evenly</td>
      <td><code>false</code></td>
    </tr>
    <tr>
       <td colspan="2">
         Result:
         <img src="/images/buy-sell-buttons-example-04.png" />
       </td>
    </tr>
  </tbody>
</table>

<table>
  <thead>
    <tr>
      <th colspan="2">Example 5</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Disabled Buy Buttons</td>
      <td>1, 3, 5</td>
    </tr>
    <tr>
      <td>Disabled Sell Buttons</td>
      <td>2, 4</td>
    </tr>
    <tr>
      <td>Hide Buy & Sell buttons if disabled</td>
      <td><code>true</code></td>
    </tr>
    <tr>
      <td>If hidden, distribute shown buttons evenly</td>
      <td><code>true</code></td>
    </tr>
    <tr>
       <td colspan="2">
         Result:
         <img src="/images/buy-sell-buttons-example-05.png" />
       </td>
    </tr>
  </tbody>
</table>
You get the idea. Experiment with it to suit your preference.

---

## Text
The *Text* will be displayed **followed by the button's lot size**.

Default values:\
• **Buy** for Buy buttons\
• **Sell** for Sell buttons

So if you set:
- 0.1, 0.2, 0.5, 1, 2 for the buttons' *lot size* for Buy & Sell buttons 1 to 5 respectively
- Set the buttons' *Text* to "Buy" for Buy Buttons and "Sell" for Sell Buttons

Here's what you get:
![](/images/buy-sell-buttons-02.png)

You can set the *Text* to blank:
![](/images/buy-sell-buttons-03.png)

Or you can get creative:
![](/images/buy-sell-buttons-04.png)

{{< callout type="info" >}}
  **Tip**\
  You can always adjust the buttons' width from the *General Settings*.
{{< /callout >}}

---

## Lot Size
Enter the lot size for each button to be executed when the button is pressed. Enter 0 (zero) to disable the button.

---

## Button Color
You can set each button's background color. It is recommended that you use different colors for Buy Buttons and Sell Buttons, but use the same color for all Buy Buttons 1 to 5, and another same color for all Sell Buttons 1 to 5.

---

## Text Color, Font Family, and Font Size
Please refer to [Button Appearance](/docs/configuration/buttons-appearance.md).

---

## Shortcut Key
Only Buy Buttons 1, 2, 3 and Sell Buttons 1, 2, 3 have the option for a shortcut key due to the limitation of only 26 available shortcut keys. Please read more about [shortcut keys](/docs/shortcut-keys.md).

Disabling a button will also disable its shortcut key. Leave blank if you don't want to use it.

---

## Take Profit and Stop Loss Integration
Buy and Sell buttons can work together with:
- Auto Take Profit
- Auto Stop Loss
- Manual TP / SL settings

If Auto TP or Auto SL is enabled, they are applied automatically when the trade is opened. Please refer to [Auto TP & SL](/docs/fastbtn/configuration/auto-tp-sl.md).