---
description: >-
  One-click SOL / WSOL two-way converter on Solana, accelerating pre-operational
  setups for multi-wallet market making and automated trading.
---

# Solana - SOL Wrapper Guide

## Overview <a href="#what-is-coinfactory-solana-multisender" id="what-is-coinfactory-solana-multisender"></a>

CiaoTool WSOL Converter is a tool for converting between SOL and WSOL. It supports batch processing across multiple wallets for DEX trading, automated strategies, and on-chain program interactions.

SOL is the native asset of the Solana network and is used to pay network fees. WSOL is the SPL Token-compatible wrapped version of SOL, designed for operations that require an SPL Token Token interface. Users can wrap SOL into WSOL or unwrap WSOL back into SOL with one click.

Start your SOL wrapping and WSOL unwrapping operations on Solana with CiaoTool now:

{% embed url="https://ciaotool.io/en/wallet/solana-wrapper" %}

***

## Step by Step

{% stepper %}
{% step %}
### **Connect Wallet**

Click the button in the top right corner to connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select Wrap / Unwrap

Click the arrow to toggle between the Wrap SOL and Unwrap WSOL functions.

* Due to smart contract limitations, when wrapping SOL into WSOL, you can customize and enter a specific amount to wrap.
* When unwrapping WSOL back into SOL, you can only perform a full unwrap of all WSOL; entering a specific customized amount for exchange is not supported.

<figure><img src="../../../.gitbook/assets/image (1142).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Choose Wallet to swap <a href="#enter-sending-wallet-private-key" id="enter-sending-wallet-private-key"></a>

<figure><img src="../../../.gitbook/assets/image (1143).png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
<mark style="color:$danger;">**Security Tips**</mark>

Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

Supports two methods for importing sending private key: **"Manual Input"** and **"Upload File"**. Select an option to view the detailed tutorial.

{% tabs %}
{% tab title="Manual Input" %}
1. Click the "Bulk Input" button to open the input field.

<figure><img src="../../../.gitbook/assets/image (1122).png" alt=""><figcaption></figcaption></figure>

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

<figure><img src="../../../.gitbook/assets/image (1125).png" alt=""><figcaption></figcaption></figure>

2. Click ![](<../../../.gitbook/assets/image (7).png>)"Import File" button to open the input field.
3. Click "Import" to import all entered wallets into the operation panel.

<figure><img src="../../../.gitbook/assets/image (1124).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Enter Transfer Amount

{% hint style="info" %}
When selecting to convert WSOL to SOL, all WSOL inside the wallet will be converted into SOL; no further action is required on your part for this step.
{% endhint %}

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
### Review Details

Click **“Next”** to review:

* [x] Source wallets and the number of fragmentation wallets
* [x] Transfer amount, total transfer amount, and ATA rent for new addresses
* [x] Estimated fees

<figure><img src="../../../.gitbook/assets/image (1136).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Review Details

Click **“Next”** to review:

* [x] Wallets and token amounts to be converted
* [x] ATA rent
* [x] Estimated fees

<figure><img src="../../../.gitbook/assets/image (1136).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### **Confirm**

After verifying all details, click the **"Start Exchange"** button below and wait for the transaction process to complete.
{% endstep %}
{% endstepper %}

***

## Service Support

Need help? Join our community for real-time support:

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
