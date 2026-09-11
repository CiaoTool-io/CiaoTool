---
description: >-
  An automated new-wallet buying tool for Bonk.fun. Creates wallets, executes
  purchases, and recovers assets automatically. Helps increase unique buyers and
  improve market activity.
---

# Bonk - Boost Makers Guide

{% hint style="info" %}
**CiaoTool Bonk Boost Makers** now fully supports all quote tokens, including official **SOL and USD1**.
{% endhint %}

## Overview

**CiaoTool Bonk Trader Booster** is a multi-address automated trading tool for Bonk.fun. It generates new wallets in batches and uses them to purchase a specified token.

The system automatically completes the entire process: wallet creation, fund distribution, token purchase, asset consolidation, and account cleanup. After trading, the purchased tokens and remaining SOL are transferred to a designated main wallet. Eligible temporary Token Accounts are then closed, and their recoverable account rent is refunded.

Start your Boost Makers on Bonk with CiaoTool now:

{% embed url="https://ciaotool.io/en/bonk/newaddr-buyers-markers" %}

***

## Advantage

* **End-to-End Automation:** Completes wallet creation, fund distribution, purchasing, consolidation, and account cleanup in one workflow
* **Batch Address Interaction:** Enables multiple new wallets to complete on-chain purchases
* **Lower Account Costs:** Closes zero-balance temporary Token Accounts and recovers refundable rent
* **Centralized Asset Consolidation:** Transfers purchased tokens and remaining funds to a designated wallet
* **Trackable Process:** Displays transaction status, purchase results, and consolidation records for each address
* **Local Signing:** Temporary and main wallet private keys are used only for transaction authorization within the browser

***

## What is the difference between "Boost Makers" and "Boost Holders"?

| Feature       | Metric Boosted                        | Optimization Focus                        |
| ------------- | ------------------------------------- | ----------------------------------------- |
| Boost Makers  | Number of addresses that have traded  | Activity, sense of market participation   |
| Boost Holders | Number of addresses holding the token | Consensus distribution, long-term holders |

***

## Step by Step

{% stepper %}
{% step %}
### Connect Wallet

Click the button in the top right corner, and connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select Token Pair

Enter a token address or select a token held by the connected wallet.

* **Project Token:** The token used to execute the market-making strategy.
* **Quote Token:** The token used to pay for transactions and quote the trading pair price.

<figure><img src="../../../.gitbook/assets/image (1202).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Buy Funding Wallet

{% hint style="danger" %}
Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

The **Main Wallet** pays all on-chain fees, refundable SOL account rent, and platform service fees. Ensure its balance exceeds the estimated fee shown on the page to avoid execution failure.

Each new address requires **0.00203928 SOL** in account rent, which will be automatically returned to the Main Wallet after completion.
{% endstep %}

{% step %}
### Generate and Buy Amount

{% hint style="danger" %}
**Download Wallets**

Please download and securely save the newly generated wallet information to prevent asset loss if the network disconnects or the page closes.
{% endhint %}

#### Number of New Addresses

Generate the specified number of new wallets and execute purchases to increase the number of traders.

#### Trade Amount

Set the purchase amount for each new wallet:

* **Fixed Amount:** All new wallets buy the token with the specified amount.
* **Random Amount:** Each new wallet buys the token with a random amount within the specified range.

#### Trade Interval

Set the transaction interval for new addresses:

* **Fixed Interval:** Transactions are submitted at a fixed interval.
* **Random Interval:** Transactions are submitted randomly within the specified time range.
{% endstep %}

{% step %}
### Confirm

The program runs automatically. Review the following on the confirmation page:

* [x] Number of new addresses
* [x] Purchase amount
* [x] Estimated fees

<figure><img src="../../../.gitbook/assets/image (1187).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Start Trade

{% hint style="danger" %}
Closing or refreshing the page will **stop the bot immediately**. Keep the page open and running in the background while the strategy is active. This feature is **not recommended for mobile devices**.
{% endhint %}

Each wallet pays its own transaction fees. After confirming the details, click **“Confirm”** to launch the trading program.
{% endstep %}
{% endstepper %}

***

## **FAQs**

<details>

<summary><strong>What is the Bonk Boost Makers feature?</strong></summary>

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

## Service Support

Need help? Join our community for real-time support:

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
