---
description: >-
  Process batch SOL or SPL transfers. Mimic natural transactions to obfuscate
  linkages, avoid cluster detection, and streamline multi-wallet management and
  asset strategy.
---

# Solana - Multisender | Multi-to-Multi Transfer Guide

{% hint style="info" %}
You are currently on the **"Solana - Multi-to-Multi Transfer"** tutorial page.

Click [**"EVM - Multi-to-Multi Transfer"**](../../../tools/multisender/multi-to-multi/many-to-many.md) to view multisender tutorials for EVM networks such as BSC, opBNB, Base, X Layer, IoTeX, and BOT Chain.
{% endhint %}

## Overview

**CiaoTool Solana Multi-to-Multi Transfer** is an advanced tool tailored for efficient Web3 asset management. It allows you to automatically execute batch transfers of SOL or any SPL token from multiple sender wallets to multiple recipient wallets in a single operation.

Compared to traditional single-address distributions, the core advantage of Multi-to-Multi Transfer lies in its ability to completely mimic independent transaction patterns of real users. The system automatically splits and executes peer-to-peer independent transactions, effectively obfuscating fund flow paths and breaking correlation analysis by on-chain tracking tools. This not only significantly saves time on bulk operations and reduces manual error rates, but also effectively prevents wallet addresses from being tracked.

Key Use Cases:

* Untraceable Airdrops & Token Distributions
* Discreet On-Chain Fund Transfers & Diversified Rebalancing
* Efficient Bulk Community Payments Across Multiple Addresses
* Complex Capital Management for Web3 Growth Campaigns

Start your Multi-to-Multi Transfer on Solana with CiaoTool now:

{% embed url="https://ciaotool.io/en/transfer/many-to-many" %}

***

## Advantage

* **Flexible Mapping:** Freely connect multiple sending wallets with multiple recipient addresses.
* **Batch Execution:** Automatically create, group, and submit transfer tasks to reduce repetitive operations.
* **Easy Import:** Import addresses, amounts, and transfer mappings from Excel.
* **Flexible Amounts:** Distribute equal, fixed, or randomized amounts.
* **Multiple Sending Options:** Choose between RPC broadcasting and Jito bundle submission.
* **Pre-Submission Review:** Verify transfer mappings, total amounts, and estimated fees before submitting.
* **Local Signing:** Private keys are used locally for transaction signing and are never uploaded to the server.

## Technical Workflow

Each many-to-many transfer is defined by a sender, recipient, and transfer amount. The system maps multiple sending wallets to multiple recipient addresses, then automatically creates, groups, and executes the transfer tasks for flexible batch asset distribution.

{% columns %}
{% column %}
<table><thead><tr><th width="95">Sender</th><th width="109">Recipient</th><th>Transfer Amount</th></tr></thead><tbody><tr><td>A</td><td>1</td><td>A→1</td></tr><tr><td>A</td><td>2</td><td>A→2</td></tr><tr><td>A</td><td>3</td><td>A→3</td></tr><tr><td>B</td><td>1</td><td>B→1</td></tr><tr><td>B</td><td>2</td><td>B→2</td></tr><tr><td>B</td><td>3</td><td>B→3</td></tr></tbody></table>
{% endcolumn %}

{% column %}
<figure><img src="../../../.gitbook/assets/image.avif" alt=""><figcaption></figcaption></figure>
{% endcolumn %}
{% endcolumns %}

***

## **Step by Step**

{% stepper %}
{% step %}
### Connect Wallet

Click the button in the top right corner, and connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select a Token to Send

You can choose SOL or any SPL token to transfer.

<figure><img src="../../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### **Import Private Keys**

{% hint style="danger" %}
Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

{% hint style="info" %}
The number of sender wallets must match the number of recipient wallets.
{% endhint %}

Unlimited sender addresses. Add them **Manually Input** or **Upload File**. Click to view the guide.

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
### **Import Recipient Addresses**

{% hint style="info" %}
The number of sender wallets must match the number of recipient wallets.
{% endhint %}

Unlimited recipient addresses. Add them **Manually Input** or **Upload File**. Click to view the guide.

{% tabs %}
{% tab title="Manual Input" %}
1. Click the "Bulk Input" button to open the input field.

<figure><img src="../../../.gitbook/assets/image (1129).png" alt=""><figcaption></figcaption></figure>

2. Enter / paste wallet addresses, one per line. Optionally add the transfer amount after each address.

```
address, 300
```

<figure><img src="../../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

3. Click "Import" to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (1130).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Download the CiaoTool template and fill in the transfer details.

<figure><img src="../../../.gitbook/assets/image (1132).png" alt=""><figcaption></figcaption></figure>

2. Click ![](<../../../.gitbook/assets/image (7).png>)"Import File" button to open the input field.
3. Click "Import" to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (1131).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Send Interval

Set the submission interval between transactions.

<figure><img src="../../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

* **Fixed Interval**\
  Set to `0` to broadcast all transactions immediately.
* **Random Interval**\
  Transactions are submitted randomly within the selected time range. Keep the page open during execution.
{% endstep %}

{% step %}
### Send method

The system automatically groups recipients, with up to 4 addresses per group.

<figure><img src="../../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

* **RPC**\
  Broadcasts transactions through an RPC node without a Jito tip. Execution order is not guaranteed.
* **Jito Bundle**\
  Each Bundle supports up to 5 groups, totaling 20 recipients. A Jito tip increases landing priority, and transactions execute in the specified order.
{% endstep %}

{% step %}
### Review Details

Click **“Next”** to review:

* [x] Recipient address for each relay task
* [x] Number of transfers, total transfer amount, and estimated amount received
* [x] Estimated fees

<figure><img src="../../../.gitbook/assets/image (1128).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### **Confirm**

After confirming the details, click **“Confirm and Send”** to track the transfer progress and results in real time.

<figure><img src="../../../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

***

## **FAQs**

<details>

<summary><strong>What is Multi-to-Multi Bulk Transfer?</strong></summary>

Solana Multi-to-Multi Batch Transfer tool is a visual service utility. It allows you to concurrently distribute tokens from multiple sender wallets to multiple target addresses simultaneously, without requiring any code. Through a mesh-cross transfer pattern, it breaks up singular funding tracks, offering greater precision and stealth than manual operations.

</details>

<details>

<summary><strong>How do I import sending addresses?</strong></summary>

You can either manually enter addresses or upload a CSV file to import a list of sending addresses. The system will automatically recognize and display a preview.

</details>

<details>

<summary><strong>Is the operation secure?</strong></summary>

CiaoTool uses a fully client-side signing mechanism. Your private key is never uploaded or stored on any server, and all transactions are signed locally in your browser. This ensures, at a technical level, that the platform has no access to your private key.

</details>

<details>

<summary><strong>How many addresses can be sent at once?</strong></summary>

Using the private key import mode, the Multi-to-Multi Transfer feature eliminates the hassle of signing for every individual wallet, with no limit on the number of sending addresses.

</details>

<details>

<summary><strong>Can I send multiple types of tokens at the same time?</strong></summary>

The current version supports selecting a single SPL token or SOL for multisender. For multiple asset consolidation, you can perform the operation multiple times.

</details>

***

## Service Support

Need help? Join our community for real-time support:

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
