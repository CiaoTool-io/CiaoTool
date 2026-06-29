---
description: >-
  One-click SOL / WSOL two-way converter on Solana, accelerating pre-operational
  setups for multi-wallet market making and automated trading.
---

# Solana - SOL Wrapper Tutorial

## What is CiaoTool Solana Wrapper? <a href="#what-is-coinfactory-solana-multisender" id="what-is-coinfactory-solana-multisender"></a>

<figure><img src="../../../.gitbook/assets/image (745).png" alt="CiaoTool Solana Toolkit Page about Solana Wrapper Feature"><figcaption></figcaption></figure>

**CiaoTool Solana Wrapper** is a foundational asset exchange tool built specifically for Solana ecosystem users and project teams. It aims to solve the efficiency pain points of frequent conversions between Solana's native token (SOL) and its wrapped version (WSOL).

On the Solana network, native SOL serves as the base blockchain gas and is not directly compatible with the SPL token standard. Consequently, when executing multi-wallet bulk buying and selling, automated market making, or interacting with the underlying smart contracts of various DEXs, the use of SPL-compliant WSOL is strictly required. The core mechanism of this wrapper provides a high-speed, visual two-way channel: users can wrap SOL into WSOL across multiple wallets with a single click, or unwrap aggregated WSOL back into native SOL at any time, ensuring the seamless flow of funds across different trading scenarios.

Start your SOL wrapping and WSOL unwrapping operations on Solana with CiaoTool now:

{% embed url="https://ciaotool.io/en-US/wallet/solana-wrapper" %}

***

## **Step by Step |** Solana Wrapper

{% stepper %}
{% step %}
### **Connect Wallet**

Click the button in the top right corner to connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image (746).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select Wrap / Unwrap

Click the arrow to toggle between the Wrap SOL and Unwrap WSOL functions.

* Due to smart contract limitations, when wrapping SOL into WSOL, you can customize and enter a specific amount to wrap.
* When unwrapping WSOL back into SOL, you can only perform a full unwrap of all WSOL; entering a specific customized amount for exchange is not supported.

<figure><img src="../../../.gitbook/assets/image (747).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Input Wallet Private Key <a href="#enter-sending-wallet-private-key" id="enter-sending-wallet-private-key"></a>

{% hint style="danger" %}
<mark style="color:$danger;">**Security Tips**</mark>

Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

Supports two methods for importing sending private key: **"Manual Input"** and **"Upload File"**. Select an option to view the detailed tutorial.

{% tabs %}
{% tab title="Manual Input" %}
1. Click the **"Upload File"** button to open the file upload window.

<figure><img src="../../../.gitbook/assets/image (750).png" alt=""><figcaption></figcaption></figure>

2. Enter / bulk paste private keys, one private key per line. Press Enter to start a new line.

<figure><img src="../../../.gitbook/assets/image (749).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (755).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Click the **"Upload File"** button to open the file upload window.

<figure><img src="../../../.gitbook/assets/image (751).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (752).png" alt=""><figcaption></figcaption></figure>

2. Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.   \
   Click to download and view the template:

{% file src="../../../.gitbook/assets/Solana_privateKey_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (753).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (754).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Enter Amount

{% hint style="info" %}
When selecting to convert WSOL to SOL, all WSOL inside the wallet will be converted into SOL; no further action is required on your part for this step.
{% endhint %}

Support **Custom Input** and **All Amount.**

1. **Custom Input**\
   Enter the transfer amount for each wallet individually.
   * If an amount is filled in, the transfer will use that specific amount.
   * If an amount is left blank, the transfer will default to the amount configured in the global settings.
2. **All**\
   Quickly swap all of a specific token from the wallets to the addresses with no extra steps.
{% endstep %}

{% step %}
### **Confirm**

After verifying all details, click the **"Submit"** button below and wait for the transaction process to complete.
{% endstep %}
{% endstepper %}

***

**Need help? Join our community for real-time support:**

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
