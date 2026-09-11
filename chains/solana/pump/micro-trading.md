---
description: >-
  A micro trading tool for Pump.fun and PumpSwap. Automatically executes small
  buy and sell transactions to maintain activity, increase visibility, and
  maximize exposure at minimal cost.
---

# Pump - Micro Trading Guide

{% hint style="info" %}
**CiaoTool Pump Micro Trading** now fully supports all quote tokens, including official **SOL and USDC**.&#x20;
{% endhint %}

## Overview

**CiaoTool Pump Micro-Trading Bot** is an automated exposure tool for Pump.fun and PumpSwap. Users can customize micro-trade amounts and execution intervals, while the system continuously executes small buy and sell transactions across multiple wallets.

The tool uses Pump.fun’s recent trading activity display mechanism to keep tokens active through continuous micro-transactions. This increases their chances of appearing on the homepage and recent activity lists, helping projects gain more exposure and attract user attention.

Start your Micro Trading on PumpFun and PumpSwap with CiaoTool now:

{% embed url="https://ciaotool.io/en/pump/micro-trading" %}

***

## Advantage

* **Increased Exposure:** Keeps token activity updated to increase visibility on the homepage and active lists
* **Low-Cost Micro-Trades:** Uses small transactions to control execution costs and price impact
* **Multi-Wallet Trading:** Automatically coordinates multiple wallets for buy and sell operations
* **Flexible Settings:** Customize trade amounts, execution intervals, and run count
* **Automated Cycles:** Start continuous trading with one click and reduce manual operation
* **Local Signing:** Private keys are used locally for transaction authorization and are not uploaded

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

There are no quantity limits on importing wallets. Transaction fees are paid independently by each wallet.
{% endhint %}

Add them **Manually Input** or **Upload File**. Click to view the guide.

{% tabs %}
{% tab title="Manual Input" %}
1. Click the "Bulk Input" button to open the input field.

<figure><img src="../../../.gitbook/assets/image (1184).png" alt=""><figcaption></figcaption></figure>

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

<figure><img src="../../../.gitbook/assets/image (1185).png" alt=""><figcaption></figcaption></figure>

2. Click ![](<../../../.gitbook/assets/image (7).png>)"Import File" button to open the input field.
3. Click "Import" to import all entered wallets into the operation panel.

<figure><img src="../../../.gitbook/assets/image (1165).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Loop Setting

Set the buy price range and wallet execution order. Each transaction will be executed within the specified range.
{% endstep %}

{% step %}
### Trade Interval

Set the execution interval between transactions.

* **Fixed:** Transactions are broadcast at fixed intervals.
* **Random:**&#x54;ransactions are submitted randomly within the specified time range to simulate natural trading activity. Keep the page open during execution.
{% endstep %}

{% step %}
### Start Trade

{% hint style="danger" %}
Closing or refreshing the page will **stop the bot immediately**. Keep the page open and running in the background while the strategy is active. This feature is **not recommended for mobile devices**.
{% endhint %}

Each wallet pays its own transaction fees. After confirming the details, click **“Confirm and Start Micro-Trading”** to launch the trading program.
{% endstep %}

{% step %}
### Confirm

The program runs automatically and displays trading activity in real time:

* [x] Successful purchases
* [x] Successful sales
* [x] Failed and stopped steps

<figure><img src="../../../.gitbook/assets/image (1186).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

***

## **FAQs**

<details>

<summary><strong>What is the PumpFun Micro Trading Bot?</strong></summary>

It is an automated execution engine custom-built to sustain real-time order book activity. By deploying continuous, micro-volume bidirectional trades on Pump.fun, the bot exploits the platform's data-refresh mechanism to ensure your token status is constantly updated, permanently maintaining its visibility on the homepage.

</details>

<details>

<summary><strong>How does this differ from Volume Bot?</strong></summary>

Their core objectives are completely different. Volume Bot deploy substantial capital to artificially inflate total trading volume. In contrast, the Micro Trading Bot prioritizes "frequency over capital"—using hyper-low transaction sizes at a relentless pace purely to secure and hold high-visibility homepage exposure.

</details>

<details>

<summary><strong>Why does this operation keep a project pinned to the Pump.fun homepage?</strong></summary>

Pump.fun’s front-end display ranks tokens based on their "most recent transaction timestamp." By generating high-frequency, real-time tx records, the Micro-Transaction Bot seamlessly bumps your token back to the very top of the feed, unlocking continuous algorithmic exposure.

</details>

<details>

<summary><strong>Will running micro-transactions bleed my capital rapidly?</strong></summary>

Attrition is negligible. Because each individual trade size is tuned to the absolute minimum, your principal constantly rolls back and recirculates between buy and sell execution loops. Your only real overhead consists of standard Solana network gas and the fractional platform fees applied by Pump.fun.

</details>

<details>

<summary><strong>Will enabling this feature impact the token's price chart?</strong></summary>

Virtually zero impact. Due to the hyper-micro capital scale of each interaction, the transactions lack the weight to push the price up or down along the bonding curve. On the chart, it manifests simply as an ultra-dense cluster of activity dots without disrupting the underlying price action or market structure.

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
