---
description: >-
  Consolidates native or ERC-20 tokens from multiple accounts into a single main
  wallet, improving fund management efficiency while reducing time and
  transaction costs.
---

# EVM - Multisender | Multi-to-One Transfer Tutorial

{% hint style="info" %}
You are currently on the **"EVM - Multi-to-One Transfer"** tutorial page for EVM networks including **BSC, opBNB, Base, X Layer, IoTeX, and BOT Chain.**

Demonstrated on BSC. Universally compatible across all EVM networks, please switch to your target chain to operate.

Click [**"Solana - Multi-to-One Transfer"**](../../../chains/solana/multisender/many-to-one.md) to view the Solana network multisender tutorial.
{% endhint %}

## What is CiaoTool EVM Multi-to-One Transfer?

<figure><img src="../../../.gitbook/assets/image (13).png" alt="CiaoTool BSC Toolkit Page about BSC Batch Multi-to-One Transfer Feature"><figcaption></figcaption></figure>

**CiaoTool EVM Multi-to-One Transfer** is a highly efficient on-chain asset reclamation and multi-wallet fund management tool specially designed for the BSC (BNB Smart Chain) and EVM-compatible ecosystems.

It allows users to fully automatically aggregate specified tokens or native tokens (such as BNB) scattered across hundreds or thousands of sub-wallets into a single main address within a single, visual operation.

Compared to the traditional method of "copying addresses and manually signing transfers one by one," the core mechanism of this feature lies in "underlying batch command aggregation." The system integrates a massive number of independent transfer commands into a single, indivisible data packet via a smart contract, which is then submitted to the blockchain.

Start your Multi-to-One Transfer on EVM Network with CiaoTool now:

<table data-view="cards"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/BSC.png" alt="" data-size="line">BSC (BNB Chain)</td><td><a href="https://bsc.ciaotool.io/en/transfer/many-to-one">https://bsc.ciaotool.io/en/transfer/many-to-one</a></td></tr><tr><td><img src="../../../.gitbook/assets/BSC.png" alt="" data-size="line">opBNB</td><td><a href="https://opbnb.ciaotool.io/en/transfer/many-to-one">https://opbnb.ciaotool.io/en/transfer/many-to-one</a></td></tr><tr><td><img src="../../../.gitbook/assets/Base3.png" alt="" data-size="line">Base</td><td><a href="https://base.ciaotool.io/en/transfer/many-to-one">https://base.ciaotool.io/en/transfer/many-to-one</a></td></tr><tr><td><img src="../../../.gitbook/assets/3 (1).png" alt="" data-size="line">X Layer</td><td><a href="https://xlayer.ciaotool.io/en/transfer/many-to-one">https://xlayer.ciaotool.io/en/transfer/many-to-one</a></td></tr><tr><td><img src="../../../.gitbook/assets/IoTex.png" alt="" data-size="line">IoTeX</td><td><a href="https://iotex.ciaotool.io/en/transfer/many-to-one">https://iotex.ciaotool.io/en/transfer/many-to-one</a></td></tr><tr><td><img src="../../../.gitbook/assets/BOT-2.png" alt="" data-size="line"> BOT</td><td><a href="https://bot.ciaotool.io/en/transfer/many-to-one">https://bot.ciaotool.io/en/transfer/many-to-one</a></td></tr></tbody></table>

***

## Why Choose CiaoTool EVM Multi-to-One Transfer?

CiaoTool provides a professional asset allocation solution for EVM networks, balancing absolute security with minimalist operation. It delivers an efficient, robust execution pipeline for high-frequency, large-scale token or gas distribution:

* **Efficiency Boost**\
  Eliminate tedious manual account switching, address copying, and repetitive signing. Execute hundreds of transfers concurrently with one click for ultra-fast asset aggregation.
* **Flexible Configuration**\
  Import addresses and amounts instantly via Excel. Supports equal, fixed, or random allocations, perfectly adapting to complex airdrop strategies.
* **Local Security**\
  Pure front-end local execution ensures private keys never leave your device. Sign transactions locally to guarantee absolute asset security with maximum speed.

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

<figure><img src="../../../.gitbook/assets/image (919).png" alt=""><figcaption></figcaption></figure>

Enter the receiving address, or click the right button to select the connected wallet.
{% endstep %}

{% step %}
### Input Sender Wallet Private Key

{% hint style="danger" %}
Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

Supports two methods for importing sending private key: **"Manual Input"** and **"Upload File"**. Select an option to view the detailed tutorial.

{% tabs %}
{% tab title="Manual Input" %}
Enter / batch paste wallet private keys, one address per line. Press Enter to start a new line.

<figure><img src="../../../.gitbook/assets/image (922).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Click the "Upload File" button to open the file upload window.

<figure><img src="../../../.gitbook/assets/image (920).png" alt=""><figcaption></figcaption></figure>

2. Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.   \
   Click to download and view the template:

{% file src="../../../.gitbook/assets/EVM_privateKey_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (921).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Confirm Receiving Address

Please verify the destination address to ensure accuracy. Click Next to continue.

<figure><img src="../../../.gitbook/assets/image (923).png" alt=""><figcaption></figcaption></figure>
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

<summary><strong>What Is Multi-to-One Multisender?</strong></summary>

Multi-to-One Multisender consolidates tokens from multiple wallets into one main address for centralized asset management and allocation.

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
