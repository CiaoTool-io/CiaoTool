---
description: >-
  Conveniently consolidate SOL or SPL tokens scattered across multiple accounts
  into a single master account, improving fund management efficiency while
  reducing transaction costs and time.
---

# Solana - Multisender | Multi-to-One Transfer Tutorial

{% hint style="info" %}
You are currently on the **"Solana - Multi-to-One Transfer"** tutorial page.

Click [**"EVM - Multi-to-One Transfer"**](../../../tools/multisender/multi-to-one/many-to-one.md) to view multisender tutorials for EVM networks such as BSC, opBNB, Base, X Layer, IoTeX, and BOT Chain.
{% endhint %}

## What is CiaoTool Solana Multi-to-One Transfer?

<figure><img src="../../../.gitbook/assets/image (687).png" alt="CiaoTool Solana Toolkit Page about Multi-to-One Transfer Feature"><figcaption></figcaption></figure>

**CiaoTool Solana Multi-to-One Transfer** is a simple and efficient tool that allows you to consolidate SOL (native token) or any SPL token from multiple wallet addresses into a single address at once. Unlike manual, transaction-by-transaction transfers, this feature automates the process, saving time, reducing human error, and streamlining the token consolidation workflow.

Start your Multi-to-One Transfer on Solana with CiaoTool now:

{% embed url="https://ciaotool.io/en-US/wallet/manage/batch-collection" %}

***

## Why Choose CiaoTool Multi-to-One Transfer?

CiaoTool provides the fastest and most reliable way to consolidate tokens on Solana. Whether you are aggregating funds from market-making wallets, reallocating capital, or sweeping idle balances, its bulk transfer feature ensures accuracy, scalability, and a smooth user experience.

Supporting **SOL and SPL tokens**, file imports, and automatic batching, it is an essential tool for any Web3 project operating on Solana.

***

## **Step by Step | Solana Multisender - Multi-to-One Transfer**

{% stepper %}
{% step %}
### Connect Wallet

Click the button in the top right corner to connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image (688).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select a Token to Send

You can choose SOL or any SPL token currently held in your wallet for transfer.

<figure><img src="../../../.gitbook/assets/image (690).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Input Sending Wallet Private Key

{% hint style="danger" %}
Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

Supports two methods for importing sending private key: **"Manual Input"** and **"Upload File"**. Select an option to view the detailed tutorial.

{% tabs %}
{% tab title="Manual Input" %}
1. Click the "Manual Input" button to open the input field.

<figure><img src="../../../.gitbook/assets/image (691).png" alt=""><figcaption></figcaption></figure>

2. Enter / bulk paste private keys, one private key per line. Press Enter to start a new line.

<figure><img src="../../../.gitbook/assets/image (695).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (696).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Click the **"Upload File"** button to open the file upload window.

<figure><img src="../../../.gitbook/assets/image (692).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (693).png" alt=""><figcaption></figcaption></figure>

2. Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.   \
   Click to download and view the template:

{% file src="../../../.gitbook/assets/Solana_privateKey_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (698).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (697).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Enter Transfer Amount

<figure><img src="../../../.gitbook/assets/image (699).png" alt=""><figcaption></figcaption></figure>

Click the "Set" button above the Collect Amount to choose from three transfer modes: **"All"**, **"Collect Amount"**, and **"Retain Amount"**.

1. **All**\
   Quickly consolidate all of a specific token from your wallets to one address with no extra steps.
2. **Collect Amount**\
   Consolidate a uniform amount from all selected wallets.
3. **Retain Amount**\
   Ensure a fixed amount remains in each wallet for future use.
{% endstep %}

{% step %}
### Enter Payment Wallet Private Key

Import the private key; this wallet will be used to pay the transaction fees for this operation.

<figure><img src="../../../.gitbook/assets/image (700).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Enter Recipient Wallet Address

Specify the consolidation recipient address by entering a wallet address or selecting your currently bound wallet.

<figure><img src="../../../.gitbook/assets/image (701).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### **Confirm**

After verifying all details, click the **"Start Collction"** button below and wait for the transaction process to complete.
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

**Need help? Join our community for real-time support:**

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
