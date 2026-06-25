---
description: >-
  A multi-wallet batch swap tool for Raydium. Enables multiple wallets to
  simultaneously swap tokens into a target token, improving trading efficiency
  and execution speed for large-scale transactions.
---

# Solana - Batch Swap Tutorial

{% hint style="info" %}
**CiaoTool Raydium Batch Swap** now fully supports all liquidity pool types, including **AMM, CLMM, and CPMM**. Please switch to the specific pool function page first to perform market making operations.
{% endhint %}

## What is CiaoTool Solana Batch Swap?

<figure><img src="../../../.gitbook/assets/image (808).png" alt="CiaoTool Solana Toolkit Page about Raydium Batch Swap Feature"><figcaption></figcaption></figure>

**CiaoTool Solana Batch Swap** is a multi-address automated trade execution tool custom-built for the **Raydium platform** within the Solana ecosystem. It allows users to fully automatically and synchronously execute token buy and sell operations by batch importing multiple wallet addresses and configuring trading parameters.

The core mechanism of this feature lies in rapidly performing batch swaps of tokens across multiple addresses into a designated token. Compared to traditional manual operations handled one by one via a single address, the system vastly improves the response speed and processing efficiency of trading commands through multi-address concurrent execution. It completely revolutionizes inefficient manual execution models and comprehensively enhances the time-sensitivity of multi-wallet interactions, making it particularly suitable for scenarios that require ultra-fast completion of large-scale token swaps and asset reallocations.

Start your Batch Swap on Raydium with CiaoTool now:

{% embed url="https://ciaotool.io/en-US/raydium/multi-swap" %}

***

## Why Choose CiaoTool Solana Batch Swap?

CiaoTool provides a professional solution for multi-address swapping management on the Raydium platform, balancing ultra-fast speed and security. For users who need to rapidly execute large volumes of transactions, this tool can significantly enhance overall execution efficiency:

* **Ultra-Fast Concurrent Execution**\
  Supports one-click initiation of synchronous swap commands across multiple wallets, completely eliminating the tedious process of manually switching addresses frequently and repeating signatures, vastly improving the time-sensitivity of large-scale transactions.
* **Efficient Asset Swap**\
  Capable of rapidly and synchronously swapping tokens across multiple independent addresses into a designated unified token, meeting various high-frequency, large-volume asset circulation needs.
* **Flexible Parameter Configuration**\
  Supports customizing trading scales for different wallet addresses, precisely matching various complex multi-address automated trading strategies.
* **Local Secure Environment**\
  Utilizes a pure front-end, local execution mechanism where private keys are only used locally for transaction signing, guaranteeing the absolute security of multi-wallet assets while exponentially boosting trading efficiency.

***

## **Step by Step |** Solana Batch Swap

{% stepper %}
{% step %}
### Connect Wallet

Click the button in the top right corner to connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image (799).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select Swap Token

You can choose to enter the token address, or select a token currently owned by your wallet to perform the buy operation. Click the middle arrow to quickly switch the swap direction.

<figure><img src="../../../.gitbook/assets/image (800).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Input Trading Wallet Private Key

{% hint style="danger" %}
<mark style="color:$danger;">**Security Tips**</mark>

Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

{% hint style="info" %}
<mark style="color:$primary;">**Trading Wallet Setting**</mark>

There are no quantity limits on importing wallets for **Raydium Batch Swap**. Transaction fees are paid independently by each wallet.
{% endhint %}

Supports two methods for importing sending private key: **"Manual Input"** and **"Upload File"**. Select an option to view the detailed tutorial.

{% tabs %}
{% tab title="Manual Input" %}
1. Click the **"Manual Input"** button to open the input field.

<figure><img src="../../../.gitbook/assets/image (802).png" alt=""><figcaption></figcaption></figure>

2. Enter / bulk paste private keys, one private key per line. Press Enter to start a new line.

<figure><img src="../../../.gitbook/assets/image (801).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (807).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Click the **"Upload File"** button to open the file upload window.

<figure><img src="../../../.gitbook/assets/image (803).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (804).png" alt=""><figcaption></figcaption></figure>

2. Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.   \
   Click to download and view the template:

{% file src="../../../.gitbook/assets/Solana_privateKey_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (805).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (806).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Enter Buy Amount <a href="#enter-transfer-amount" id="enter-transfer-amount"></a>

<figure><img src="../../../.gitbook/assets/image (712).png" alt=""><figcaption></figcaption></figure>

Support **Custom Input, All Amount, Fixed Amount, Random Amount and Random Percentage.**

1. **Custom Input**\
   Enter the transfer amount for each wallet individually.
   * If an amount is filled in, the transfer will use that specific amount.
   * If an amount is left blank, the transfer will default to the amount configured in the global settings.
2. **All Amount**\
   All wallets will swap 100% of their token holdings into the designated token.
3. **Fixed Amount**\
   All wallets will swap an identical, specified amount of tokens into the designated token.
4. **Random Amount**\
   All wallets will swap a randomized amount of tokens within a preset range into the designated token.
5. **Random Percentage**\
   All wallets will swap a randomized percentage of each wallet's remaining balance within a preset range into the designated token.
{% endstep %}

{% step %}
### Confirm

After verifying all details, click the **"Start Batch Transactions"** button below and wait for the transaction process to complete.
{% endstep %}
{% endstepper %}

## Common Failure Cases

* Slippage set too low, causing the pair price to exceed the specified range.
* Insufficient liquidity, causing severe price volatility.
* Jito tip set too low, resulting in being front-run by MEV bots.

***

## **FAQs**

<details>

<summary><strong>What is Solana Batch Swap?</strong></summary>

Batch Swap refers to the automated execution of buy or sell operations across multiple addresses to complete token swaps within a preset slippage range. This feature is primarily used for rapid portfolio rebalancing or asset conversion of large-scale funds, maximizing execution efficiency while minimizing losses caused by slippage.

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
