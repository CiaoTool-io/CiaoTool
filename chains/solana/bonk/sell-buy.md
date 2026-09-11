---
description: >-
  An asset migration tool for Bonk.fun that combines sells and multi-wallet buys
  within the same block. Creates natural trading activity, reducing MEV risk and
  optimizing on-chain asset distribution.
---

# Bonk - Sell & Bundled Buy Guide

{% hint style="info" %}
**CiaoTool Bonk Sell & Bundled Buy** now fully supports all quote tokens, including official **SOL and USDC**. Please switch to the specific pool function page first to perform bundled operations.
{% endhint %}

## Overview

**CiaoTool Bonk Sell and Multi-Wallet Bundled Buy** is a combined trading tool for Bonk.fun and PumpSwap. Users can configure the selling wallet, sell amount, buying wallets, and purchase amount for each wallet. The system automatically builds a “sell first, buy next” transaction sequence and submits it as a Bundle.

When executed successfully, the sell and multiple buy transactions are completed consecutively within the same block in the preset order. This reduces transaction gaps and repeated wallet switching while improving execution consistency.

**Use Cases:**

* Multi-wallet asset allocation and position adjustments
* Project treasury and operational wallet reconfiguration
* Liquidity management strategy execution
* Combined buy-and-sell strategies and DApp transaction testing
* Batch management of multi-wallet transactions

Start your Sell & Bundled Buy on Bonk with CiaoTool now:

{% embed url="https://ciaotool.io/en/bonk/sell-buy" %}

***

## Advantage

* **Combined Buy and Sell Execution:** Combines a sell from the specified wallet with purchases from multiple wallets in a complete transaction sequence
* **Same-Block Sequential Execution:** Transactions within the Bundle are completed in the preset order after landing on-chain
* **Reduced Transaction Gaps:** Reduces the risk of other transactions being inserted between the sell and buy transactions
* **Multi-Wallet Configuration:** Configure each buying wallet and its purchase amount separately
* **Automated Execution:** Automatically builds, signs, and submits the Bundle
* **Local Signing:** Private keys are used only for transaction authorization in the browser and are never uploaded

***

## Technology Workflow

#### Traditional Trade

Transactions from multiple wallets are broadcast separately and confirmed independently, with no guarantee of execution order or inclusion in the same block. If other transactions execute first, the trading-pair price may fluctuate, increasing the cost for subsequent buying wallets and reducing the number of tokens received.

<figure><img src="../../../.gitbook/assets/image (1191).png" alt=""><figcaption></figcaption></figure>

#### Bundled Trade

The sell transaction and multi-wallet buy transactions are packaged into a Bundle in the preset order and executed consecutively within the same block. This reduces the risk of other transactions being inserted between them while improving execution consistency and transaction priority.

<figure><img src="../../../.gitbook/assets/image (1193).png" alt=""><figcaption></figcaption></figure>

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
### Seller Wallet

{% hint style="danger" %}
Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

Enter the selling wallet’s private key and the amount of the target token to sell.
{% endstep %}

{% step %}
### Buyer Private Keys

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

The program runs automatically. Review the following information on the confirmation page:

* [x] Number of buying wallets, purchase amount, and estimated tokens received
* [x] Sell amount and estimated proceeds

<figure><img src="../../../.gitbook/assets/image (1198).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Start Trade

{% hint style="info" %}
**Bundle Settings**

The first address in each group pays the service fee, while the last imported address pays the Jito tip. Ensure both addresses have sufficient balances.
{% endhint %}

After confirming the details, click **“Sell and Bundled Buy”** to track the trade progress and result in real time.
{% endstep %}
{% endstepper %}

***

## **FAQs**

<details>

<summary><strong>What Is the Bonk Sell &#x26; Bundle Buy Feature?</strong></summary>

Sell & Bundle Buy is an advanced asset migration tool built for Bonk.fun. It allows a designated wallet to sell tokens while multiple wallets simultaneously execute buy orders within the same block. Using block-level transaction coordination, assets can be redistributed across wallets through real market trades.

</details>

<details>

<summary><strong>How Is It Different from Fragmentation?</strong></summary>

The main difference lies in how assets are moved on-chain.

**Fragmentation (Transfer-Based)**\
Tokens are distributed directly from one wallet to multiple wallets through standard transfers. No market trades occur, making it suitable for simple asset distribution without affecting market activity.

**Sell & Bundle Buy (Trade-Based)**\
Assets are redistributed through real sell and buy transactions on the market rather than direct transfers. This creates normal trading records on-chain and removes direct transfer links between wallets.

</details>

<details>

<summary><strong>Does Sell &#x26; Bundle Buy Affect Market Data?</strong></summary>

Yes. Since the process is completed through actual market transactions on Raydium, it naturally generates trading activity while redistributing assets. This can contribute to trading volume, active wallet participation, and broader token distribution across multiple addresses.

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
