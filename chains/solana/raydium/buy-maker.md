---
description: >-
  An automated new-wallet buying tool for Raydium. Creates wallets, executes
  purchases, and recovers assets automatically. Helps increase unique buyers and
  improve market activity.
---

# Solana - Boost Makers Tutorial

{% hint style="info" %}
**CiaoTool Raydium Boost Makers** now fully supports all liquidity pool types, including **AMM, CLMM, and CPMM**. Please switch to the specific pool function page first to perform market making operations.
{% endhint %}

## Waht is CiaoTool Solana Boost Makers?

<figure><img src="../../../.gitbook/assets/image (827).png" alt="CiaoTool Solana Toolkit Page about Raydium Boost Makers Feature"><figcaption></figcaption></figure>

**CiaoTool Solana Boost Makers** is an on-chain data optimization and automated execution tool custom-built for the **Raydium platform** within the Solana ecosystem. It is designed to help users rapidly increase the number of unique purchasing wallets for a designated token with ultra-low capital attrition.

The core mechanism of this feature lies in a complete "fully automated execution closed-loop": the system automatically creates brand-new wallet addresses in batches at the underlying level, and controls these new addresses to execute token buy operations on the order book. Upon completion of the purchase interaction, the system automatically and securely transfers the purchased tokens along with the remaining funds into a master wallet specified by the user, while synchronously sending commands to the Solana network to close these temporary accounts. This mechanism not only leaves authentic new address purchase records on-chain, but also reclaims on-chain rent by destroying the accounts, thereby making the project's activity data stand out in the market at an ultra-low cost.

Start your Boost Makers on Raydium with CiaoTool now:

{% embed url="https://ciaotool.io/en-US/raydium/newaddr-buyers-markers" %}

***

## Why Choose CiaoTool Solana Boost Makers?

CiaoTool provides a professional solution for data optimization on the Raydium platform, balancing ultra-low costs with high execution efficiency. For users who need to rapidly increase active buyer metrics on the order book, this tool builds a robust automated defense:

* **Fully Automated Closed-Loop Execution:** With one click, it automatically completes the entire process of "generating new addresses, executing purchases, consolidating assets, and closing accounts," completely eliminating tedious manual address management and funds collection operations.
* **Ultra-Low Cost to Boost Makers:** Through the underlying mechanism of closing temporary accounts immediately after execution, it effectively reclaims account rent on the Solana chain, rapidly increasing the number of unique buyers with ultra-low capital consumption.
* **Optimize Market Data Performance:** Through massive authentic new address purchase interactions, it significantly boosts the active trader metrics of tokens on various market tracking platforms, improving market data presentation.
* **Secure Local Environment:** Utilizing a pure front-end local execution mechanism, all temporarily generated private keys and the master wallet private key are used exclusively within the local environment for transaction signing, comprehensively guaranteeing the absolute security of consolidated assets.

***

## What is the difference between "Boost Makers" and "Boost Holders"?

| Feature       | Metric Boosted                        | Optimization Focus                        |
| ------------- | ------------------------------------- | ----------------------------------------- |
| Boost Makers  | Number of addresses that have traded  | Activity, sense of market participation   |
| Boost Holders | Number of addresses holding the token | Consensus distribution, long-term holders |

***

## **Step by Step |** Solana **Boost Makers**

{% stepper %}
{% step %}
### Connect Wallet

Click the button in the top right corner to connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image (17).png" alt=""><figcaption></figcaption></figure>
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

<summary><strong>What is the Solana Boost Makers feature?</strong></summary>

Boost Makers is an automated on-chain optimization tool that creates new wallet addresses to purchase tokens automatically. After the purchase is completed, assets are transferred back to a designated main wallet and the temporary wallets are closed. Its primary purpose is to increase the number of unique buyers.

</details>

<details>

<summary><strong>Why Close the Wallets?</strong></summary>

On Solana, creating token accounts requires a small amount of SOL as rent. After the purchase and asset consolidation are completed, the tool automatically closes the temporary accounts and reclaims the rent deposit. This helps minimize the overall cost of increasing unique buyers.

</details>

<details>

<summary><strong>Where Do the Purchased Tokens Go?</strong></summary>

Your assets are never lost. After each purchase, the tool automatically transfers the acquired tokens from the temporary wallets to your designated main wallet for centralized management.

</details>

<details>

<summary><strong>How Is Boost Makers Different from a Regular Buy?</strong></summary>

A regular purchase is typically made from an existing wallet with transaction history, making fund flows and holdings easy to track on-chain.

Boost Makers uses newly generated wallets to execute purchases. These wallets appear as independent participants on-chain and have no prior transaction history. This approach helps diversify buyer activity, improve buyer metrics, and streamline liquidity management workflows.

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
