---
description: >-
  Built for Pump.fun and PumpSwap, this tool bundles multi-wallet sell
  transactions within the same block to reduce MEV sandwich risks and improve
  exit efficiency.
---

# Pump - Multi-address Bundled Sell Guide

{% hint style="info" %}
**CiaoTool Pump Multi-Address Bundled Sell** now fully supports all quote tokens, including official **SOL and USDC**.
{% endhint %}

## Overview

**CiaoTool Pump Multi-Wallet Bundled Sell** is a batch-selling tool for Pump.fun and PumpSwap. Users can configure multiple seller wallets and token amounts, while the system automatically builds the transactions and submits them in a Bundle according to the preset order.

When executed successfully, the sell transactions within the Bundle are completed consecutively in the same block. This reduces the risk of other transactions being inserted between them and improves execution consistency and management efficiency.

**Use Cases:**

* Batch position reduction or exit across multiple wallets
* Project treasury and operational fund recovery
* Market-making and liquidity position adjustments
* Coordinated selling before multi-wallet asset consolidation
* Automated trading and execution testing

Start your Multi-address Bundled Sell on PumpFun and PumpSwap with CiaoTool now:

{% embed url="https://ciaotool.io/en/pump/multi-address-sell" %}

***

## Advantage

* **Multi-Wallet Configuration:** Configure each seller wallet and its token amount separately
* **Same-Block Execution:** Transactions are completed consecutively in the preset order after the Bundle lands on-chain
* **Reduced Transaction Gaps:** Reduces the risk of other transactions being inserted during batch selling
* **Automated Processing:** Automatically builds, signs, and submits the Bundle
* **Improved Landing Priority:** Uses a Jito tip to improve the Bundle’s landing priority
* **Local Signing:** Private keys are used only for transaction authorization in the browser and are never uploaded

##

***

## **Step by Step |** PumpFun Multi-Address Bundled Sell

{% stepper %}
{% step %}
### **Connect Wallet**

Click the button in the top right corner to connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image (836).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select a Token to Sell

You can choose to enter the token address, or select a token currently owned by your wallet to perform the sell operation.

<figure><img src="../../../.gitbook/assets/image (856).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Input Trading Wallet Private Key

{% hint style="danger" %}
<mark style="color:$danger;">**Security Tips**</mark>

Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

{% hint style="info" %}
<mark style="color:$primary;">**Bundle Settings**</mark>

There is no limit on the number of imported wallets for **PumpFun Multi-address Bundled Sell**, but each transaction group supports a maximum of **20 addresses** for bundled buying.

The service fees for the Multi-address Bundled Buy are paid entirely by the first address of each group, and the Jito tip is paid by the last address imported. Please ensure that the first and last addresses imported have sufficient balances.
{% endhint %}

Supports two methods for importing sending private key: **"Manual Input"** and **"Upload File"**. Select an option to view the detailed tutorial.

{% tabs %}
{% tab title="Manual Input" %}
1. Click the **"Manual Input"** button to open the input field.

<figure><img src="../../../.gitbook/assets/image (857).png" alt=""><figcaption></figcaption></figure>

2. Enter / bulk paste private keys, one private key per line. Press Enter to start a new line.

<figure><img src="../../../.gitbook/assets/image (787).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (860).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Click the **"Upload File"** button to open the file upload window.

<figure><img src="../../../.gitbook/assets/image (858).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (790).png" alt=""><figcaption></figcaption></figure>

2. Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.   \
   Click to download and view the template:

{% file src="../../../.gitbook/assets/Solana_privateKey_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (791).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (859).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Confirm

After verifying all details, click the **"Bundled Sell"** button below and wait for the transaction process to complete.
{% endstep %}
{% endstepper %}

***

## **FAQs**

<details>

<summary><strong>What is the PumpFun Multi-Address Bundled Sell feature?</strong></summary>

It executes synchronous sell operations across multiple wallets within a single block. By packaging transactions together, it eliminates time-gap price fluctuations, minimizes slippage, and boosts execution efficiency—ideal for market exiting and profit-taking.

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
