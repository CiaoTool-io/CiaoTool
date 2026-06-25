---
description: >-
  Rapidly disperse tokens from a few addresses into multiple brand-new ones.
  Dilute top holders, optimize the on-chain distribution structure, enhance
  chart naturalness, and boost project credibility.
---

# Solana - Asset Fragmentation Tutorial

{% hint style="info" %}
You are currently on the **"Solana -** Fragmentatio&#x6E;**"** tutorial page.

Click [**"EVM - Fragmentation"**](../../../tools/asset-migration/fragmentation.md) to view tutorials for EVM networks such as BSC, Base, X Layer, and IoTeX.
{% endhint %}

## What is CiaoTool Solana Fragmentation? <a href="#definition" id="definition"></a>

<figure><img src="../../../.gitbook/assets/image (723).png" alt="CiaoTool Solana Toolkit Page about Fragmentation Feature"><figcaption></figcaption></figure>

Solana Fragmentation (Token Holding Dispersal) enables projects or whales to automatically split concentrated tokens across hundreds of newly generated, independent Solana wallets without passing through exchanges or pools.

Since holder distribution is a key metric for project health and decentralization on blockchain explorers, Fragmentation optimizes on-chain bubble charts instantly to enhance underlying data metrics.

Key Use Cases:

* Pre-Launch Initialization: Disperse minted supply to treasuries and contributors before adding liquidity to Raydium, structuring a healthy tokenomics foundation.
* Bubble Chart Optimization: Sever correlations of centralized whale wallets to counter third-party cluster analysis and improve top-holder ratios.
* On-Chain Wallet Matrix: Pre-fund highly segregated sub-wallets for market making bots, eliminating central wallet risks.

Start your holding dispersal and fragmented asset migration on the Solana network now using CiaoTool's Fragmentation feature:

{% embed url="https://ciaotool.io/en-US/changeWarehouseZone/one-click-coldChangeWarehouse" %}

***

## Why Choose CiaoTool for Solana Fragmentation?

In a high-speed blockchain network, the success of asset dispersal depends entirely on execution speed and private key security. CiaoTool builds an ultra-secure on-chain operational defense for professional teams:

* **Maximum Cost Reduction**\
  By utilizing smart contract multi-calls and batch-bundling tech, multiple transfers are aggregated into a single on-chain interaction. This minimizes network fees and significantly cuts funding overhead during large-scale distributions.
* **Local Security Environment**\
  Operating via a pure client-side architecture, private keys never leave your machine and are used solely for local transaction signing. This maximizes execution efficiency while ensuring the absolute security of your multi-wallet assets.

***

## **Step by Step | Solana Fragmentation** <a href="#solana-one-to-multi-guide" id="solana-one-to-multi-guide"></a>

{% stepper %}
{% step %}
### **Connect Wallet**

Click the button in the top right corner to connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image (725).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select a Token to Send

You can choose SOL or any SPL token currently held in your wallet for fragmentation.

<figure><img src="../../../.gitbook/assets/image (726).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
#### Input Wallet Private Key <a href="#input-sending-wallet-private-key" id="input-sending-wallet-private-key"></a>

{% hint style="danger" %}
Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

Supports two methods for importing sending private key: **"Manual Input"** and **"Upload File"**. Select an option to view the detailed tutorial.
{% endstep %}

{% step %}
{% tabs %}
{% tab title="Manual Input" %}
1. Click the **"Manual Input"** button to open the input field.

<figure><img src="../../../.gitbook/assets/image (727).png" alt=""><figcaption></figcaption></figure>

2. Enter / bulk paste **private keys**, one private key per line. Press Enter to start a new line.

<figure><img src="../../../.gitbook/assets/image (730).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (733).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Click the **"Upload File"** button to open the file upload window.

<figure><img src="../../../.gitbook/assets/image (728).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (729).png" alt=""><figcaption></figcaption></figure>

2. Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.   \
   Click to download and view the template:

{% file src="../../../.gitbook/assets/Solana_privateKey_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (731).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (732).png" alt=""><figcaption></figcaption></figure>
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
   Quickly transfer all of a specific token from the wallets to the recipient addresses with no extra steps.
{% endstep %}

{% step %}
### Enter Number of Fragmentation Wallet

Enter the number of destination addresses to fragment each wallet into. Each wallet will transfer its total specified tokens into this set number of wallets. A single address can be fragmented into a maximum of 200 new addresses.

Click **"Generate Wallet"** and the system will automatically download all newly generated fragmented addresses.

<figure><img src="../../../.gitbook/assets/image (734).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
#### **Confirm** <a href="#confirm" id="confirm"></a>

After verifying all details, click the **"Confirm Transfer"** button below and wait for the transaction process to complete.
{% endstep %}
{% endstepper %}

***

## **FAQs**

<details>

<summary><strong>What is the purpose of Fragmentation?</strong></summary>

Fragmentation disperses tokens from your current addresses into a large number of brand-new ones. This dilutes the holding ratio of individual wallets, optimizes the on-chain distribution structure, and enhances project security and stealth.

</details>

<details>

<summary><strong>Why use newly generated wallet addresses after Fragmentation?</strong></summary>

New addresses have no transaction history, preventing them from being flagged as "linked wallets" by on-chain analysis tools. This makes them ideal for strategy restructuring and decentralized operations.

</details>

<details>

<summary><strong>Is the operation secure?</strong></summary>

CiaoTool uses a fully client-side signing mechanism. Your private key is never uploaded or stored on any server, and all transactions are signed locally in your browser. This ensures, at a technical level, that the platform has no access to your private key.

</details>

<details>

<summary><strong>Can I fragment multiple types of tokens at the same time?</strong></summary>

The current version supports selecting a single token for fragmented distribution per session. If you need to disperse multiple assets, simply execute the process for each token sequentially.

</details>

***

**Need help? Join our community for real-time support:**

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
