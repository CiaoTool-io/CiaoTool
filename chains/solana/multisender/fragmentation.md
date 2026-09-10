---
description: >-
  Rapidly disperse tokens from a few addresses into multiple brand-new ones.
  Dilute top holders, optimize the on-chain distribution structure, enhance
  chart naturalness, and boost project credibility.
---

# Solana - Asset Fragmentation Guide

{% hint style="info" %}
You are currently on the **"Solana -** Fragmentatio&#x6E;**"** tutorial page.

Click [**"EVM - Fragmentation"**](../../../tools/asset-migration/fragmentation.md) to view tutorials for EVM networks such as BSC, Base, X Layer, and IoTeX.
{% endhint %}

## Overview <a href="#definition" id="definition"></a>

CiaoTool Solana Cold Wallet Reallocation is a batch token distribution tool that allocates tokens from one or more wallets to multiple new or existing Solana wallets using fixed, percentage-based, or randomized amounts.

The system can automatically generate recipient wallets, calculate allocation amounts, create transfer tasks, and execute them in batches. No trading through a centralized exchange or DEX is required, making it suitable for project asset allocation and multi-wallet holdings management.

**Use Cases:**

* **Project Asset Allocation:** Distribute tokens across treasury, operations, and other business wallets
* **Team and Community Distribution:** Allocate tokens to contributors or members according to predefined rules
* **Risk Segmentation:** Reduce the risks associated with storing assets in a single wallet
* **Operational Wallet Preparation:** Prepare wallets for authorized testing, liquidity management, and other operations

Start your holding dispersal and fragmented asset migration on the Solana network now using CiaoTool's Fragmentation feature:

{% embed url="https://ciaotool.io/en/asset-migration/fragmentation" %}

***

## Advantage

* **Automatic Wallet Creation:** Generate recipient addresses in batches and organize the corresponding wallet information.
* **Flexible Distribution:** Allocate tokens using fixed, percentage-based, or randomized amounts.
* **Automatic Grouping:** Automatically create and submit multiple transfer transactions based on the number of tasks.
* **Trackable Results:** View the transfer amount, transaction hash, and execution status of each task.
* **Local Signing:** Private keys are used locally for transaction authorization and are never uploaded to the server.

***

## **Step by Step** <a href="#solana-one-to-multi-guide" id="solana-one-to-multi-guide"></a>

{% stepper %}
{% step %}
### Connect Wallet

Click the button in the top right corner, and connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select a Token to Send

You can choose SOL or any SPL token currently held in your wallet for transfer.

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
### Generate New Wallets

Set the number of new wallets generated for each fragmentation task.

More wallets distribute the tokens across more addresses but also increase transaction fees and ATA rent costs.

<figure><img src="../../../.gitbook/assets/image (1135).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Send method

<figure><img src="../../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

* **RPC**\
  Broadcast transactions through an RPC node without paying a Jito tip.
* **Jito Bundle**\
  Bundle and execute transactions in order, using a Jito tip to increase on-chain priority.
{% endstep %}

{% step %}
### Review Details

Click **“Next”** to review:

* [x] Source wallets and the number of fragmentation wallets
* [x] Transfer amount, total transfer amount, and ATA rent for new addresses
* [x] Estimated fees

<figure><img src="../../../.gitbook/assets/image (1136).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### **Confirm**

After confirming the details, click **“Confirm and Start Fragmentation”** to track the transfer progress and results in real time.

<figure><img src="../../../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>
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

## Service Support

Need help? Join our community for real-time support:

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
