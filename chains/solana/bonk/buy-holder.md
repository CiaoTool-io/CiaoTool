---
description: >-
  An automated new-wallet buying tool for Bonk.fun. Creates wallets and executes
  real purchases automatically. Helps increase holder count and improve token
  distribution.
---

# Bonk - Boost Holders Tutorial

{% hint style="info" %}
**CiaoTool Bonk Boost Makers** now fully supports all quote tokens, including official **SOL and USD1**. Please switch to the specific token page first to perform market management operations, meeting your rapid market-making service needs across various scenarios.
{% endhint %}

## What is CiaoTool Bonk Boost Holders?

<figure><img src="../../../.gitbook/assets/image (839).png" alt="CiaoTool Solana Toolkit Page about Bonk.fun Boost Holders Feature"><figcaption></figcaption></figure>

**CiaoTool Bonk Boost Holders** is an on-chain data and asset distribution optimization tool custom-built for the **Bonk.fun platform** within the Solana ecosystem. It allows users to automatically generate brand-new wallet addresses in batches through configured parameters and control these addresses to independently execute token buy operations on the order book.

Distinctly different from the mechanism of "Boost Makers," which consolidates funds and destroys accounts after trading, this feature permanently retains the purchased tokens within these newly generated independent addresses upon completion of the order book purchase. This not only generates authentic, natural buy records on the order book, but also directly increases the number of unique on-chain holding addresses for the token, thereby effectively dispersing chips and rendering the overall token distribution structure more even and healthy.

Start your Boost Holders on Bonk with CiaoTool now:

{% embed url="https://ciaotool.io/en-US/letsbonkZone/newaddr-buyers-holders" %}

***

## Why Choose CiaoTool Bonk Boost Holders?

CiaoTool provides a professional solution for optimizing holder data on the Bonk.fun platform, balancing authenticity with high execution efficiency. For users who need to perfect early chip distribution or steadily enhance the project's data health, this tool builds a robust automated defense:

* **Authentically Boost Holders:** Through a large number of new addresses executing genuine capital purchases on the order book and holding tokens independently, it steadily and authentically increases the total number of on-chain holding addresses.
* **Optimize Chip Distribution Structure:** By rationally dispersing purchased tokens across numerous completely independent wallets, it effectively avoids over-concentration of chips in a single address and beautifies the token distribution bubble map.
* **Fully Automated Closed-Loop Executio**n: With one click, it automatically completes the entire process of "generating addresses in batches, master wallet distributing SOL, and executing purchases independently," completely eliminating the tedious manual operations of individual creation and transfers.
* **Local Security and Data Export:** Utilizing a pure front-end local execution mechanism, all newly generated private keys run exclusively locally. The system supports a one-click export of the private key spreadsheet for all new addresses, facilitating convenient and secure management of dispersed assets for users in the future.

***

## What is the difference between "Boost Holders" and "Boost Makers"?

| Feature       | Metric Boosted                        | Optimization Focus                        |
| ------------- | ------------------------------------- | ----------------------------------------- |
| Boost Holders | Number of addresses holding the token | Consensus distribution, long-term holders |
| Boost Makers  | Number of addresses that have traded  | Activity, sense of market participation   |

***

## **Step by Step |** Bonk Boost Holders

{% stepper %}
{% step %}
### Connect Wallet

Click the button in the top right corner to connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image (836).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select a Token to trade

You can choose to enter the token address, or select a token currently owned by your wallet to perform the buy operation.

<figure><img src="../../../.gitbook/assets/image (828).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select Number of Buy Addresses

Choose or enter the number of buy addresses to increase the number of makers.

<figure><img src="../../../.gitbook/assets/image (829).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Enter Buy Amount

Set the amount each new wallet will spend on purchases. You can also define a range for randomized buy amounts within the specified limits.
{% endstep %}

{% step %}
### Generate Wallets and Download Private Key File

Unlike "Boost Makers," all wallets will retain tokens to maintain a token-holding status. To prevent any potential financial loss, please ensure that you download the private key file and safeguard it properly. This will allow you to continue using these wallets for subsequent operations such as market making, transfers, asset recovery, and account closure.
{% endstep %}

{% step %}
### Enter Main Wallet PrivateKey

{% hint style="danger" %}
<mark style="color:$danger;">**Security Tips**</mark>

Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

{% hint style="info" %}
<mark style="color:$primary;">**Main Wallet Settings**</mark>

On-chain fees generated by purchases, SOL account rent (automatically refunded), and platform service fees are all paid uniformly by the master wallet. An estimated required balance will be displayed at the bottom of the page. Please ensure that the master wallet balance is higher than the estimated amount, otherwise, it may result in transaction failure.

Each new address requires a payment of **0.00203928 SOL** for **SOL account rent**, which is automatically refunded to the master wallet once the transaction process is complete.
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (830).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Confirm

{% hint style="danger" %}
Closing / refreshing the page will **immediately stop** the bot strategy. Please ensure that the page remains open and running continuously in the background while the strategy is being executed. To ensure necessary strategy execution, **this feature is not recommended for use on mobile devices.**
{% endhint %}

After verifying all details, click the **"Start"** button below and wait for the transaction process to complete.
{% endstep %}
{% endstepper %}

***

## **FAQs**

<details>

<summary><strong>What is the Bonk Boost Holders feature?</strong></summary>

This is an on-chain data optimization tool. The system automatically creates a large number of brand-new wallet addresses, allocates the required funds to them, and executes token buy operations on the order book. The purchased tokens will be retained directly within these new addresses, primarily used to authentically increase the number of token holders and optimize chip distribution.

</details>

<details>

<summary><strong>What is the difference between this and transferring directly to multiple addresses in multisender (One-to-Multi Transfers)?</strong></summary>

Multisender (One-to-Multi Transfers) only generate simple token transfer records on-chain, which do not affect market prices or increase trading activity. Conversely, a "new address buy" executes authentic DEX transactions through each new wallet on the Raydium order book. This not only increases the number of holders, but also simultaneously boosts the total trading volume and the number of traders on the order book, providing a more comprehensive and natural approach to on-chain data optimization.

</details>

<details>

<summary><strong>Where do the private keys of the massive number of generated new addresses go? How do I manage these tokens in the future?</strong></summary>

Upon completion of the execution process, the system will generate a local spreadsheet file for you containing all the new addresses and their corresponding private keys. You can download this file with one click and safeguard it properly, allowing you to import it into CiaoTool's "MultiSender" or "Batch Consolidation" features at any time in the future for centralized management of these dispersed assets.

</details>

<details>

<summary><strong>Is the operation secure?</strong></summary>

CiaoTool uses a fully client-side signing mechanism. Your private key is never uploaded or stored on any server, and all transactions are signed locally in your browser. This ensures, at a technical level, that the platform has no access to your private key.

</details>

***

**Need help? Join our community for real-time support:**

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
