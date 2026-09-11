---
description: >-
  Custom-built for Bonk.fun, this bundled sell tool aggregates multi-address
  sales within the same block—securely minimizing MEV sandwich risks and
  optimizing team asset exit efficiency.
---

# Bonk - Multi-Address Bundled Sell Guide

{% hint style="info" %}
**CiaoTool Bonk Multi-Address Bundled Sell** now fully supports all quote tokens, including official **SOL and USD1**.
{% endhint %}

## Overview

**CiaoTool Bonk Multi-Wallet Bundled Sell** is a batch-selling tool for Bonk.fun. Users can configure multiple seller wallets and token amounts, while the system automatically builds the transactions and submits them in a Bundle according to the preset order.

When executed successfully, the sell transactions within the Bundle are completed consecutively in the same block. This reduces the risk of other transactions being inserted between them and improves execution consistency and management efficiency.

**Use Cases:**

* Batch position reduction or exit across multiple wallets
* Project treasury and operational fund recovery
* Market-making and liquidity position adjustments
* Coordinated selling before multi-wallet asset consolidation
* Automated trading and execution testing

Start your Multi-address Bundled Sell on Bonk.fun with CiaoTool now:

{% embed url="https://ciaotool.io/en-US/bonk/multi-address-sell" %}

***

## Advantage

* **Multi-Wallet Configuration:** Configure each seller wallet and its token amount separately
* **Same-Block Execution:** Transactions are completed consecutively in the preset order after the Bundle lands on-chain
* **Reduced Transaction Gaps:** Reduces the risk of other transactions being inserted during batch selling
* **Automated Processing:** Automatically builds, signs, and submits the Bundle
* **Improved Landing Priority:** Uses a Jito tip to improve the Bundle’s landing priority
* **Local Signing:** Private keys are used only for transaction authorization in the browser and are never uploaded

***

## Technology Workflow

#### Traditional Trade

Transactions from multiple wallets are broadcast separately and confirmed independently, with no guarantee of execution order or inclusion in the same block. If other transactions execute first, the trading pair price may decline, resulting in lower execution prices and fewer assets received by subsequent wallets.

<figure><img src="../../../.gitbook/assets/image (1199).png" alt=""><figcaption></figcaption></figure>

#### Bundled Trade

Tokens from up to 20 wallets are consolidated into one wallet and sold through that wallet. The token transfers and sell transaction are packaged into a single Bundle and executed in the preset order. This reduces the risk of other transactions being inserted between them while improving batch-selling consistency and transaction priority.

<figure><img src="../../../.gitbook/assets/image (1200).png" alt=""><figcaption></figcaption></figure>

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
### Seller Private Keys

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

<figure><img src="../../../.gitbook/assets/image (1196).png" alt=""><figcaption></figcaption></figure>

2. Enter / paste wallet private keys, one per line. Optionally add the transfer amount after each wallet.

```
privateKey, 300
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

<figure><img src="../../../.gitbook/assets/image (1195).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Send Method

* **RPC:** Broadcasts transactions without a Jito tip. Execution is best-effort and transactions may not land in the same block, creating a risk of bot interference and potential losses.
* **Jito Bundle:** Uses a Jito tip to package multiple transactions into one Bundle, preventing transaction insertion and improving landing priority, but incurs additional fees.
{% endstep %}

{% step %}
### Start Trade

{% hint style="info" %}
**Bundle Settings**

The first address in each group pays the service fee, while the last imported address pays the Jito tip. Ensure both addresses have sufficient balances.
{% endhint %}

After confirming the details, click **“Bundled Sell”** to track the trade progress and result in real time.
{% endstep %}
{% endstepper %}

***

## **FAQs**

<details>

<summary><strong>What is the Bonk Multi-Address Bundled Sell feature?</strong></summary>

It executes synchronous sell operations across multiple wallets within a single block. By packaging transactions together, it eliminates time-gap price fluctuations, minimizes slippage, and boosts execution efficiency—ideal for market exiting and profit-taking.

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
