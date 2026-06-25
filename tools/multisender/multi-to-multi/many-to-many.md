---
description: >-
  Batch transfer native or ERC-20 tokens across multiple wallets. Helps reduce
  wallet linkage, improve distribution, and simplify multi-wallet asset
  management.
---

# EVM - Multisender | Multi-to-Multi Transfer Tutorial



{% hint style="info" %}
You are currently on the **"EVM - Multi-to-Multi Transfer"** tutorial page for EVM networks including **BSC, opBNB, Base, X Layer, IoTeX, BOT Chian.**

Demonstrated on BSC. Universally compatible across all EVM networks, please switch to your target chain to operate.

Click [**"Solana - Multi-to-Multi Transfer"**](../../../chains/solana/multisender/many-to-many.md) to view the Solana network multisender tutorial.
{% endhint %}

## What is CiaoTool EVM Multi-to-Multi Transfer?

<figure><img src="../../../.gitbook/assets/image (927).png" alt="CiaoTool BSC Toolkit Page about BSC Batch Multi-to-Multi Transfer Feature"><figcaption></figcaption></figure>

**CiaoTool EVM Multi-to-Multi Transfer** is an advanced parallel asset flow and financial distribution tool specifically crafted for the BSC (BNB Smart Chain) and EVM-compatible ecosystems.

It allows users to cross-transfer and batch-send native tokens (such as BNB) or any BEP-20 / ERC-20 standard tokens from multiple independent source wallets (senders) to multiple target receiving wallets within a single operation.

Compared to traditional unidirectional "One-to-Multi" or "Multi-to-One" models, the core mechanism of this feature lies in "Comprehensive Cross-Matrix Flow." The system breaks the limitations of single address mapping, automatically establishing a cross-network matrix from multiple sources to multiple targets at the underlying layer. This means: Source A and Source B can send funds to Target A simultaneously; likewise, Source A and Source B can also distribute to Target B at the same time.

Start your Multi-to-Multi Transfer on EVM Network with CiaoTool now:

<table data-view="cards"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/BSC.png" alt="" data-size="line">BSC (BNB Chain)</td><td><a href="https://bsc.ciaotool.io/en/transfer/many-to-many">https://bsc.ciaotool.io/en/transfer/many-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/BSC.png" alt="" data-size="line">opBNB</td><td><a href="https://opbnb.ciaotool.io/en/transfer/many-to-many">https://opbnb.ciaotool.io/en/transfer/many-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/Base3.png" alt="" data-size="line">Base</td><td><a href="https://base.ciaotool.io/en/transfer/many-to-many">https://base.ciaotool.io/en/transfer/many-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/3 (1).png" alt="" data-size="line">X Layer</td><td><a href="https://xlayer.ciaotool.io/en/transfer/many-to-many">https://xlayer.ciaotool.io/en/transfer/many-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/IoTex.png" alt="" data-size="line">IoTeX</td><td><a href="https://iotex.ciaotool.io/en/transfer/many-to-many">https://iotex.ciaotool.io/en/transfer/many-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/BOT-2.png" alt="" data-size="line"> BOT</td><td><a href="https://bot.ciaotool.io/en/transfer/many-to-many">https://bot.ciaotool.io/en/transfer/many-to-many</a></td></tr></tbody></table>

***

## Why Choose CiaoTool EVM Multi-to-Multi Transfer?

Cross-distributing funds across numerous addresses carries high risks of operational errors and private key exposure. CiaoTool delivers an efficient and secure solution for complex matrix allocations:

* **Efficiency Boost**\
  Eliminate tedious manual account switching, address copying, and repetitive signing. Execute hundreds of transfers concurrently with one click for ultra-fast asset aggregation.
* **Flexible Configuration**\
  Import addresses and amounts instantly via Excel. Supports equal, fixed, or random allocations, perfectly adapting to complex airdrop strategies.
* **Optimize Fund Distribution**\
  Break up large, uniform fund flows using cross-transfers and random amounts, ensuring more organic asset migration and optimized on-chain links.<br>

***

## **Step by Step**

{% stepper %}
{% step %}
### Switch Chain & Connect Wallet <a href="#switch-chain-and-connect-wallet" id="switch-chain-and-connect-wallet"></a>

Select your target blockchain and connect an EVM-compatible wallet.

<figure><img src="../../../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Enter Recipient Wallet Address

Enter the receiving address, or click the right button to select the connected wallet.

<figure><img src="../../../.gitbook/assets/image (919).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Input Sender Wallet Private Key

{% hint style="danger" %}
Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

{% hint style="info" %}
The number of sender wallets must match the number of recipient wallets.
{% endhint %}

Supports two methods for importing sending private key: **"Manual Input"** and **"Upload File"**. Select an option to view the detailed tutorial.

{% tabs %}
{% tab title="Manual Input" %}
Enter / batch paste wallet private keys, one address per line. Press Enter to start a new line.

<figure><img src="../../../.gitbook/assets/image (931).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Click the "Upload File" button to open the file upload window.

<figure><img src="../../../.gitbook/assets/image (928).png" alt=""><figcaption></figcaption></figure>

2. Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.   \
   Click to download and view the template:

{% file src="../../../.gitbook/assets/EVM_privateKey_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (930).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Input Recipient Wallet Address

{% hint style="danger" %}
Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

{% hint style="info" %}
The number of recipient wallets must match the number of sender wallets.
{% endhint %}

Supports two methods for importing sending private key: **"Manual Input"** and **"Upload File"**. Select an option to view the detailed tutorial.

{% tabs %}
{% tab title="Manual Input" %}
Enter / bulk paste wallet addresses, one address per line. Press Enter to start a new line.

<figure><img src="../../../.gitbook/assets/image (935).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Click the "Upload File" button to open the file upload window.

<figure><img src="../../../.gitbook/assets/image (933).png" alt=""><figcaption></figcaption></figure>

2. Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.   \
   Click to download and view the template:

{% file src="../../../.gitbook/assets/EVM_address_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (934).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Enter Transfer Amount

<figure><img src="../../../.gitbook/assets/image (925).png" alt=""><figcaption></figcaption></figure>

Supports four transfer amount types: **"Custom"**, **"All Balance"**, **"Fixed Amount"**, and **"Fixed Retain"**.

1. **Custom**\
   Enter the transfer amount for each wallet individually.
   * If an amount is filled in, the transfer will use that specific amount.
   * If an amount is left blank, the transfer will default to the amount configured in the global settings.
2. **All Balance**\
   Transfer the entire token balance from all wallets.
3. **Fixed Amount**\
   Transfer an identical, fixed token amount from all wallets.
4. **Fixed Retain**\
   Keep a fixed balance in each wallet and transfer the rest.
{% endstep %}

{% step %}
### Double Check

Review transfer info and check status.

<figure><img src="../../../.gitbook/assets/image (926).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### **Confirm**

After verifying all details, click the **"Send"** button below and wait for the transaction process to complete.
{% endstep %}
{% endstepper %}

***

## **FAQs**

<details>

<summary><strong>What Is Multi-to-Multi Multisender?</strong></summary>

A no-code, visual tool for cross-transferring tokens from multiple senders to multiple receivers instantly. It breaks uniform fund paths for enhanced precision and privacy over manual operations.

</details>

<details>

<summary><strong>How Do I Import Recipient Addresses?</strong></summary>

You can manually enter addresses or upload an Excel file containing recipient addresses. The system will automatically recognize and preview the imported data.

</details>

<details>

<summary><strong>Can I Send Different Amounts to Different Addresses?</strong></summary>

Yes. You can assign a different transfer amount to each address, or set a unified amount or fixed amount for all recipient addresses.

</details>

<details>

<summary><strong>Is It Secure?</strong></summary>

The platform uses a fully client-side signing mechanism. Your private key is never uploaded or stored on any server, and all transactions are signed locally in your browser, ensuring the platform cannot access your private key.

</details>

<details>

<summary><strong>How Many Addresses Can I Send To at Once?</strong></summary>

No limit. Thanks to the private key import design, manual signing for individual wallets is completely eliminated.

</details>

<details>

<summary><strong>Can I Transfer Multiple Tokens at the Same Time?</strong></summary>

Currently, single token batch transfers only. Please repeat the process for different tokens.

</details>

***

**Need help? Join our community for real-time support:**

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
