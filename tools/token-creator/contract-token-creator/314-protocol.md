---
description: >-
  CiaoTool provides no-code deployment for BSC ERC-314 tokens. Trade directly
  through transfers without swaps, with built-in cooldown protection for a
  seamless token launch experience.
---

# BSC - ERC-314 Token Creator Tutorial

{% hint style="danger" %}
<mark style="color:red;">**Security Alert**</mark>

This token type contains custom logic that **may be flagged** by certain audit platforms. For 100% flawless green scores, please choose [**"Standard Token"**](standard-token-evm.md). By proceeding with this deployment, **you acknowledge and accept that such security alerts or risk flags may appear.**
{% endhint %}

## What is ERC-314 Token Creator?

<figure><picture><source srcset="../../../.gitbook/assets/屏幕截图 2026-06-17 113111.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (966).png" alt="CiaoTool BSC Toolkit Page about BSC ERC-314 Token Creator Feature"></picture><figcaption></figcaption></figure>

{% hint style="warning" %}
ERC-314 Token is experimental and carries unexpected risks. Permissions are critical. Please double-check before proceeding.
{% endhint %}

ERC-314 Token is a new, experimental token standard designed to reduce high transaction fees and cumbersome approval processes for users. Unlike traditional Swaps, the 314 Protocol enables a novel functionality of "transferring as trading."

* **Buying Tokens:** Users can obtain tokens simply by transferring BNB into the contract address.
* **Selling Tokens:** Users can obtain BNB simply by transferring tokens into the contract address.
* **Trading Cooldown:** Within a designated timeframe, only a single buy order is permitted across the entire market, and only a single sell order is permitted per address.

Start your ERC-314 Token Creator on BNB Smart Chain with CiaoTool now:

{% embed url="https://bsc.ciaotool.io/en/token/314-protocol" %}

***

## Why Choose CiaoTool BSC 314 Protocol Token Creator?

For project teams pursuing technological innovation and paramount security, CiaoTool constructs the most efficient implementation pathway:

* **No-Code**\
  Form-based deployment with no coding or debugging. Confirm Gas to launch your 314 token instantly.
* **Ecosystem**\
  Direct access to MM & liquidity tools, bridging the full lifecycle from creation to operation.

***

## **Step by Step**

{% stepper %}
{% step %}
### **Connect Wallet**

Click the button in the top right corner to connect a wallet that supports the EVM network.

<figure><img src="../../../.gitbook/assets/image (963).png" alt=""><figcaption></figcaption></figure>
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
### 314 Settings

<figure><img src="../../../.gitbook/assets/image (967).png" alt=""><figcaption></figcaption></figure>

* **Liquidity Ratio:** The percentage of tokens automatically transferred to the contract address during token creation, used to provide liquidity.
* **Cooldown:** The interval time between each buy order, and the individual interval time for each sell order.
{% endstep %}

{% step %}
### Set Buy/Sell Tax Rates

{% hint style="info" %}
Individual tax rate cannot exceed 25%.

Combined buy and sell tax rates cannot exceed 50%.
{% endhint %}

CiaoTool features a dual-tax framework for transaction friction. You can flexibly customize individual tax rates for both buy and sell orders.

<figure><img src="../../../.gitbook/assets/image (968).png" alt=""><figcaption></figcaption></figure>

* **Fund Fee:** A specified portion of tokens in each tradewill be automatically transferred to the marketing walletfor project promotion and other marketing activities.
* **Burn fee:** A specified portion of tokens in each trade willbe sent to a burn (black hole) address, effectively creatinga deflationary mechanism.
* **Fund Address:** The designated wallet address used to collect marketing tax allocations from transactions.
{% endstep %}

{% step %}
### Function Setup

All of the following functions can be managed by adjusting parameters via the Console, or their administrative permissions can be permanently renounced.

1. **Max Holding**\
   Allows you to cap the maximum number of tokens a single wallet can hold (Anti-Whale). Once this toggle is disabled, it is permanently locked and cannot be enabled again.
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
Creating a liquidity pool **is not recommended**. This token still has many restrictive conditions and lacks tax functionality, and creating a liquidity pool only supports BNB.

Meanwhile, a single token will form two pools (DEX pool and the transfer pool) and two different prices, making it highly vulnerable to arbitrage trading.
{% endhint %}

Although 314 Protocol tokens can directly achieve buying and selling operations through the form of transfers, you can still choose to create a V2 liquidity pool paired with BNB, allowing your token to be displayed and traded on decentralized exchanges.

Click here to view the Liquidity Pool Creation Tutorial:

<table data-card-size="large" data-view="cards"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td>Create Liquidity Pool - V2</td><td><a href="../../../chains/bsc/swap/create-liquidity-v2.md">create-liquidity-v2.md</a></td></tr><tr><td><a data-footnote-ref href="#user-content-fn-1">Liquidity Bundler</a> - V2</td><td><a href="../../../chains/bsc/swap/bundler-v2.md">bundler-v2.md</a></td></tr></tbody></table>
{% endstep %}
{% endstepper %}

***

## **FAQs**

<details>

<summary><strong>Why did Multisender fail?</strong></summary>

Before performing a multisender, you must ensure that the multisender contract address is included in both the "trading cooldown whitelist" and the "holding whitelist" to successfully achieve batch transfers.

Multisender Contract Address: `0x7FF7E8Bb75De25d411Df3940eb96400d234cd62e`

</details>

<details>

<summary><strong>How does the trading cooldown take effect?</strong></summary>

The trading cooldown restricts the number of buy orders across the entire network and sell orders per address within the set timeframe. During the cooldown period, other users cannot buy, and a single address can only sell once. Normal trading will only resume after the cooldown time ends.

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
