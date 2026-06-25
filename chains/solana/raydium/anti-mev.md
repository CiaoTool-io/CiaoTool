---
description: >-
  An anti-MEV trading tool for Raydium. Executes buy and sell transactions
  within the same block to reduce MEV interference and capital loss. Helps
  increase trading volume and improve market activity.
---

# Solana - Anti-MEV Volume Bot Tutorial

{% hint style="info" %}
**CiaoTool Raydium Anti-MEV Volume Bot** now fully supports all liquidity pool types, including **AMM, CLMM, and CPMM**. Please switch to the specific pool function page first to perform market making operations.
{% endhint %}

## What is CiaoTool Solana Anti-MEV Volume Bot?

<figure><img src="../../../.gitbook/assets/image (814).png" alt="CiaoTool Solana Toolkit Page about Raydium Anti-MEV Volume Bot Feature"><figcaption></figcaption></figure>

**CiaoTool Solana Anti-EVM Volume Bot** is an advanced automated trade execution tool custom-built for the Raydium platform within the Solana ecosystem. It allows users to execute fully automated, continuous buy and sell interactions on-chain through customized parameters, safely boosting token trading activity.

Compared to conventional volume tools, the core mechanism of this feature lies in "same-block aggregated execution." The system bundles both the buy and sell operations of a token to be completed synchronously within the very same block. This underlying mechanism effectively prevents transactions from being "sandwiched" by on-chain MEV bots, thereby avoiding the severe slippage and capital attrition commonly seen in high-frequency interactions. It steadily enhances the token's trading volume, the number of unique trading addresses, and the overall naturalness of data performance under the prerequisite of ultra-low slippage loss.

Start your Anti-EVM Volume Bot on Raydium with CiaoTool now:

{% embed url="https://ciaotool.io/en-US/raydium/anti-mev" %}

***

## Why Choose CiaoTool Solana Anti-MEV Volume Bot?

**CiaoTool** provides a professional solution for boosting trading volume on the **Raydium platform**, balancing high security with ultra-low costs. Whether you need to maintain daily order book activity or optimize on-chain data presentation, this tool builds a robust execution defense for you:

* **Secure Anti-MEV Protection**\
  Two-way buy and sell operations are seamlessly aggregated and executed within the same block, effectively blocking sandwich attack interference from MEV bots and ensuring a secure transaction process.
* **Ultra-Low Capital Attrition**\
  By evading MEV bot risks and locking execution into the same block, the impact of slippage and capital attrition is minimized to the greatest extent, achieving your trading volume goals at an ultra-low cost.
* **Optimize On-Chain Data**\
  Through automated and continuous multi-address interactions, it steadily enhances token trading volume and activity, making on-chain behaviors closely align with authentic market participation.
* **Fully Automated Efficient Execution**\
  Supports customized transaction scales and frequencies. With a one-click initiation for automated cyclic execution, it completely eliminates tedious manual operations, vastly improving operational efficiency.

***

## **Step by Step |** Solana Anti-MEV Volume Bot

{% stepper %}
{% step %}
### Connect Wallet

Click the button in the top right corner to connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select a Token to trade

You can choose to enter the token address, or select a token currently owned by your wallet to perform the buy operation.

<figure><img src="../../../.gitbook/assets/image (815).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Input Trading Wallet Private Key

{% hint style="danger" %}
<mark style="color:$danger;">**Security Tips**</mark>

When use private key import. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

{% hint style="info" %}
<mark style="color:$primary;">**Trading Wallet Setting**</mark>

There are no quantity limits on importing wallets using private keys for **Raydium Anti-MEV Volume Bot**. Transaction fees are paid independently by each wallet.
{% endhint %}

Supports two modes: **"Current Wallet"** and **"Private Keys".**

* **Current Wallet:** Allows single-wallet transaction operations exclusively through the currently connect wallet.
* **Private Keys:** Supports multi-address synchronous transaction operations to decentralize holders. It supports two import types for transfer address private keys: **"Manual Input"** and **"Upload File".** Select an option to view the detailed tutorial.

{% tabs %}
{% tab title="Manual Input" %}
1. Click the **"Manual Input"** button to open the input field.

<figure><img src="../../../.gitbook/assets/image (816).png" alt=""><figcaption></figcaption></figure>

2. Enter / bulk paste private keys, one private key per line. Press Enter to start a new line.

<figure><img src="../../../.gitbook/assets/image (801).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (819).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Click the **"Upload File"** button to open the file upload window.

<figure><img src="../../../.gitbook/assets/image (817).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (804).png" alt=""><figcaption></figcaption></figure>

2. Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.   \
   Click to download and view the template:

{% file src="../../../.gitbook/assets/Solana_privateKey_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (805).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (818).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Trading Setting

{% hint style="danger" %}
Closing / refreshing the page will **immediately stop** the bot strategy. Please ensure that the page remains open and running continuously in the background while the strategy is being executed. To ensure necessary strategy execution, **this feature is not recommended for use on mobile devices.**
{% endhint %}

* **Trading Amount Settings:** The amount range for a single buy and sell operation for each wallet. It can be configured to execute buy and sell operations with a randomized amount within a specified range.
* **Task Execution Interval:** The transaction interval between each buy and sell operation. It can be configured to execute buy and sell operations at randomized time intervals within a specified range.
* **Transaction Times:** Sets the number of transaction cycles for each wallet. One buy and one sell for a single cycle.

<figure><img src="../../../.gitbook/assets/image (820).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Confirm

After verifying all details, click the **"Start"** button below and wait for the transaction process to complete.
{% endstep %}
{% endstepper %}

## Common Failure Cases

* Bundle packaging failed, resulting in transactions being split during execution.
* Insufficient liquidity, causing excessive slippage during the buying and selling process.
* Insufficient tip, resulting in being preempted by higher-priority transactions.

***

## **FAQs**

<details>

<summary><strong>What is the Solana Anti-MEV Volume Bot?</strong></summary>

This feature is used to execute buy and sell trades within the same block on **Raydium**, forming a closed trading loop. This reduces exposure of the trading path and external interference, thereby enhancing execution stability and trading efficiency.

</details>

<details>

<summary><strong>What are MEV Bots?</strong></summary>

MEV bots are automated blockchain arbitrage programs. By paying higher gas fees to manipulate block order, they sandwich a user's pending transaction with their own buy and sell orders, capturing risk-free spread profits. This is known as a "sandwich attack."

</details>

<details>

<summary><strong>Why do we need an Anti-MEV Volume Bot? What are the pain points of conventional tools?</strong></summary>

Conventional volume bots execute buy and sell commands separately, making them easy targets for MEV attacks. Bots front-run your buys to inflate prices and front-run your sells to force lower returns, causing severe slippage and massive capital attrition. The Anti-MEV Bot eliminates this vulnerability completely.

</details>

<details>

<summary><strong>What role does Jito technology play in anti-MEV execution?</strong></summary>

Jito can bundle and transmit critical transactions to priority pools, elevating on-chain sorting priority and preventing other transactions from cutting in line in between.

</details>

<details>

<summary><strong>How does it achieve "anti-MEV" and minimize transaction attrition?</strong></summary>

The tool utilizes "same-block aggregated execution" to bundle your buy and sell commands together. By executing both interactions consecutively within the exact same block, it leaves zero time lag for MEV bots to insert malicious orders, fundamentally blocking sandwich attacks and minimizing capital attrition.

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
