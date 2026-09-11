---
description: >-
  A multi-wallet batch swap tool for Bonk.fun. Enables multiple wallets to
  simultaneously swap tokens into a target token, improving trading efficiency
  and execution speed for large-scale transactions.
---

# Bonk - Batch Swap Guide

{% hint style="info" %}
**CiaoTool Bonk Batch Swap** now fully supports all quote tokens, including official **SOL and USD1**.
{% endhint %}

## Overview

**CiaoTool Bonk Batch Trading** is a multi-wallet automated trading tool for Bonk.fun. Users can import or select multiple wallets, configure the trade direction and amount for each wallet, and execute token purchases or sales in one batch.

The system converts these settings into independent trading tasks and submits them concurrently, reducing repetitive wallet switching, parameter entry, and transaction signing.

Start your Batch Swap on Bonk with CiaoTool now:

{% embed url="https://ciaotool.io/en/bonk/batch-swap" %}

***

## Advantage

* **Batch Execution:** Run buy or sell tasks across multiple wallets at once
* **Concurrent Submission:** Broadcast multiple transactions within a short period
* **Flexible Settings:** Configure the trade direction and amount for each wallet
* **Centralized Management:** View wallet balances, transaction statuses, and results in one place
* **Fast Swaps:** Convert assets across multiple wallets into a target asset
* **Local Signing:** Private keys are used locally and are not uploaded

***

## Step by Step

{% stepper %}
{% step %}
### Connect Wallet

Click the button in the top right corner, and connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select Token Pair

Enter a token address or select a token held by the connected wallet.

* **Project Token:** The token used to execute the market-making strategy.
* **Quote Token:** The token used to pay for transactions and quote the trading pair price.

<figure><img src="../../../.gitbook/assets/image (1202).png" alt=""><figcaption></figcaption></figure>
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

<figure><img src="../../../.gitbook/assets/image (1176).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Download the CiaoTool template and fill in the transfer details.

<figure><img src="../../../.gitbook/assets/image (1164).png" alt=""><figcaption></figcaption></figure>

2. Click ![](<../../../.gitbook/assets/image (7).png>)"Import File" button to open the input field.
3. Click "Import" to import all entered wallets into the operation panel.

<figure><img src="../../../.gitbook/assets/image (1177).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Enter Amount

Choose from 4 amount options: **Individual, Fixed, Random Range, or All.**

1. **Individual**\
   Enter a different amount for each address.
2. **Fixed Amount**\
   Click ![](<../../../.gitbook/assets/image (8).png>) above “Amount”, and select “Fixed Amount” to apply the same amount to all addresses.
3. **Random Range**\
   Click ![](<../../../.gitbook/assets/image (8).png>) above “Amount”, and select “Random Range” and set the minimum and maximum. The system will generate an amount within that range for each address.
4. **All**\
   Click ![](<../../../.gitbook/assets/image (8).png>) above “Amount”, and select “All” to transfer the full available balance.
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
{% endtabs %}
{% endstep %}

{% step %}
### Send Method

* **RPC:** Broadcast transactions through an RPC node without paying a Jito tip.
* **Jito Bundle:** Use a Jito tip to improve landing priority.

<figure><img src="../../../.gitbook/assets/image (1173).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Start Swap

The program runs automatically. On the confirmation page, review:

* [x] Active wallets and number of transactions
* [x] Estimated fees

Each wallet pays its own transaction fees.

<figure><img src="../../../.gitbook/assets/image (1178).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Confirm

{% hint style="danger" %}
Closing or refreshing the page will **stop the bot immediately**. Keep the page open and running in the background while the strategy is active. This feature is **not recommended for mobile devices**.
{% endhint %}

After confirming the details, click **“Confirm and Start Batch Swap”** to begin the batch swap process.

<figure><img src="../../../.gitbook/assets/image (1175).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Common Failure Cases

* Slippage set too low, causing the pair price to exceed the specified range.
* Insufficient liquidity, causing severe price volatility.
* Jito tip set too low, resulting in being front-run by MEV bots.

***

## **FAQs**

<details>

<summary><strong>What is Bonk Batch Swap?</strong></summary>

Batch Swap refers to the automated execution of buy or sell operations across multiple addresses to complete token swaps within a preset slippage range. This feature is primarily used for rapid portfolio rebalancing or asset conversion of large-scale funds, maximizing execution efficiency while minimizing losses caused by slippage.

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
