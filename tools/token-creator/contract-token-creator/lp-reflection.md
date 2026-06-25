---
description: >-
  Deploy a BEP-20 liquidity reward token with one click. Customize tax rates and
  automatically reward liquidity providers, helping build deeper liquidity and
  sustainable tokenomics.
---

# BSC - LP Reflection Token Creator Tutorial

{% hint style="danger" %}
<mark style="color:red;">**Security Alert**</mark>

This token type contains custom logic that **may be flagged** by certain audit platforms. For 100% flawless green scores, please choose [**"Standard Token"**](standard-token-evm.md). By proceeding with this deployment, **you acknowledge and accept that such security alerts or risk flags may appear.**
{% endhint %}

## What is CiaoTool BSC LP Reflection Token Creator?

<figure><picture><source srcset="../../../.gitbook/assets/屏幕截图 2026-06-16 172014.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (12).png" alt="CiaoTool BSC Toolkit Page about BSC LP Reflection Token Creator Feature"></picture><figcaption></figcaption></figure>

**CiaoTool BSC LP Reflection Token Creator** is an advanced smart contract deployment workbench specifically engineered to resolve the pain point of a "liquidity crunch" for Web3 projects. Breaking through the bottlenecks of complex contract development, it empowers project founders to ultra-fast launch BEP-20 protocol tokens equipped with an exclusive LP reward pool on the BNB Chain.

Unlike standard holding reflections, this feature uniquely rewards liquidity providers. Upon any on-chain trade, the smart contract automatically levies a tax and—within the exact same block—routes the reflections to all active LP addresses based on their liquidity provisioning weight on PancakeSwap.

| Dimension              | Holders Reflection Token                                       | LP Reflection Token                                                                        |
| ---------------------- | -------------------------------------------------------------- | ------------------------------------------------------------------------------------------ |
| Target Recipients      | Anyone holding the token in their wallet.                      | Exclusively those who provide liquidity (LPs) on the exchange.                             |
| Project Benefits       | Incentivizes a "buy-and-hold" mentality among users.           | Significantly thickens liquidity pool depth, curbing violent price volatility.             |
| User Yield Sources     | Passively receiving reflections generated from trading volume. | Earns dual yields: standard DEX swap fees plus automated smart contract token reflections. |
| Price Floor Resilience | Moderate.                                                      | Powerful.                                                                                  |

Start your LP Reflection Token Creator on BNB Smart Chain with CiaoTool now:

{% embed url="https://bsc.ciaotool.io/en/token/lp-reflection" %}

***

## Why Choose CiaoTool BSC LP Reflection Token Creator?

CiaoTool delivers a professional asset issuance solution on the BNB Chain that perfectly balances absolute security with streamlined operations. For users seeking rapid deployment of pure tokens, this tool establishes a highly efficient and robust execution standard:

* **Flexible Taxes**\
  Customizable buy/sell taxes with flexible options for LP reflection, marketing cut, or burn to suit any trading strategy.
* **No-Code**\
  Form-based deployment with no coding or debugging. Confirm Gas to launch your LP reflection token instantly.
* **Trust & Control**\
  Supports permanently renouncing sensitive modules post-launch to boost community and holder confidence.
* **Ecosystem**\
  Direct access to MM & liquidity tools, bridging the full lifecycle from creation to operation.

***

## **Step by Step**

{% stepper %}
{% step %}
### **Connect Wallet**

Click the button in the top right corner to connect a wallet that supports the EVM network.

<figure><img src="../../../.gitbook/assets/image (960).png" alt=""><figcaption></figcaption></figure>
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
### Function Setup

All of the following functions can be managed by adjusting parameters via the Console, or their administrative permissions can be permanently renounced.

1.  **Manual Trading Enable**

    The initial trading session after adding liquidity must be activated manually via the dashboard console.
2.  **Anti-Bot Blocks**

    Automatically blacklists all addresses that execute transactions within the first "n" blocks after trading goes live. Designed to prevent front-running sniper bots, this feature requires trading to be enabled manually.

<figure><img src="../../../.gitbook/assets/image (961).png" alt=""><figcaption></figcaption></figure>

3. **Tax Switch**\
   Buy and sell tax rates can be manually adjusted at any time post-creation. However, both individual buy and sell taxes must strictly adhere to the range of 0% to 25%.
4. **Auto Airdrop**\
   Automatically airdrops a microscopic amount of tokens to up to 5 random addresses upon every transaction, organically expanding the project's total holder count.
5. **Blacklist**\
   Enables blocking specific wallet addresses from trading or transferring tokens. Once this module is turned off, it is permanently renounced and cannot be reactivated.
6. **Max Holding**\
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

<summary><strong>How do I choose the dividend token?</strong></summary>

When creating your token, you can select major crypto assets (such as WBNB, USDT, USDC, or DOGE) as the reward token. The chosen asset must establish an active trading pair with BNB and possess sufficient liquidity.

</details>

<details>

<summary><strong>How can users ensure they qualify for and receive reflections?</strong></summary>

Users must actively provide liquidity (add LP) and trade. Merely receiving LP tokens via transfer or executing single-sided buys will not activate reflections.

</details>

<details>

<summary><strong>Why are there still no reflections after making multiple purchases?</strong></summary>

1. Avoid trading with tax-exempt whitelisted wallets (deployer/marketing).&#x20;
2. The contract relies on a "buy-and-sell" tax cycle; a market sell order must occur to trigger the reflection payout.

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
