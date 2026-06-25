---
description: >-
  Process batch SOL or SPL transfers. Mimic natural transactions to obfuscate
  linkages, avoid cluster detection, and streamline multi-wallet management and
  asset strategy.
---

# Solana - Multisender | Multi-to-Multi Transfer Tutorial

{% hint style="info" %}
You are currently on the **"Solana - Multi-to-Multi Transfer"** tutorial page.

Click [**"EVM - Multi-to-Multi Transfer"**](../../../tools/multisender/multi-to-multi/many-to-many.md) to view multisender tutorials for EVM networks such as BSC, opBNB, Base, X Layer, IoTeX, and BOT Chain.
{% endhint %}

## What is CiaoTool Solana Multi-to-Multi Transfer?

<figure><img src="../../../.gitbook/assets/image (702).png" alt="CiaoTool Solana Toolkit Page about Multi-to-Multi Transfer Feature"><figcaption></figcaption></figure>

**CiaoTool Solana Multi-to-Multi Transfer** is an advanced tool tailored for efficient Web3 asset management. It allows you to automatically execute batch transfers of SOL or any SPL token from multiple sender wallets to multiple recipient wallets in a single operation.

Compared to traditional single-address distributions, the core advantage of Multi-to-Multi Transfer lies in its ability to completely mimic independent transaction patterns of real users. The system automatically splits and executes peer-to-peer independent transactions, effectively obfuscating fund flow paths and breaking correlation analysis by on-chain tracking tools. This not only significantly saves time on bulk operations and reduces manual error rates, but also effectively prevents wallet addresses from being tracked.

Key Use Cases:

* Untraceable Airdrops & Token Distributions
* Discreet On-Chain Fund Transfers & Diversified Rebalancing
* Efficient Bulk Community Payments Across Multiple Addresses
* Complex Capital Management for Web3 Growth Campaigns

Start your Multi-to-Multi Transfer on Solana with CiaoTool now:

{% embed url="https://ciaotool.io/en-US/wallet/manage/multi-to-multi" %}

***

## Why Choose CiaoTool Multi-to-Multi Transfer?

CiaoTool provides a premier solution for managing on-chain assets efficiently and discreetly on Solana. Whether you need highly anonymous token distributions, secure rebalancing of market-making inventories, or complex fund allocations across nodes, the Multi-to-Multi Transfer feature ensures operational accuracy and seamlessly breaks on-chain links by mimicking real, independent transactions.

With comprehensive **support for SOL** and **all SPL tokens**, combined with one-click file imports and an intelligent automated batching engine, it drastically reduces operational overhead. It stands as an indispensable growth and asset management powerhouse for any Web3 project or professional team dedicated to building on Solana.

***

## **Step by Step | Solana Multisender - Multi-to-Multi Transfer**&#x20;

{% stepper %}
{% step %}
### **Connect Wallet**

Click the button in the top right corner to connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image (703).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select a Token to Send

You can choose SOL or any SPL token currently held in your wallet for transfer.

<figure><img src="../../../.gitbook/assets/image (704).png" alt=""><figcaption></figcaption></figure>
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
### **Confirm**

After verifying all details, click the **"Confirm Transfer"** button below and wait for the transaction process to complete.
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

***

**Need help? Join our community for real-time support:**

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
