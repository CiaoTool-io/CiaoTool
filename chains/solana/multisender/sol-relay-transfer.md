---
description: >-
  Route SOL via intermediary addresses to sever direct links. This disrupts
  funding ties, optimizes bubblemap, secures multi-wallet transfers, and keeps
  your asset strategy discreet.
---

# Solana - Multisender | SOL Relay Transfer Guide

{% hint style="info" %}
You are currently on the **"Solana - SOL Relay Transfe Transfer"** tutorial page.

Click [**"EVM - Relay Transfer"**](../../bsc/multisender/relay-transfer.md) to view multisender tutorials for BNB Smart Chain.
{% endhint %}

## Overview

CiaoTool Solana Relay Transfer is an automated asset-routing tool. It creates an independent relay wallet between the sending wallet and the recipient, splitting a direct transfer into:

**Sending Wallet → Relay Wallet → Recipient Address**

The system generates relay addresses, builds transactions, and tracks execution status based on the task settings, eliminating the need to create or manage relay wallets manually.

**Use Cases:**

* Batch SOL distribution and consolidation
* Multi-wallet asset migration and allocation
* Project treasury and operational fund management
* Test-account funding and balance recovery

Start your SOL Relay Transfer on Solana with CiaoTool now:

{% embed url="https://ciaotool.io/en/transfer/relay-transfer" %}

***

## Advantage

* **Automatic Relay Wallet Creation:** Creates relay addresses based on the number of tasks, with no manual setup required.
* **Automated Two-Stage Execution:** Completes the incoming and outgoing transfers in sequence and records the status of each each stage.
* **Batch Task Support:** Manages multiple relay routes at once to reduce repetitive operations.
* **Clear Fund Flow:** Displays the mapping between sending, relay, and recipient wallets for easy verification.
* **Local Signing:** Transactions are authorized locally, and private keys do not need to be uploaded to the server.

***

## Workflow

Relay transfers use a two-stage routing mechanism. A temporary relay wallet is created between the source and destination wallets, splitting one direct transfer into two independent on-chain transactions:

**Source Wallet → Relay Wallet → Destination Wallet**

<figure><img src="../../../.gitbook/assets/image (1133).png" alt=""><figcaption></figcaption></figure>

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
### Relay Amont

Set the number of relay wallets used for each transfer route.

Additional relay layers can reduce the direct connection between source and destination wallets but will increase the number of transactions, network fees, and execution time.

<figure><img src="../../../.gitbook/assets/image (1134).png" alt=""><figcaption></figcaption></figure>
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

<summary><strong>What is a Relay Transfer?</strong></summary>

The Solana Relay Transfer is a visual operational tool dedicated to on-chain privacy protection. By automatically generating intermediary wallets to act as "stepping stones," it routes funds from the sender to these transit addresses first, before automatically transferring them to the final recipient wallets. This mechanism effectively severs the direct transaction history between the sender and recipient on blockchain explorers.

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

Using the private key import mode, the Relay Transfer feature eliminates the hassle of signing for every individual wallet, with no limit on the number of sending addresses.

</details>

<details>

<summary><strong>What token types are supported for transfers?</strong></summary>

The current version only supports SOL for bulk transfers.

</details>

***

## Service Support

Need help? Join our community for real-time support:

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
