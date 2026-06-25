---
description: >-
  Supports same-block multi-wallet sell execution on Flap.sh. With fully
  client-side processing, it enables efficient batch exits across multiple
  wallets and streamlines multi-wallet asset management.
---

# Flap - Multi-Address Bundled Sell Tutorial

{% hint style="info" %}
**CiaoTool Flap Multi-Address Bundled Sell** fully supports all quote tokens, including  **BNB, USD1, UUSD and USDT**. Please switch to the specific token page to perform bundled trading operations based on your needs.&#x20;
{% endhint %}

## What is CiaoTool Flap Multi-Address Bundled Sell?

<figure><picture><source srcset="../../../.gitbook/assets/屏幕截图 2026-06-18 163137.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (1013).png" alt="CiaoTool BSC Toolkit Page about Flap.sh Multi-Address Bundled Sell Feature"></picture><figcaption></figcaption></figure>

**Flap Multi-Address Bundled Sell** is an advanced strategy for the Flap.sh launchpad. It deploys dozens or hundreds of sub-wallets to execute concurrent sell orders within a single block, achieving instant multi-address fund reclamation.

Common Use Cases:

* **Lossless Exit**\
  Selling one by one manually depresses prices for subsequent wallets. Same-block concurrent execution ensures all sub-wallets exit at the exact same optimal price.
* **Anti-MEV Frontrun**\
  Bundled selling removes the time gap for malicious MEV bots to frontrun large-scale token dumps, fully securing your exit profits.

Start your Multi-Address Bundled Sell on Flap.sh with CiaoTool now:

{% embed url="https://bsc.ciaotool.io/en/flap/bnb/multi-address-sell" %}

***

## Why Choose CiaoTool Flap Multi-Address Bundled Sell?

In fierce on-chain execution, capital efficiency and concealment determine the success or failure of a strategy. CiaoTool builds the ultimate on-chain defense line for professional teams:

* **No-Code**\
  Visual web panel replaces complex RPC scripts. Just check token-holding wallets for one-click anti-MEV bot exits.
* **Local Privacy**\
  Pure client-side local signing ensures total key privacy and multi-wallet safety.
* **All-in-One Toolkit**\
  Instantly links Fourmeme bundled sells with Multi-to-One Transfer to aggregate funds into one wallets.

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

<figure><img src="../../../.gitbook/assets/image (1012).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Enter Token Address

Enter / Paste the contract address of the target token into the token input box.

<figure><img src="../../../.gitbook/assets/image (1009).png" alt=""><figcaption></figcaption></figure>
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
### Enter Sell Amount

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
