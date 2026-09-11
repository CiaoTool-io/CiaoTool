---
description: >-
  An automated market-making and trading tool built for Raydium. Increasing
  token trading activity, simulate real on-chain trading, and improve the
  natural appearance of market activity and order flow.
---

# Solana - Market Making Tutorial

{% hint style="info" %}
**CiaoTool Raydium Market Making** now fully supports all liquidity pool types, including **AMM V4, CLMM, and CPMM**.
{% endhint %}

## Overview

**CiaoTool Solana Market Making** is an automated market-making and liquidity management tool for Raydium. Users can customize trade amounts, execution frequency, wallet count, and buy/sell strategies, while the system coordinates multiple wallets to execute trades continuously, increase market activity, and optimize overall data performance.

**Use Cases:**

* **Price Boosting:** Use continuous, staged purchases to strengthen buying pressure and support steady price growth
* **Controlled Pullback:** Execute sales at predefined intervals to manage the scale of price corrections
* **Volume Growth:** Use multiple wallets and randomized intervals to increase trading volume and active address count
* **Automated Market-Making:** Run recurring buy-and-sell cycles with less manual work

Start your Market Making on Solana with CiaoTool now:

{% embed url="https://ciaotool.io/en/raydium/market-making" %}

***

## Advantage

* **Multiple Strategies:** Supports price boosting, controlled pullbacks, and trading volume strategies
* **Flexible Settings:** Customize amounts, frequency, intervals, execution count, and participating wallets
* **Multi-Wallet Coordination:** Manage multiple addresses and execute predefined trading strategies
* **Automated Operation:** Start tasks with one click and continuously track their status and results
* **Local Signing:** Private keys are used only for transaction authorization within the browser and are not uploaded

***

## Video Tutorial

{% embed url="https://www.youtube.com/watch?v=WEwHuWE34WM" %}

***

## Step by Step

{% stepper %}
{% step %}
### Connect Wallet

Click the button in the top right corner, and connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select Pair and Pool

#### Token Pair

Enter a token address or select a token held by the connected wallet.

* **Project Token:** The token used to execute the market-making strategy.
* **Quote Token:** The token used to pay for transactions and quote the trading pair price.

<figure><img src="../../../.gitbook/assets/image (1163).png" alt=""><figcaption></figcaption></figure>

#### Pool

Select the pool for market making and ensure it supports the selected trading pair.
{% endstep %}

{% step %}
### Import Private Keys

{% hint style="danger" %}
Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

{% hint style="info" %}
<mark style="color:$primary;">**Trading Wallet Setting**</mark>

There are no quantity limits on importing wallets. Transaction fees are paid independently by each wallet.
{% endhint %}

Add them **Manually Input** or **Upload File**. Click to view the guide.

{% tabs %}
{% tab title="Manual Input" %}
1. Click the "Bulk Input" button to open the input field.

<figure><img src="../../../.gitbook/assets/image (1155).png" alt=""><figcaption></figcaption></figure>

2. Enter / paste wallet private keys, one per line.

```
privateKey
```

<figure><img src="../../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

3. Click "Import" to import all entered wallets into the operation panel.

<figure><img src="../../../.gitbook/assets/image (1166).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Download the CiaoTool template and fill in the transfer details.

<figure><img src="../../../.gitbook/assets/image (1164).png" alt=""><figcaption></figcaption></figure>

2. Click ![](<../../../.gitbook/assets/image (7).png>)"Import File" button to open the input field.
3. Click "Import" to import all entered wallets into the operation panel.

<figure><img src="../../../.gitbook/assets/image (1165).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Trading Mode

Choose a bot type based on your market-making strategy, then switch to the corresponding strategy page.

<figure><img src="../../../.gitbook/assets/image (1167).png" alt=""><figcaption></figcaption></figure>

* **Upward Trend:** Trading wallets continuously buy based on your settings, gradually building positions and increasing buying activity to support an upward trend.
* **Upward Trend:** Trading wallets continuously sell for gradual position reduction or fund recovery, helping form a downward trend.
* **Volume:** Randomly alternates between buys and sells to generate two-way trading activity and keep market data updated.
{% endstep %}

{% step %}
### Trading Setting

{% hint style="danger" %}
Closing or refreshing the page will **stop the bot immediately**. Keep the page open and running in the background while the strategy is active. This feature is **not recommended for mobile devices**.
{% endhint %}

Click a market-making strategy below to view its complete setup guide.

{% tabs %}
{% tab title="Upward Trend" %}
#### Per-trade amount

The amount purchased in each transaction, denominated in the selected **Quote Token**.

If the minimum and maximum values are the same, a fixed amount is used. If they differ, each trade uses a random amount within the range.

#### Stop conditions

Three optional stop conditions are available: **Target Price, Maximum Cumulative Volume**, and **Run Time**. If no condition is set, trading will continue. The task stops automatically when any configured condition is reached.

* **Target Price:** Stops when the **Project Token** reaches the specified price.
* **Maximum cumulative volume:** Stops when the cumulative volume reaches the specified amount, denominated in the **Quote Token**.
* **Maximum duration:** Stops after the specified number of minutes.

<figure><img src="../../../.gitbook/assets/image (1168).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upward Trend" %}
#### Per-trade amount

The amount of **Project Tokens** sold in each transaction.

If the minimum and maximum values are the same, a fixed amount is used. If they differ, each trade uses a random amount within the selected range.

#### Stop conditions

Three optional stop conditions are available: **Target Price, Maximum Cumulative Volume**, and **Run Time**. If no condition is set, trading will continue. The task stops automatically when any configured condition is reached.

* **Target Price:** Stops when the exchange price reaches the specified **Quote Token** value.
* **Maximum cumulative volume:** Stops when the cumulative amount of **Project Tokens** sold reaches the specified value.
* **Run Time:** Stops after the specified number of minutes.

<figure><img src="../../../.gitbook/assets/image (1169).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Volume" %}
#### Per-trade amount

The sell amount for each transaction, denominated in the selected **Quote Token**.

If the minimum and maximum values are the same, a fixed amount is used. If they differ, each trade uses a random amount within the selected range.

#### Stop conditions

Two optional stop conditions are available: **Maximum cumulative volume** and **Run Time**. If neither is set, trading will continue. The task stops automatically when either configured condition is reached.

* **Maximum cumulative volume:** Stops when the cumulative trading volume reaches the specified **Quote Token** amount.
* **Run Time:** Stops after the specified number of minutes.

<figure><img src="../../../.gitbook/assets/image (1170).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### General Settings

{% tabs %}
{% tab title="Interval" %}
Set the execution interval between transactions.

<figure><img src="../../../.gitbook/assets/image (1171).png" alt=""><figcaption></figcaption></figure>

* **Fixed:** Transactions are broadcast at fixed intervals.
* **Random:**&#x54;ransactions are submitted randomly within the specified time range to simulate natural trading activity. Keep the page open during execution.
{% endtab %}

{% tab title="Slippage" %}
Slippage is the difference between the expected price and the actual execution price. Setting the tolerance too low may cause transactions to fail, while setting it too high may expose you to greater price movement.

<figure><img src="../../../.gitbook/assets/image (1172).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Send Method" %}
* **RPC:** Broadcast transactions through an RPC node without paying a Jito tip.
* **Jito Bundle:** Use a Jito tip to improve landing priority.

<figure><img src="../../../.gitbook/assets/image (1173).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Start Trade

Each wallet pays its own transaction fees.

After confirming the details, click **“Start Market Making”** to start the market-making program.

<figure><img src="../../../.gitbook/assets/image (1174).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Confirm

{% hint style="danger" %}
Closing or refreshing the page will **stop the bot immediately**. Keep the page open and running in the background while the strategy is active. This feature is **not recommended for mobile devices**.
{% endhint %}

While the program is running, monitor:

* [x] Current trading pair price
* [x] Number of successful transactions
* [x] Cumulative trading volume and other details

<figure><img src="../../../.gitbook/assets/image (1175).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Common Failure Cases

* Over-pumping, leading to concentrated selling pressure that triggers a sharp crash.
* Insufficient liquidity, causing severe price volatility.
* Over-concentration of token holdings, leaving the market vulnerable to single-point dumping.
* Out-of-control pacing, where frequent operations lead to a decline in market trust.
* Ignoring external market conditions, resulting in failed counter-trend operations.

***

## **FAQs**

<details>

<summary><strong>What is Solana Market Making?</strong></summary>

This feature is used to execute automated trading and market-making strategies within Raydium liquidity pools. Through multi-address buy and sell operations, it boosts trading activity, ensuring the project maintains continuous trading performance and market visibility. By utilizing multi-address and randomized interval mechanisms, it aligns trading behaviors closely with authentic market participation, comprehensively enhancing the naturalness of overall data performance.

</details>

<details>

<summary><strong>Is the operation secure?</strong></summary>

CiaoTool uses a fully client-side signing mechanism. Your private key is never uploaded or stored on any server, and all transactions are signed locally in your browser. This ensures, at a technical level, that the platform has no access to your private key.

</details>

***

## Service Support

Need help? Join our community for real-time support:

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
