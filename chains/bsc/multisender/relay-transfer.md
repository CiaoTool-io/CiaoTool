---
description: >-
  Route BNB / BEP-20 via intermediary addresses to sever direct links. This
  disrupts funding ties, optimizes bubblemap, secures multi-wallet transfers,
  and keeps your asset strategy discreet.
---

# BSC - Multisender | Relay Transfer Tutorial

{% hint style="info" %}
You are currently on the **"BSC - Relay Transfer"** tutorial page for EVM networks.

Click [**"Solana - Relay Transfer"**](../../solana/multisender/sol-relay-transfer.md) to view the Solana network multisender tutorial.
{% endhint %}

## What is CiaoTool BSC Relay Transfer?

<figure><img src="../../../.gitbook/assets/image (936).png" alt="CiaoTool BSC Toolkit Page about BSC Batch Relay Transfer Feature"><figcaption></figcaption></figure>

CiaoTool BSC Intermediary Transfer is an advanced asset privacy and trace-resistant flow tool explicitly crafted for the BSC (BNB Smart Chain) network.

It automatically inserts a brand-new layer of "isolated intermediary wallets" between the sender (source wallet) and the receiver (target wallet). This breaks down what would otherwise be a fully visible transfer on the public ledger into a disconnected path: "Source Address → Intermediary Address → Target Address."

Compared to traditional direct transfers, Intermediary Transfer eliminates the need for users to manually create and manage temporary wallets. The system automatically handles intermediary address generation, fund routing, and workflow execution, significantly lowering the operational barrier for complex asset migrations.

Start your Relay Transfer on BNB Smart Chain with CiaoTool now:

{% embed url="https://bsc.ciaotool.io/en/transfer/relay-transfer" %}

***

## Why Choose CiaoTool BSC Relay Transfer?

Cross-distributing funds across numerous addresses carries high risks of operational errors and private key exposure. CiaoTool delivers an efficient and secure solution for complex matrix allocations:

* **Smart Intermediary Isolation**\
  Automatically insert independent intermediary wallets between senders and receivers, breaking a single-path transfer into multi-stage steps to optimize on-chain linkage.
* **Automated Wallet Generation**\
  Eliminate manual temporary wallet creation. The system dynamically generates intermediary addresses and executes the entire workflow seamlessly.
* **Efficient Batch Execution**\
  Run intermediary tasks across multiple wallets simultaneously. No account switching or repetitive signing required, maximizing large-scale migration speed.
* **Flexible Asset Restructuring**\
  Integrate intermediary routing with multi-address migration for flexible fund structures, perfectly fitting token dispersion, portfolio rebalancing, and wallet management.
* **Local Security**\
  Front-end local execution ensures private keys never leave your device. Sign transactions locally for absolute multi-wallet security with top-tier efficiency.

***

## **Video Tutorial**

{% embed url="https://www.youtube.com/watch?t=1s&v=BnwoyB8k2wU" %}

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

<summary><strong>What Is BSC Relay Transfer?</strong></summary>

A visual on-chain privacy tool that uses automatically generated temporary wallets as a "springboard." By routing funds via "Sender → Intermediary → Receiver," it effectively breaks the direct transaction link between the two parties on blockchain explorers.

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
