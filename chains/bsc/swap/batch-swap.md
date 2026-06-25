---
description: >-
  A multi-wallet batch swap tool for PancakeSwap. Supports both V2 and V3
  liquidity pools, allowing tokens from multiple wallets to be swapped into a
  target token efficiently and at scale.
---

# BSC - Batch Swap Tutorial

{% hint style="info" %}
**CiaoTool PancakeSwap Batch Swap** supports all **V2 and V3** liquidity pool types. Please switch to the corresponding pool page to perform market-making operations based on your needs.
{% endhint %}

## What is CiaoTool BSC Batch Swap? <a href="#what-is-coinfactory-solana-multisender" id="what-is-coinfactory-solana-multisender"></a>

<figure><picture><source srcset="../../../.gitbook/assets/屏幕截图 2026-06-18 111902.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (991).png" alt="CiaoTool BSC Toolkit Page about PancakeSwap Batch Swap Feature"></picture><figcaption></figcaption></figure>

**CiaoTool BSC Batch Swap** is an automated on-chain engine that removes single-wallet manual bottlenecks, allowing users to execute batch trades on PancakeSwap V2 / V3 with a single click.

By executing concurrently across multiple addresses, the system rapidly swaps tokens in batches to boost response speed and flow efficiency. This eliminates manual tasks and is ideal for large-scale token swaps or asset allocations.

Start your Batch Swap on BNB Smart Chain with CiaoTool now:

<table data-card-size="large" data-view="cards"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td>PancakeSwap V2 Batch Swap</td><td><a href="https://bsc.ciaotool.io/en/swap/v2/batch-swap-v2">https://bsc.ciaotool.io/en/swap/v2/batch-swap-v2</a></td></tr><tr><td>PancakeSwap V3 Batch Swap</td><td><a href="https://bsc.ciaotool.io/en/swap/v3/batch-swap-v3">https://bsc.ciaotool.io/en/swap/v3/batch-swap-v3</a></td></tr></tbody></table>

***

## Why Choose CiaoTool BSC Batch Swap? <a href="#why-use-coinfactory-multisender-for-solana" id="why-use-coinfactory-multisender-for-solana"></a>

CiaoTool delivers a fast, secure multi-address solution on PancakeSwap, significantly enhancing execution efficiency for high-volume traders:

* **Concurrent Run**\
  One-click synchronized wallet swaps without manual switching or repeating signatures.
* **Efficient Swaps**\
  Instantly aggregates tokens from scattered addresses into a single asset, perfectly matching high-frequency and large-scale fund allocation demands.
* **Flexible Setup**\
  Customizes trade sizes for individual wallets to align precisely with complex automated trading strategies.
* **Local Privacy**\
  Pure client-side local signing ensures total key privacy and multi-wallet safety.

***

## Video Tutorial

{% embed url="https://www.youtube.com/watch?t=1s&v=hhV6wh9jEKc" %}

***

## **Step by Step**

{% stepper %}
{% step %}
### **Connect Wallet**

Click the button in the top right corner to connect a wallet that supports the EVM network.

<figure><img src="../../../.gitbook/assets/image (992).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Enter Token Addresses

{% hint style="info" %}
V2 / V3 layouts vary slightly. Click to switch and view the corresponding tutorial.
{% endhint %}

{% tabs %}
{% tab title="V2" %}
Enter a token address or select from your wallet to buy.\
Click the center arrow to quickly flip the swap direction.

<figure><img src="../../../.gitbook/assets/image (993).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="V3" %}
Unlike V2 liquidity pools, each V3 liquidity pool with a different token pair and fee tier has a unique pool address; please enter the correct pair address to select the swap pair.

Click the center arrow to quickly flip the swap direction.

<figure><img src="../../../.gitbook/assets/image (994).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Enter Payment Wallet Private Key

Enter the paying wallet's private key. Enter the private key of the wallet that will be used to pay the service fees for market-making operations.

<figure><img src="../../../.gitbook/assets/image (995).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Import Trading Wallet Private Key

{% hint style="danger" %}
<mark style="color:red;">**Security Tips**</mark>

Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

Supports two import types for trading address private keys: "Manual Input" and "Upload File". Up to 20 addresses is supported.

1. Click the **"Import Private Key"** button to open the input pop-up.

<figure><img src="../../../.gitbook/assets/image (983).png" alt=""><figcaption></figcaption></figure>

2. Manually enter or import the private key file, and click confirm once the private key is displayed in the confirmation box.

<figure><img src="../../../.gitbook/assets/image (984).png" alt=""><figcaption></figcaption></figure>

Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.\
Click to download and view the template:

{% file src="../../../.gitbook/assets/EVM_privateKey_demo.xlsx" %}
{% endstep %}

{% step %}
### Enter Buy Amount

{% hint style="info" %}
Keep at least 0.0008 BNB in each wallet to cover gas fees.
{% endhint %}

Supports three trading amount types: **"Fixed Amount"**, **"Fixed Retain"**, and **"All Balance"**.

<figure><img src="../../../.gitbook/assets/image (985).png" alt=""><figcaption></figcaption></figure>

1. **Fixed Amount**\
   Swaps a set number of tokens across all wallets.
2. **Fixed Retain**\
   Keeps a set balance in wallets and swaps the rest.
3. **All Balance**\
   Swaps the entire wallet balance into the target token.
{% endstep %}

{% step %}
### Trading Setting

{% hint style="info" %}
V2 / V3 layouts vary slightly. (Skip this step for V3).
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (996).png" alt=""><figcaption></figcaption></figure>

**Slippage**\
Set max slippage percentage.\
The gap between execution and expected price. Too low may cause failed trades; too high exposes you to large price fluctuations.

**Transaction Speed**\
Set higher priority fees to speed up block execution and frontrun MEV bots.

**Timeout**\
The maximum duration allowed for a trade to execute before the pending swap is cancelled.
{% endstep %}

{% step %}
### **Confirm** <a href="#confirm" id="confirm"></a>

After verifying all details, click the **"Start Swap"** button below and wait for the transaction process to complete.
{% endstep %}
{% endstepper %}

***

## **FAQs**

<details>

<summary><strong>What is BSC Batch Swap?</strong></summary>

Batch swap refers to the automated execution of buy or sell operations across multiple addresses. This feature is primarily used for rapid portfolio rebalancing or asset conversion of large-scale funds.

</details>

<details>

<summary><strong>Is It Secure?</strong></summary>

The platform uses a fully client-side signing mechanism. Your private key is never uploaded or stored on any server, and all transactions are signed locally in your browser, ensuring the platform cannot access your private key.

</details>

***

**Need help? Join our community for real-time support:**

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
