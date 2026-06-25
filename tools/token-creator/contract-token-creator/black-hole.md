---
description: >-
  CiaoTool provides no-code deployment for BSC blackhole reward tokens. Combine
  holder rewards and automatic burns in a single BEP-20 token to build a
  deflationary token model.
---

# BSC - Burning Reflection Token Creator Tutorial

{% hint style="danger" %}
<mark style="color:red;">**Security Alert**</mark>

This token type contains custom logic that **may be flagged** by certain audit platforms. For 100% flawless green scores, please choose [**"Standard Token"**](standard-token-evm.md). By proceeding with this deployment, **you acknowledge and accept that such security alerts or risk flags may appear.**
{% endhint %}

## What is BSC Burning Reflection Token Creator?

<figure><picture><source srcset="../../../.gitbook/assets/屏幕截图 2026-06-17 141353.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (971).png" alt="CiaoTool BSC Toolkit Page about BSC Burning Reflection Token Creator Feature"></picture><figcaption></figcaption></figure>

The core of this feature lies in the introduction of a tokenomics innovation called "Burn-to-Earn": once the token is deployed, the system automatically opens a dividend pool. Standard token holders cannot directly earn yields; users must actively transfer their project tokens to the black hole address (permanent destruction) to activate and qualify for reflections.&#x20;

Meanwhile, when creating the contract, project owners can freely designate the specific asset type distributed by the dividend pool.

This mechanism drives holders into a strategic game between "holding to wait for appreciation" and "burning to exchange for stable cash flow," thereby achieving an ultra-fast, permanent reduction in circulating supply.

{% hint style="info" %}
Blackhole Address: `0x000000000000000000000000000000000000dEaD`
{% endhint %}

Use Case:

* **Hyper-Scarcity:**  Rewards token-burning to rapidly and permanently reduce circulating market supply.
* **Token Synergy:** Distributes USDT, BNB, or ecosystem assets to drive dual-token synergy.

| Dimension                 | Holders Dividend Token                                | Burning Reflection Token                                                       |
| ------------------------- | ----------------------------------------------------- | ------------------------------------------------------------------------------ |
| Eligibility Condition     | Simply holding the token in the wallet is sufficient. | Must actively transfer the token to the black hole address for destruction.    |
| Yield Asset Type          | Typically rewards the project token itself.           | Can customize rewards to be any on-chain token.                                |
| Circulating Supply Impact | Unchanged; it merely transfers between user wallets.  | Decreases; users will actively eliminate circulating supply to secure profits. |
| User Game Psychology      | Passively waiting for transaction tax yields.         | 主动出击，权衡“卖出赚差价”还是“销毁拿永续分红”                                                      |

Start your Burning Reflection Token Creator on BNB Smart Chain with CiaoTool now:

{% embed url="https://bsc.ciaotool.io/en/token/black-hole" %}

***

## Why choode CiaoTool BSC Burning Reflection Token Creatoe

CiaoTool delivers a secure, streamlined asset issuance solution on the BNB Chain, providing highly efficient infrastructure for complex on-chain cross-asset routing:

* **Flexible Taxes**\
  Custom buy/sell taxes with flexible rewards and parameter settings for any economic model.
* **No-Code**\
  Form-based deployment without coding or debugging; confirm Gas to issue tokens instantly.
* **Ecosystem**\
  Direct access to MM & liquidity tools, bridging the full lifecycle from creation to operation.

***

## **Step by Step**

{% stepper %}
{% step %}
### **Connect Wallet**

Click the button in the top right corner to connect a wallet that supports the EVM network.

<figure><img src="../../../.gitbook/assets/image (972).png" alt=""><figcaption></figcaption></figure>
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
### Choose Dividends Token

<figure><img src="../../../.gitbook/assets/image (970).png" alt=""><figcaption></figcaption></figure>

Select or enter the token contract address you wish to distribute as dividend.

**The selected dividend token must possess an active BNB trading pair and be fully tradeable.** If the token suffers from insufficient liquidity or lacks a BNB paired pool, the automated reflection mechanism may fail to execute. Major assets are highly recommended.
{% endstep %}

{% step %}
### Set Buy/Sell Tax Rates

{% hint style="info" %}
Individual tax rate cannot exceed 25%.

Combined buy and sell tax rates cannot exceed 50%.
{% endhint %}

CiaoTool features a dual-tax framework for transaction friction. You can flexibly customize individual tax rates for both buy and sell orders.

<figure><img src="../../../.gitbook/assets/image (973).png" alt=""><figcaption></figcaption></figure>

* **Fund Fee:** Auto-transfers a fixed rate of tokens to the fund address for project promotion.
* **Reflect Fee:** Distributes tax allocations to all LP token holders based on ownership percentages.
* **LP Fee:** Automatically injects a portion of tokens into the pool to sustain deep trading liquidity.
{% endstep %}

{% step %}
### Initial Liquidity Setup

<figure><img src="../../../.gitbook/assets/image (957).png" alt=""><figcaption></figcaption></figure>

When initially creating the liquidity pool, you must complete the initial setup to activate the native token reflection mechanism.

* **Target DEX:** PancakeSwap (Currently the only supported platform on BSC)
* **Currency:** The asset paired with your new token, typically using major tokens like BNB or USDT.
{% endstep %}

{% step %}
### Function Setup

All of the following functions can be managed by adjusting parameters via the Console, or their administrative permissions can be permanently renounced.

1.  **Manual Trading Enable**

    The initial trading session after adding liquidity must be activated manually via the dashboard console.
2. **Tax Switch**\
   Buy and sell tax rates can be manually adjusted at any time post-creation. However, both individual buy and sell taxes must strictly adhere to the range of 0% to 25%.
3. **Blacklist**\
   Enables blocking specific wallet addresses from trading or transferring tokens. Once this module is turned off, it is permanently renounced and cannot be reactivated.
4. **Max Holding**\
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

<summary><strong>Do all black hole addresses unlock reflect?</strong></summary>

No. Currently, only one specific black hole address is supported, which is: `0x000000000000000000000000000000000000dEaD`. The other black hole address does not support dividend eligibility.

</details>

<details>

<summary><strong>Why are there still no reflections after making multiple purchases?</strong></summary>

1. Avoid trading with tax-exempt whitelisted wallets (deployer/marketing).&#x20;
2. The contract relies on a "buy-and-sell" tax cycle; a market sell order must occur to trigger the reflection payout.

</details>

<details>

<summary><strong>Can the black hole dividend threshold value be modified?</strong></summary>

No, this value is immutable even with permissions. It must be set correctly during creation.

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
