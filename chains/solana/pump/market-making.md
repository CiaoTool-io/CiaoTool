---
description: >-
  An automated market-making and trading tool built for Pump.fun. Increasing
  token trading activity, simulate real on-chain trading, and improve the
  natural appearance of market activity and order flow.
---

# PumpFun - Market Making Guide

{% hint style="info" %}
**CiaoTool PumpFun Market Making** now fully supports all quote tokens, including official **SOL and USDC**.
{% endhint %}

## Overview

**CiaoTool Pump Market Making** is an automated market-making and liquidity management tool for Pump.fun and PumpSwap. Users can customize trade amounts, execution frequency, wallet count, and buy/sell strategies, while the system coordinates multiple wallets to execute trades continuously, increase market activity, and optimize overall data performance.

**Use Cases:**

* **Price Boosting:** Use continuous, staged purchases to strengthen buying pressure and support steady price growth
* **Controlled Pullback:** Execute sales at predefined intervals to manage the scale of price corrections
* **Volume Growth:** Use multiple wallets and randomized intervals to increase trading volume and active address count
* **Automated Market-Making:** Run recurring buy-and-sell cycles with less manual work

Start your Market Making on PumpFun with CiaoTool now:

{% embed url="https://ciaotool.io/en/pump/market-making" %}

***

## Advantage

* **Multiple Strategies:** Supports price boosting, controlled pullbacks, and trading volume strategies
* **Flexible Settings:** Customize amounts, frequency, intervals, execution count, and participating wallets
* **Multi-Wallet Coordination:** Manage multiple addresses and execute predefined trading strategies
* **Automated Operation:** Start tasks with one click and continuously track their status and results
* **Local Signing:** Private keys are used only for transaction authorization within the browser and are not uploaded

***

## Video Tutorial

{% hint style="info" %}
The Market Making function pages for all platforms on the Solana chain are identical. You can watch the "Solana Market Management" video tutorial below to learn more about the detailed steps of the market management feature.
{% endhint %}

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
### Select Token

Enter a token address or select a token held in the connected wallet. The system will automatically identify the quote token and locate the corresponding liquidity pool.

<figure><img src="../../../.gitbook/assets/image (1163).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Import Private Keys

{% hint style="danger" %}
Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

{% hint style="info" %}
<mark style="color:$primary;">**Trading Wallet Setting**</mark>

There are no quantity limits on importing wallets for **PumpFun Market Making**. Transaction fees are paid independently by each wallet.
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
### Enter  Amount

Choose from 2 amount options: **Individual, or Fixed**. Dev and bundled wallets purchases are limited to **86 SOL** in total.

1. **Individual**\
   Enter a different amount for each address.
2. **Fixed Amount**\
   Click ![](<../../../.gitbook/assets/image (8).png>) above “Amount”, and select “Fixed Amount” to apply the same amount to all addresses.
{% endstep %}

{% step %}
### Auto Sell

During the bonding curve phase, all bundled wallets automatically sell when the token reaches the target gain from the initial purchase price.
{% endstep %}

{% step %}
### Jito Tips

{% hint style="danger" %}
This feature uses Jito Bundles and may fail due to network, RPC, or Block Engine conditions. If the Bundle does not land, the token will not be created and no on-chain fees will be charged. Try another RPC or Block Engine, increase the Jito tip, or retry later.
{% endhint %}

Use a Jito tip to bundle token creation and multi-wallet transactions, reducing sniping risk and improving landing priority at an additional cost.

<figure><img src="../../../.gitbook/assets/image (1158).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Confirm

After confirming the details, click **“Create and Buy”** to track the creation progress and result in real time.

<figure><img src="../../../.gitbook/assets/image (1148).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Connect Wallet

Click the button in the top right corner to connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image (757).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select Value Token and MM Token

You can choose to input the token address, or select a token currently owned by your wallet to perform the buy operation.

* **Value Token:** The token address used to pay the pair's price when executing trading operations.
* **MM Token:** The token address used to achieve the market management strategy goals when executing trading operations.

<figure><img src="../../../.gitbook/assets/image (794).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select Market-Making Strategy

Based on different market-making strategy requirements, select the appropriate bot type and switch to the corresponding strategy bot page.

* **Pull Up:** The operating wallet continuously performs buy operations to steadily build positions and drive up the trading pair's price.
* **Drop:** The operating wallet continuously performs sell operations to steadily liquidate positions and drive down the trading pair's price.
* **Trading Bot:** The operating wallet continuously performs both buy and sell operations to keep the order book constantly flashing.

<figure><img src="../../../.gitbook/assets/image (781).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### MM Bot Setting

{% hint style="danger" %}
Closing / refreshing the page will **immediately stop** the bot strategy. Please ensure that the page remains open and running continuously in the background while the strategy is being executed. To ensure necessary strategy execution, **this feature is not recommended for use on mobile devices.**
{% endhint %}

Click the market-making strategies below to display the full bot setup tutorial.

{% tabs %}
{% tab title="Pull Up" %}
#### Single Transaction Volume

The buy volume for each transaction, anchored to the settings of the **"Value Token".**

If the left and right range limits are identical, it will be a fixed amount; if the range amounts differ, each transaction will use a randomized amount within that specified range.

#### Condition Parameters

Three conditional parameters are provided: **Target Price, Total Maximum Transaction Amount, and Duration**. If left blank, transactions will proceed continuously. If any parameter is filled, the task will automatically stop once that condition is met.

* **Target Price:** When the trading pair price reaches the set **"USDT"** value, the strategy execution stops immediately.
* **Total Maximum Transaction Amount:** Anchored to the settings of the **"Value Token",** when the cumulative total reaches the set value, the strategy execution stops immediately.
* **Duration:** Measured in minutes, when the duration reaches the set value, the strategy execution stops immediately.

<figure><img src="../../../.gitbook/assets/image (782).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Drop" %}
#### Single Transaction Volume

The buy volume for each transaction, anchored to the settings of the **"MM Token".**

If the left and right range limits are identical, it will be a fixed amount; if the range amounts differ, each transaction will use a randomized amount within that specified range.

#### Condition Parameters

Three conditional parameters are provided: **Target Price, Total Maximum Transaction Amount, and Duration**. If left blank, transactions will proceed continuously. If any parameter is filled, the task will automatically stop once that condition is met.

* **Target Price:** When the trading pair price reaches the set **"USDT"** value, the strategy execution stops immediately.
* **Total Maximum Transaction Amount:** Anchored to the settings of the **"MM Token",** when the cumulative total reaches the set value, the strategy execution stops immediately.
* **Duration:** Measured in minutes, when the duration reaches the set value, the strategy execution stops immediately.

<figure><img src="../../../.gitbook/assets/image (783).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Traffic Bot" %}
#### Single Transaction Volume

The buy volume for each transaction, anchored to the settings of the **"Value Token".**

If the left and right range limits are identical, it will be a fixed amount; if the range amounts differ, each transaction will use a randomized amount within that specified range.

#### Condition Parameters

Three conditional parameters are provided: **Total Maximum Transaction Amount, and Duration**. If left blank, transactions will proceed continuously. If any parameter is filled, the task will automatically stop once that condition is met.

* **Total Maximum Transaction Amount:** Anchored to the settings of the **"Value Token",** when the cumulative total reaches the set value, the strategy execution stops immediately.
* **Duration:** Measured in minutes, when the duration reaches the set value, the strategy execution stops immediately.

<figure><img src="../../../.gitbook/assets/image (784).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Input Trading Wallet Private Key

{% hint style="danger" %}
<mark style="color:$danger;">**Security Tips**</mark>

Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

{% hint style="info" %}
<mark style="color:$primary;">**Trading Wallet Setting**</mark>

There are no quantity limits on importing wallets for **PumpFun Market Making**. Transaction fees are paid independently by each wallet.
{% endhint %}

Supports two methods for importing sending private key: **"Manual Input"** and **"Upload File"**. Select an option to view the detailed tutorial.

{% tabs %}
{% tab title="Manual Input" %}
1. Click the **"Manual Input"** button to open the input field.

<figure><img src="../../../.gitbook/assets/image (785).png" alt=""><figcaption></figcaption></figure>

2. Enter / bulk paste private keys, one private key per line. Press Enter to start a new line.

<figure><img src="../../../.gitbook/assets/image (787).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (788).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Click the **"Upload File"** button to open the file upload window.

<figure><img src="../../../.gitbook/assets/image (786).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (790).png" alt=""><figcaption></figcaption></figure>

2. Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.   \
   Click to download and view the template:

{% file src="../../../.gitbook/assets/Solana_privateKey_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (791).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (789).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
#### **Confirm** <a href="#confirm" id="confirm"></a>

After verifying all details, click the **"Activate"** button below and wait for the transaction process to complete.

<figure><img src="../../../.gitbook/assets/image (792).png" alt=""><figcaption></figcaption></figure>
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

<summary><strong>What is PumpFun Market Making?</strong></summary>

This feature is used to execute automated trading and market-making strategies within Pump.fun platfotm. Through multi-address buy and sell operations, it boosts trading activity, ensuring the project maintains continuous trading performance and market visibility. By utilizing multi-address and randomized interval mechanisms, it aligns trading behaviors closely with authentic market participation, comprehensively enhancing the naturalness of overall data performance.

</details>

<details>

<summary><strong>Is the operation secure?</strong></summary>

CiaoTool uses a fully client-side signing mechanism. Your private key is never uploaded or stored on any server, and all transactions are signed locally in your browser. This ensures, at a technical level, that the platform has no access to your private key.

</details>

***

**Need help? Join our community for real-time support:**

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
