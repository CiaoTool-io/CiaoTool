---
description: >-
  Route SOL via intermediary addresses to sever direct links. This disrupts
  funding ties, optimizes bubblemap, secures multi-wallet transfers, and keeps
  your asset strategy discreet.
---

# Solana - Multisender | Relay Transfer Tutorial

{% hint style="info" %}
You are currently on the **"Solana - Relay Transfe Transfer"** tutorial page.

Click [**"EVM - Relay Transfer"**](../../bsc/multisender/relay-transfer.md) to view multisender tutorials for BNB Smart Chain.
{% endhint %}

## What is CiaoTool Solana Relay Transfer?

<figure><img src="../../../.gitbook/assets/image (720).png" alt="CiaoTool Solana Toolkit Page about Relay Transfer Feature"><figcaption></figcaption></figure>

**CiaoTool Solana Relay Transfer** is an advanced tool dedicated to on-chain privacy protection and asset obfuscation. It allows you to automatically introduce independent intermediary wallet nodes during the transfer process, intelligently routing and distributing SOL (native token) to target wallets in batches.

Compared to standard direct transfers, the core advantage of a Relay Transfer lies in severing the direct on-chain link between the sender and recipient. By automatically routing funds through intermediary addresses, the system perfectly mimics real, independent interactions. This effectively breaks up fund flow paths and optimizes how on-chain tools display cluster analysis and bubble charts. It not only hides capital movements and protects the privacy of master wallets, but also secures flows across multi-wallet interactions.

This tool is particularly suitable for:

* SOL Capital Allocation & Portfolio Splitting under Privacy Protection
* Optimizing On-Chain Bubble Charts & Cluster Analysis Displays
* Secure Asset Distribution Management Across Multiple Addresses

Start your SOL Relay Transfer on Solana with CiaoTool now:

{% embed url="https://ciaotool.io/en-US/wallet/manage/relay-transfer" %}

***

## Why Choose CiaoTool Relay Transfer?

CiaoTool provides a professional solution for managing on-chain assets efficiently and securely on Solana. Whether you need privacy-focused SOL distributions, secure rebalancing across multiple wallets, or complex fund allocations between nodes, the Relay Transfer feature ensures operational accuracy, effectively diversifies fund flow paths, and optimizes on-chain linkage displays by introducing intermediary nodes to mimic real, independent transactions.

Purpose-built for **SOL** asset flows and combined with one-click file imports and bulk processing, it drastically reduces operational overhead. It stands as an indispensable secure asset management tool for any Web3 project or professional team dedicated to building on Solana.

***

## **Step by Step | Solana Multisender - Relay Transfer**

{% stepper %}
{% step %}
### Connect Wallet <a href="#connect-wallet" id="connect-wallet"></a>

Click the button in the top right corner to connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image (721).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select a Token to Send

You can choose SOL or any SPL token currently held in your wallet for transfer.

<figure><img src="../../../.gitbook/assets/image (722).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Input Sending Wallet Private Key

{% hint style="danger" %}
Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

{% hint style="info" %}
The number of sender wallets must match the number of recipient wallets.
{% endhint %}

Supports two methods for importing sending private key: **"Manual Input"** and **"Upload File"**. Select an option to view the detailed tutorial.

{% tabs %}
{% tab title="Manual Input" %}
1. Click the "Manual Input" button to open the input field.

<figure><img src="../../../.gitbook/assets/image (705).png" alt=""><figcaption></figcaption></figure>

2. Enter / bulk paste private keys, one private key per line. Press Enter to start a new line.

<figure><img src="../../../.gitbook/assets/image (707).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (708).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Click the **"Upload File"** button to open the file upload window.

<figure><img src="../../../.gitbook/assets/image (706).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (710).png" alt=""><figcaption></figcaption></figure>

2. Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.   \
   Click to download and view the template:

{% file src="../../../.gitbook/assets/Solana_privateKey_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (711).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (709).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Enter Transfer Amount <a href="#enter-transfer-amount" id="enter-transfer-amount"></a>

<figure><img src="../../../.gitbook/assets/image (712).png" alt=""><figcaption></figcaption></figure>

Click the **"Batch Input"** button above the transfer amount to choose from four transfer modes: **"Amount"**, **"Percentage"**, **"Retain Amount"**, and **"All"**. Custom Input is also supported.

1. **Custom Input**\
   Enter the transfer amount for each wallet individually.
   * If an amount is filled in, the transfer will use that specific amount.
   * If an amount is left blank, the transfer will default to the amount configured in the global settings.
2. **Amount**\
   Apply a uniform, designated amount across all wallets for the transfer.
3. **Percentage**\
   Set a uniform balance percentage; each wallet will transfer funds according to its specific percentage.
4. **Retain Amount**\
   Ensure a fixed amount remains in each wallet for future use, transferring the remaining balance to the recipient address.
5. **All**\
   Quickly transfer all of a specific token from the wallets from the sending addresses with no extra steps.
{% endstep %}

{% step %}
### Input Recipient Wallet Address

{% hint style="info" %}
The number of sender wallets must match the number of recipient wallets.
{% endhint %}

Supports two methods for importing recipient addresses: **"Manual Input"** and **"Upload File"**. Select an option to view the detailed tutorial.

{% tabs %}
{% tab title="Manual Input" %}
1. Click the "Manual Input" button to open the input field.

<figure><img src="../../../.gitbook/assets/image (713).png" alt=""><figcaption></figcaption></figure>

2. Enter / bulk paste wallet addresses, one address per line. Press Enter to start a new line.

<figure><img src="../../../.gitbook/assets/image (715).png" alt=""><figcaption></figcaption></figure>

3. Click "OK" to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (716).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Click the "Upload File" button to open the file upload window.

<figure><img src="../../../.gitbook/assets/image (714).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (718).png" alt=""><figcaption></figcaption></figure>

2. Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.   \
   Click to download and view the template:

{% file src="../../../.gitbook/assets/Solana_address_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (719).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (717).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Set Relay Count

Customize the number of relay addresses. All transfers will pass through the specified number of intermediary addresses before reaching the destination wallet.
{% endstep %}

{% step %}
### **Confirm**

After verifying all details, click the **"Confirm Transfer"** button below and wait for the transaction process to complete.
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

**Need help? Join our community for real-time support:**

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
