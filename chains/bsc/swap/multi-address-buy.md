---
description: >-
  PancakeSwap Bundled Buy allows multiple wallets to purchase tokens
  simultaneously and supports both V2 and V3 protocols. Same-block execution
  helps optimize token holder distribution efficiently.
---

# BSC - Multi-Address Bundled Buy Tutorial

{% hint style="info" %}
**CiaoTool PancakeSwap Multi-Address Bundled Buy** supports all **V2 and V3** liquidity pool types. Please switch to the corresponding pool page to perform bundled trading operations based on your needs.
{% endhint %}

## What is CiaoTool PancakeSwap Multi-Address Bundled Buy?

<figure><picture><source srcset="../../../.gitbook/assets/屏幕截图 2026-06-18 142735.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (1000).png" alt="CiaoTool BSC Toolkit Page about PancakeSwap Multi-Address Bundled Buy Feature"></picture><figcaption></figcaption></figure>

**PancakeSwap Multi-Address Bundled Buy** is an advanced strategy for V2 / V3 liquidity pools. It allows users to deploy dozens of sub-wallets to execute concurrent buy orders within a single block, securing low-priced tokens without loss.

Common Use Cases:

* **Anti-MEV Hub**\
  Same-block trade bundling leaves zero time gap for MEV bots, securing entry prices.
* **Whale Masking**\
  Splitting large funds into scattered sub-wallets breaks on-chain links and masks whale accumulation, perfecting the token's early holder metrics.
* **Launch Support**\
  Executing concurrent multi-wallet buys at launch effectively drives up token prices, ignites market sentiment, and stockpiles early low-cost assets.

Start your Multi-Address Bundled Buy on BNB Smart Chain with CiaoTool now:

<table data-card-size="large" data-view="cards"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td>PancakeSwap V2 Multi-Address Bundled Buy</td><td><a href="https://bsc.ciaotool.io/en/swap/v2/multi-address-buy-v2">https://bsc.ciaotool.io/en/swap/v2/multi-address-buy-v2</a></td></tr><tr><td>PancakeSwap V3 Multi-Address Bundled Buy</td><td><a href="https://bsc.ciaotool.io/en/swap/v3/multi-address-buy-v3">https://bsc.ciaotool.io/en/swap/v3/multi-address-buy-v3</a></td></tr></tbody></table>

***

## Why Choose CiaoTool PancakeSwap Multi-Address Bundled Buy?

In fierce on-chain execution, capital efficiency and concealment determine the success or failure of a strategy. CiaoTool builds the ultimate on-chain defense line for professional teams:

* **No-Code V2 / V3**\
  Visualized layout replaces complex RPC scripts to trigger batch swaps on PancakeSwap V2/V3.
* **Local Privacy**\
  Pure client-side local signing ensures total key privacy and multi-wallet safety.
* **All-in-One Toolkit**\
  Smoothly transitions from bundled buys to native market making or multisender within one platform.

***

## **Step by Step**

{% stepper %}
{% step %}
#### **Connect Wallet** <a href="#connect-wallet" id="connect-wallet"></a>

Click the button in the top right corner to connect a wallet that supports the EVM network.

<figure><img src="../../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Enter Payment Wallet Private Key

{% hint style="danger" %}
<mark style="color:red;">**Security Tips**</mark>

Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

Enter the paying wallet's private key. Enter the private key of the wallet that will be used to pay the service fees for market-making operations.

<figure><img src="../../../.gitbook/assets/image (982).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Enter Token Pair Address

For V2, select or enter the market-making token addresses in the token input box; for V3, please enter the pair contract address of the designated pool.

<figure><img src="../../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Import Trading Wallet Private Key

{% hint style="danger" %}
<mark style="color:red;">**Security Tips**</mark>

Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

Supports two import types for trading address private keys: "Manual Input" and "Upload File". Up to 20 addresses is supported.

1. Click the **"Import Private Key"** button to open the input pop-up.

<figure><img src="../../../.gitbook/assets/image (1001).png" alt=""><figcaption></figcaption></figure>

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

Supports two trading amount types: **"Custom Input"**, and **"All"**.

<figure><img src="../../../.gitbook/assets/image (1002).png" alt=""><figcaption></figcaption></figure>

1. **Custom Input**\
   Enter the transfer amount for each wallet individually.
   * If an amount is filled in, the transfer will use that specific amount.
   * If an amount is left blank, the transfer will default to the amount configured in the global settings.
2. **All**\
   Swaps the entire wallet balance into the target token.
{% endstep %}

{% step %}
### **Confirm** <a href="#confirm" id="confirm"></a>

After verifying all details, click the **"Start Swap"** button below and wait for the transaction process to complete.
{% endstep %}
{% endstepper %}

***

**Need help? Join our community for real-time support:**

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
