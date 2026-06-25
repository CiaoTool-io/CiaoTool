---
description: >-
  CiaoTool provides no-code deployment for BSC reward tokens. Customize buy and
  sell tax rates and enable automatic on-chain rewards with one click. Secure
  and easy to use.
---

# BSC - Holders Dividend Token Creator Tutorial

{% hint style="danger" %}
<mark style="color:red;">**Security Alert**</mark>

This token type contains custom logic that **may be flagged** by certain audit platforms. For 100% flawless green scores, please choose [**"Standard Token"**](standard-token-evm.md). By proceeding with this deployment, **you acknowledge and accept that such security alerts or risk flags may appear.**
{% endhint %}

## What is CiaoTool BSC Holders Dividend Token Creator?

<figure><picture><source srcset="../../../.gitbook/assets/屏幕截图 2026-06-16 143130.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (952).png" alt="CiaoTool BSC Toolkit Page about BSC Holders Dividend Token Creator Feature"></picture><figcaption></figcaption></figure>

**CiaoTool BSC Holders Reflection Token Creator** is an advanced smart contract deployment workbench custom-built for Web3 communities, DAOs, and project founders. Breaking the constraints of complex code development, it empowers users to ultra-fast launch BEP-20 tokens featuring built-in transaction tax and automated reflection mechanisms via a fully front-end visual dashboard.

Historically, implementing a "trade-to-reward" feature required writing highly intricate low-level code. Today, CiaoTool simplifies these logics into an intuitive, form-based setup. The token you deploy comes with a built-in "revenue-sharing" infrastructure: whenever a buy or sell transaction occurs in the market, the system automatically levies a small transaction fee (at a percentage customized by you), converts these fees into tokens, and instantly distributes them to all existing holders.

By shifting economic incentives, this model is naturally optimized for Web3 use cases that demand high community consensus and low user churn:

* **High-Consensus Tokenomics**\
  It heavily incentivizes a "buy-and-hold" mentality, creating transaction friction through customizable taxes to curb sandwich attacks and high-frequency trading bot arbitrage.
* **Community Incentive Infrastructure**\
  It supersedes traditional, friction-heavy "manual airdrop campaigns" with a perpetual, fully automated on-chain reward stream.
* **Project Growth & Self-Sustenance:**\
  It supports allocating a portion of the transaction tax to a dedicated marketing wallet via auto-backflow, generating a continuous treasury stream to fund long-term development.

Start your Holders Dividend Token Creator on BNB Smart Chain with CiaoTool now:

{% embed url="https://bsc.ciaotool.io/en/token/holders-dividend" %}

***

## Why Choose CiaoTool BSC Holders Reflection Token Creator?

Balancing security and simplicity, CiaoTool sets an efficient and robust professional standard for BSC token deployment.

* **Flexible Taxes**\
  Customizable buy/sell taxes with flexible options for reflection, marketing cut, or burn to suit any trading strategy.
* **No-Code**\
  Form-based deployment with no coding or debugging. Confirm Gas to launch your token instantly.
* **Pure Contract**\
  Zero risky modules like mint or blacklist. Streamlined logic ensuring optimal compliance in security audits.
* **Ecosystem**\
  Direct access to MM & liquidity tools, bridging the full lifecycle from creation to operation.

***

## Video Tutorial

{% embed url="https://www.youtube.com/watch?t=4s&v=c-ri6q-lWJ0" %}

***

## **Step by Step**

{% stepper %}
{% step %}
### Connect Wallet

Click the button in the top right corner to connect a wallet that supports the EVM network.

<figure><img src="../../../.gitbook/assets/image (953).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Enter Token Information

<figure><img src="../../../.gitbook/assets/image (954).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
<mark style="color:$primary;">**LOGO & Project Description**</mark>

LOGO and descriptions are off-chain by default on EVM. You must manually apply to DeFi platforms/wallets for display, or [contact us to get a tailored service quote](https://t.me/CiaoTools).
{% endhint %}

* **Token Name:** The full name of the token as you wish it to be displayed in wallets or block explorers (e.g., MyFirstToken).
* **Token Symbol:** The abbreviation of the token, typically 3 to 6 uppercase letters (e.g., MYT).
* **Decimals:** Refers to the minimum number of decimal places a token can be divided into. The most common choice is 12.
* **Total Supply:** The total volume of tokens to be issued.
{% endstep %}

{% step %}
### Receiving Wallet Address

Enter wallet address to receive total supply. This action transfers full token ownership and the total minted supply directly to the specified address.
{% endstep %}

{% step %}
### Set Buy/Sell Tax Rates

{% hint style="info" %}
Individual tax rate cannot exceed 25%.

Combined buy and sell tax rates cannot exceed 50%.
{% endhint %}

CiaoTool features a dual-tax framework for transaction friction. You can flexibly customize individual tax rates for both buy and sell orders.

<figure><img src="../../../.gitbook/assets/image (956).png" alt=""><figcaption></figcaption></figure>

* **Fund Fee:** Auto-transfers a fixed rate of tokens to the fund address for project promotion.
* **Reflect Fee:** Distributes tax allocations to all LP token holders based on ownership percentages.
* **Burn Fee:** Distributes tax allocations to all LP token holders based on ownership percentages.
* **LP Fee:** Automatically injects a portion of tokens into the pool to sustain deep trading liquidity.
* **Fund Address:** The designated wallet address used to collect marketing tax allocations from transactions.
{% endstep %}

{% step %}
### Initial Liquidity Setup

<figure><img src="../../../.gitbook/assets/image (957).png" alt=""><figcaption></figcaption></figure>

When initially creating the liquidity pool, you must complete the initial setup to activate the native token reflection mechanism.

* **Target DEX:** PancakeSwap (Currently the only supported platform on BSC)
* **Currency:** The asset paired with your new token, typically using major tokens like BNB or USDT.
{% endstep %}

{% step %}
### Confirm

After verifying all details, click the **"Create Contract"** button below and wait for the transaction process to complete.
{% endstep %}

{% step %}
### Add Token to Wallet dApps

If your token doesn't show up automatically, simply copy the contract address and use the "Import / Add Custom Token" feature in your wallet.

<details>

<summary><strong>Add Tutorial</strong></summary>

1. Open your wallet (browser extension or mobile app).
2. Navigate to the tokens tab and select "Import Tokens" (or "Add Token").

<figure><img src="../../../.gitbook/assets/image (948).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (949).png" alt=""><figcaption></figcaption></figure>

3. Ensure you are on the network where the token was deployed. Choose "Custom Crypto" from the import options.

<figure><img src="../../../.gitbook/assets/image (950).png" alt=""><figcaption></figcaption></figure>

4. Paste your token contract address to autofill the token details, then click "Import" to finish.

<figure><img src="../../../.gitbook/assets/image (951).png" alt=""><figcaption></figcaption></figure>

</details>
{% endstep %}

{% step %}
### Create Liquidity Pool

{% hint style="danger" %}
The initial asset pool must be created as a **"V2" Liquidity Pool**. Please note that "V3" liquidity pools are incompatible with and cannot trigger any tax or reflection mechanisms.
{% endhint %}

Once created, your token only supports basic transfers and cannot be traded yet. To enable market trading, you must Add a Liquidity Pool (LP), allowing users to swap your token freely on decentralized exchanges (DEXs).

Click here to view the Liquidity Pool Creation Tutorial:

<table data-card-size="large" data-view="cards"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td>Create Liquidity Pool - V2</td><td><a href="../../../chains/bsc/swap/create-liquidity-v2.md">create-liquidity-v2.md</a></td></tr><tr><td><a data-footnote-ref href="#user-content-fn-1">Liquidity Bundler</a> - V2</td><td><a href="../../../chains/bsc/swap/bundler-v2.md">bundler-v2.md</a></td></tr><tr><td>Create Liquidity Pool - V3</td><td><a href="../../../chains/bsc/swap/create-liquidity-v3.md">create-liquidity-v3.md</a></td></tr><tr><td><a data-footnote-ref href="#user-content-fn-1">Liquidity Bundler</a> - V3</td><td><a href="../../../chains/bsc/swap/bundler-v3.md">bundler-v3.md</a></td></tr></tbody></table>
{% endstep %}
{% endstepper %}

***

## **FAQs**

<details>

<summary><strong>Can I modify the parameters after the token is deployed?</strong></summary>

No. The total supply and token decimals are permanently immutable once deployed. If you need to make changes, you will have to create and deploy a new token.

</details>

<details>

<summary><strong>Can I use Chinese characters for the Token Name and Symbol?</strong></summary>

Yes. The BNB Smart Chain (BSC) fully supports Chinese, English, and mixed alphanumeric characters for token metadata.

</details>

<details>

<summary><strong>Is It Secure?</strong></summary>

The platform uses a fully client-side signing mechanism. Your private key is never uploaded or stored on any server, and all transactions are signed locally in your browser, ensuring the platform cannot access your private key.

</details>

***

**Need help? Join our community for real-time support:**

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}

[^1]: Create Liquidity Pool & Multi-Address Bundled Buy
