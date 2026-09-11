---
description: >-
  Custom-built for Raydium, this tool executes multi-wallet purchases within a
  single block, securely optimizing holder distribution and boosting asset
  allocation efficiency.
---

# Solana - Multi-address Bundled Buy Guide

{% hint style="info" %}
**CiaoTool Raydium Multi-address Bundled Buy** now fully supports all liquidity pool types, including **AMM V4, CLMM, and CPMM**.
{% endhint %}

## Overview

CiaoTool Pump Multi-Wallet Bundle Buy is a multi-wallet trading tool for Pump.fun and PumpSwap. Users can configure multiple wallets and purchase amounts, while the system automatically builds the transactions and submits them in a Bundle according to the preset order.

When executed successfully, all transactions in the Bundle are completed sequentially within the same block. This reduces the risk of other transactions being inserted between them and improves execution consistency for batch purchases.

**Use Cases:**

* Multi-wallet batch purchases and asset allocation
* Position building for project treasury and operational wallets
* Buying tokens on the Pump.fun Bonding Curve
* Buying tokens on PumpSwap after migration
* Automated trading and liquidity strategy execution

Start your Multi-address Bundled Buy on Raydium with CiaoTool now:

{% embed url="https://ciaotool.io/en/raydium/multi-address-buy" %}

***

## Advantage

* **Multi-Wallet Configuration:** Set the buying wallet and transaction amount individually
* **Same-Block Execution:** Transactions execute sequentially within the same block after the Bundle lands
* **Reduced Transaction Gaps:** Lowers the risk of other transactions being inserted during batch execution
* **Automatic Grouping:** Automatically builds and submits Bundles based on the number of transactions
* **Improved Landing Priority:** Uses Jito tips to increase Bundle landing priority
* **Local Signing:** Transactions are signed locally in the browser without uploading private keys

***

## Technology Workflow

### Traditional Trade

Transactions from multiple wallets are broadcast separately and confirmed independently, with no guarantee of execution order or inclusion in the same block. If other transactions execute first, the pool price may change, increasing the cost for subsequent wallets and reducing the number of tokens received.

<figure><img src="../../../.gitbook/assets/image (1188).png" alt=""><figcaption></figcaption></figure>

### Bundled Trade

Transactions from 10 wallets are packaged into a Bundle in the preset order and executed consecutively within the same block. This reduces the risk of other transactions being inserted between them, improves batch-buy execution consistency, and increases transaction priority.

<figure><img src="../../../.gitbook/assets/image (1190).png" alt=""><figcaption></figcaption></figure>

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

<figure><img src="../../../.gitbook/assets/image (1197).png" alt=""><figcaption></figcaption></figure>

2. Enter / paste wallet private keys, one per line.

```
privateKey
```

<figure><img src="../../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

3. Click "Import" to import all entered wallets into the operation panel.

<figure><img src="../../../.gitbook/assets/image (1123).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Download the CiaoTool template and fill in the transfer details.

<figure><img src="../../../.gitbook/assets/image (1164).png" alt=""><figcaption></figcaption></figure>

2. Click ![](<../../../.gitbook/assets/image (7).png>)"Import File" button to open the input field.
3. Click "Import" to import all entered wallets into the operation panel.

<figure><img src="../../../.gitbook/assets/image (1123).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Enter Amount

Choose from 6 amount options: **Individual, Fixed, Random Range, Retain, Percent, or All.**

1. **Individual**\
   Enter a different amount for each address.
2. **Fixed Amount**\
   Click ![](<../../../.gitbook/assets/image (8).png>) above “Amount”, and select “Fixed Amount” to apply the same amount to all addresses.
3. **Random Range**\
   Click ![](<../../../.gitbook/assets/image (8).png>) above “Amount”, and select “Random Range” and set the minimum and maximum. The system will generate an amount within that range for each address.
4. **Retain Amount**\
   Click ![](<../../../.gitbook/assets/image (8).png>) above “Amount”, and select “Retain Amount” to retain the specified amount in each sending wallet and transfer the remaining balance.
5. **Percent Amount**\
   Click ![](<../../../.gitbook/assets/image (8).png>) above “Amount”, Select “Percent Amount” to calculate the transfer amount based on a specified percentage of each wallet’s balance.
6. **All**\
   Click ![](<../../../.gitbook/assets/image (8).png>) above “Amount”, and select “All” to transfer the full available balance.
{% endstep %}

{% step %}
### Send Method

* **RPC:** Broadcasts transactions without a Jito tip. Execution is best-effort and transactions may not land in the same block, creating a risk of bot interference and potential losses.
* **Jito Bundle:** Uses a Jito tip to package multiple transactions into one Bundle, preventing transaction insertion and improving landing priority, but incurs additional fees.
{% endstep %}

{% step %}
### Confirm

The program runs automatically. Review the confirmation page and verify:

* [x] Number of trading wallets
* [x] Protocol fees
* [x] Trading principal
{% endstep %}

{% step %}
### Start Trade

{% hint style="info" %}
**Bundle Settings**

The first address in each group pays the service fee, while the last imported address pays the Jito tip. Ensure both addresses have sufficient balances.
{% endhint %}

After confirming the details, click **“Confirm and Start Bundled Buy”** to track the trade progress and result in real time.
{% endstep %}
{% endstepper %}

***

## **FAQs**

<details>

<summary><strong>What is the Solana Multi-address Bundled Buy feature?</strong></summary>

Multi-address Bundled Buy refers to the synchronous execution of buy operations across multiple wallets within the exact same block. By packaging multiple transactions together for execution, it minimizes price fluctuations caused by time gaps, thereby reducing slippage and enhancing overall execution efficiency. This mechanism is especially suitable for critical trading phases such as market opening and position building.

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
