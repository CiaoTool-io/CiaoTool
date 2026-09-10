---
description: >-
  Conveniently consolidate SOL or SPL tokens scattered across multiple accounts
  into a single master account, improving fund management efficiency while
  reducing transaction costs and time.
---

# Solana - Multisender | Multi-to-One Transfer Guide

{% hint style="info" %}
You are currently on the **"Solana - Multi-to-One Transfer"** tutorial page.

Click [**"EVM - Multi-to-One Transfer"**](../../../tools/multisender/multi-to-one/many-to-one.md) to view multisender tutorials for EVM networks such as BSC, opBNB, Base, X Layer, IoTeX, BOT, and Robinhood Chain.
{% endhint %}

## Overview

**CiaoTool Solana Many-to-One Transfer** is a batch asset consolidation tool that transfers SOL or supported SPL tokens from multiple wallets to one designated address.

The system automatically creates and groups transfer tasks based on the number of wallets, eliminating repetitive wallet switching, address entry, and manual transaction signing.

**Use Cases:**

* Consolidating SOL or tokens from multiple wallets
* Consolidating project funds and operational revenue
* Recovering balances from test wallets
* Migrating and centrally managing multi-wallet assets

Start your Multi-to-One Transfer on Solana with CiaoTool now:

{% embed url="https://ciaotool.io/en/transfer/many-to-one" %}

***

## Advantage

* **Batch Processing:** Consolidate assets from multiple wallets at once.
* **Flexible Settings:** Import wallets and set individual amounts.
* **Sending Options:** Choose RPC or Jito.
* **Review Before Sending:** Check wallet count, total amount, and fees.
* **Local Signing:** Private keys stay on your device.

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

Choose from 4 amount options: **Individual,All ,  Fixed, or Random Range**.

1. **Individual**\
   Enter a different amount for each address.
2. **All**\
   Click ![](<../../../.gitbook/assets/image (8).png>) above “Amount”, and select “All” to transfer the full available balance.
3. **Fixed Amount**\
   Click ![](<../../../.gitbook/assets/image (8).png>) above “Amount”, and select “Fixed Amount” to apply the same amount to all addresses.
4. **Random Range**\
   Click ![](<../../../.gitbook/assets/image (8).png>) above “Amount”, and select “Random Range” and set the minimum and maximum. The system will generate an amount within that range for each address.
{% endstep %}

{% step %}
### Dedicated Fee Wallet

{% hint style="danger" %}
Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

Use a dedicated wallet to cover network fees, platform service fees, Jito tips, and recipient ATA creation costs.

<figure><img src="../../../.gitbook/assets/image (1126).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Receiver Wallet

Enter the address that will receive the consolidated assets, or select “Current Wallet” to use the connected wallet.

<figure><img src="../../../.gitbook/assets/image (1127).png" alt=""><figcaption></figcaption></figure>
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

The system automatically groups recipients, with up to 5 addresses per group.

<figure><img src="../../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

* **RPC**\
  Broadcasts transactions through an RPC node without a Jito tip. Execution order is not guaranteed.
* **Jito Bundle**\
  Each Bundle supports up to 5 groups, totaling 25 recipients. A Jito tip increases landing priority, and transactions execute in the specified order.
{% endstep %}

{% step %}
### Review Details

Click **“Next”** to review:

* [x] Fee-paying wallet address
* [x] Number of sending wallets, consolidation address, and total amount
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

<summary>What is Multi-to-One Bulk Transfer?</summary>

Multi-to-One consolidation refers to transferring tokens held in multiple wallet addresses into a single master address, facilitating centralized asset management and unified capital allocation.

</details>

<details>

<summary>How do I import sending addresses?</summary>

You can either manually enter addresses or upload a CSV file to import a list of sending addresses. The system will automatically recognize and display a preview.

</details>

<details>

<summary><strong>Is the operation secure?</strong></summary>

CiaoTool uses a fully client-side signing mechanism. Your private key is never uploaded or stored on any server, and all transactions are signed locally in your browser. This ensures, at a technical level, that the platform has no access to your private key.

</details>

<details>

<summary><strong>How many addresses can be sent at once?</strong></summary>

Using the private key import mode, the Multi-to-One Transfer feature eliminates the hassle of signing for every individual wallet, with no limit on the number of sending addresses.

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
