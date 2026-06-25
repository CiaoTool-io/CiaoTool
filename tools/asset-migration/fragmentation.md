---
description: >-
  Rapidly disperse tokens from a few addresses into multiple brand-new ones.
  Dilute top holders, optimize the on-chain distribution structure, enhance
  chart naturalness, and boost project credibility.
---

# EVM - Asset Fragmentation Tutorial

{% hint style="info" %}
You are currently on the **"EVM - Fragmentation"** tutorial page for EVM networks including **BSC, Base, X Layer, and IoTeX.**

Demonstrated on BSC. Universally compatible across all EVM networks, please switch to your target chain to operate.

Click [**"Solana - Fragmentation"**](../../chains/solana/asset-migration/fragmentation.md) to view the Solana network tutorial.
{% endhint %}

## What is CiaoTool EVM Fragmentation?

<figure><img src="../../.gitbook/assets/image (937).png" alt="CiaoTool BSC Toolkit Page about Asset Fragmentation Feature"><figcaption></figcaption></figure>

EVM Asset Fragmentation (Token Holding Dispersal) enables projects or whales to automatically split concentrated tokens across hundreds of newly generated, independent Solana wallets without passing through exchanges or pools.

Since holder distribution is a key metric for project health and decentralization on blockchain explorers, Fragmentation optimizes on-chain bubble charts instantly to enhance underlying data metrics.

Key Use Cases:

* Pre-Launch Initialization: Disperse minted supply to treasuries and contributors before adding liquidity to Raydium, structuring a healthy tokenomics foundation.
* Bubble Chart Optimization: Sever correlations of centralized whale wallets to counter third-party cluster analysis and improve top-holder ratios.
* On-Chain Wallet Matrix: Pre-fund highly segregated sub-wallets for market making bots, eliminating central wallet risks.

Start your Asset Fragmentation on EVM Network with CiaoTool now:

<table data-card-size="large" data-view="cards"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td><img src="../../.gitbook/assets/BSC.png" alt="" data-size="line">BSC (BNB Chain)</td><td><a href="https://bsc.ciaotool.io/en/assert-migration/assert-migration-cold">https://bsc.ciaotool.io/en/assert-migration/assert-migration-cold</a></td></tr><tr><td><img src="../../.gitbook/assets/Base3.png" alt="" data-size="line">Base</td><td><a href="https://base.ciaotool.io/en/assert-migration/assert-migration-cold">https://base.ciaotool.io/en/assert-migration/assert-migration-cold</a></td></tr><tr><td><img src="../../.gitbook/assets/3 (1).png" alt="" data-size="line">X Layer</td><td><a href="https://xlayer.ciaotool.io/en/assert-migration/assert-migration-cold">https://xlayer.ciaotool.io/en/assert-migration/assert-migration-cold</a></td></tr><tr><td><img src="../../.gitbook/assets/IoTex.png" alt="" data-size="line">IoTeX</td><td><a href="https://iotex.ciaotool.io/en/assert-migration/assert-migration-cold">https://iotex.ciaotool.io/en/assert-migration/assert-migration-cold</a></td></tr></tbody></table>

***

### Why Choose CiaoTool for EVM Fragmentation? <a href="#why-choose-ciaotool-for-solana-fragmentation" id="why-choose-ciaotool-for-solana-fragmentation"></a>

In a high-speed blockchain network, the success of asset dispersal depends entirely on execution speed and private key security. CiaoTool builds an ultra-secure on-chain operational defense for professional teams:

* **Maximum Cost Reduction** By utilizing smart contract multi-calls and batch-bundling tech, multiple transfers are aggregated into a single on-chain interaction. This minimizes network fees and significantly cuts funding overhead during large-scale distributions.
* **Local Security Environment** Operating via a pure client-side architecture, private keys never leave your machine and are used solely for local transaction signing. This maximizes execution efficiency while ensuring the absolute security of your multi-wallet assets.

***

## **Step by Step** <a href="#solana-one-to-multi-guide" id="solana-one-to-multi-guide"></a>

{% stepper %}
{% step %}
### Switch Chain & Connect Wallet <a href="#switch-chain-and-connect-wallet" id="switch-chain-and-connect-wallet"></a>

Select your target blockchain and connect an EVM-compatible wallet.

<figure><img src="../../.gitbook/assets/image (938).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select Transfer Token

You can select BNB or choose any token currently held in your wallet to execute the multi-transfer.

<figure><img src="../../.gitbook/assets/image (939).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Input Sender Wallet Private Key

{% hint style="danger" %}
Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../security-guide.md).
{% endhint %}

Supports two methods for importing sending private key: **"Manual Input"** and **"Upload File"**. Select an option to view the detailed tutorial.

{% tabs %}
{% tab title="Manual Input" %}
Enter / batch paste wallet private keys, one address per line. Press Enter to start a new line.

<figure><img src="../../.gitbook/assets/image (922).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Click the "Upload File" button to open the file upload window.

<figure><img src="../../.gitbook/assets/image (920).png" alt=""><figcaption></figcaption></figure>

2. Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.   \
   Click to download and view the template:

{% file src="../../.gitbook/assets/EVM_privateKey_demo.xlsx" %}

<figure><img src="../../.gitbook/assets/image (921).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Enter Number of Fragmentation Wallet

Enter the number of destination addresses to fragment each wallet into. Each wallet will transfer its total specified tokens into this set number of wallets. A single address can be fragmented into a maximum of 200 new addresses.

Click **"Generate Wallet"** and the system will automatically download all newly generated fragmented addresses.

<figure><img src="../../.gitbook/assets/image (940).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Enter Transfer Amount

<figure><img src="../../.gitbook/assets/image (925).png" alt=""><figcaption></figcaption></figure>

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
### **Confirm**

Review transfer info and check status.

After verifying all details, click the **"Send"** button below and wait for the transaction process to complete.

<figure><img src="../../.gitbook/assets/image (926).png" alt=""><figcaption></figcaption></figure>
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

<summary><strong>Is It Secure?</strong></summary>

The platform uses a fully client-side signing mechanism. Your private key is never uploaded or stored on any server, and all transactions are signed locally in your browser, ensuring the platform cannot access your private key.

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
