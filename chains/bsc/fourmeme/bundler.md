---
description: >-
  A token launch and bundle buy tool for Four.meme. Create tokens, execute
  multi-wallet buys, and snipe migration liquidity in the same block to optimize
  holder distribution and build positions.
---

# Fourmeme - Bundler Guide (Create & Buy)

{% hint style="info" %}
**CiaoTool Fourmeme Bundler** fully supports all quote tokens, including **BNB, USD1, UUSD and all RWA tokens**. Please switch to the specific token page to perform token launch operations based on your needs.&#x20;
{% endhint %}

## Overview

**CiaoTool Fourmeme Bundler** is an automated token launch and position-building tool designed for Four.meme on BSC. It covers both stages of the launch process—from token creation and bonding-curve buys to post-migration purchases—reducing manual work and waiting time between stages.

The full process consists of two separate bundles:

* **Token Creation & Bonding Curve Buys:** The token creation transaction and buys from multiple wallets are bundled in a predefined order and, under normal conditions, executed consecutively within the same block.
* **Migration & DEX Buys:** Once the token meets the graduation requirements, the migration to PancakeSwap and buys from multiple wallets are packaged into a new bundle and, under normal conditions, executed sequentially within the same block.

Start Create and Buy Token on Fourmeme with CiaoTool now:

{% embed url="https://bsc.ciaotool.io/en/fourmeme/bnb/create-and-buy" %}

***

## Advantage

CiaoTool provides a secure and efficient launch solution for Four.meme tokens, helping users optimize early token distribution and streamline the launch process.

* **Create and Buy in One Flow:** Configure your token details and the buy amount for each wallet in one setup.
* **Open Mode Support:** Exclusive support for the latest OpenFour templates, giving you more launch options.
* **Tax Token Support:** Create tax-enabled tokens and build tokenomics tailored to your project.
* **DEX Sniping:** Optionally fill the bonding curve at launch, then use multiple wallets to snipe the external pool as the token migrates.
* **Multi-Wallet Setup:** Choose the participating wallets and configure a separate buy amount for each one.
* **Automated Execution:** Automates data submission, transaction building, wallet signing, and bundle submission.

***

## Tutorial Video

{% embed url="https://www.youtube.com/watch?v=qupM7HDdaxY" %}

***

## **Step by Step**

{% stepper %}
{% step %}
### **Connect Wallet**

Click the button in the top right corner to connect a wallet that supports the EVM network.

<figure><img src="../../../.gitbook/assets/image (1036).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Enter Payment Wallet Private Key

{% hint style="danger" %}
<mark style="color:red;">**Security Tips**</mark>

Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

Enter the private key of the control address used for token issuance. This address will serve as the token developer address for creating tokens on Four.meme, as well as for paying functional service fees.



<figure><img src="../../../.gitbook/assets/image (1037).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Dev Buy

{% hint style="warning" %}
**Wallet Settings:**

The Dev wallet, Bonding Curve wallets, and DEX wallets cannot be shared; all business private keys must be unique.
{% endhint %}

The amount of tokens purchased using the token developer's wallet; on-chain monitoring platforms will display this as a developer purchase. Leaving it blank defaults to 0.

<figure><img src="../../../.gitbook/assets/image (1039).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Enter Token Information

<figure><img src="../../../.gitbook/assets/image (1) (1).png" alt=""><figcaption></figcaption></figure>

* **Token Name:** Full token name displayed in wallets and explorers (e.g., MyFirstToken).
* **Symbol:** Token abbreviation, usually 3–6 uppercase letters (e.g., MYT).
* **LOGO:** Upload the project badge image. Recommended size: 1000x1000 px.
* **Description (Opt.):** Brief background and goals to boost project trust and clarity.
{% endstep %}

{% step %}
### Open Mode

Full support for OpenFour templates, allowing your token to use different launch, trading, dividend, liquidity, and incentive models.

Switch between the tabs below to view the details:

{% tabs %}
{% tab title="Royalty" %}
Distribute royalties from transaction taxes to creators, the community, or a designated treasury.

Supported features:

* [x] Supported fundraising tokens: BNB / NVDAB / SPCXB / QQQB / GMEB / FLNCB / DJTB / MRNAB / HOODB
* [x] Token taxes
* [x] Anti-sniping
* [x] Bonding Curve bundled buys

For this template, the Recipient allocation from token taxes must be greater than 10%, and the Minimum token holding for rewards required to receive dividends is 1.
{% endtab %}

{% tab title="Creator Incentives" %}
Rewards token creators based on predefined rules. Creator fees dynamically adjust between 0.02% and 1% based on market cap, starting lower and gradually increasing as the token’s market cap grows.

Supported features:

* [x] Supported fundraising token: BNB
* [x] Anti-sniping
* [x] Bonding Curve bundled buys
{% endtab %}

{% tab title="Likwid DEX" %}
After graduation, the token migrates to Likwid DEX, where its unified liquidity system supports swaps, lending, leveraged long positions, and short positions.

Supported features:

* [x] Supported fundraising token: BNB
* [x] Anti-sniping
* [x] Bonding Curve bundled buys
{% endtab %}

{% tab title="Cubepeg" %}
Cubepeg links tradable tokens with NFT ownership benefits. Every 100,000 tokens held corresponds to one NFT, and the associated NFT is burned according to the mechanism when the tokens are sold.

* Use NFTs to showcase token-holder status.
* Link community roles and collectible identities to token holdings.
* Build gaming or membership experiences around token holdings.

Supported features:

* [x] Supported fundraising token: BNB
* [x] Anti-sniping
* [x] Bonding Curve bundled buys
{% endtab %}

{% tab title="ListaYield" %}
ListaYield combines transaction-tax distributions with Lista staking vaults. Eligible holders receive vault share tokens, and the token migrates to ListaDEX after graduation.

Supported features:

* [x] Supported fundraising token: BNB
* [x] Token taxes
* [x] Anti-sniping
* [x] Bonding Curve bundled buys
{% endtab %}

{% tab title="4STOCK" %}
Bring real-world stocks onto BNB Chain with 1:1 asset backing for on-chain trading and use them as liquidity-pool assets for stock-themed meme coins.

Supported features:

* [x] Supported fundraising token: BNC4
* [x] Token taxes
* [x] Anti-sniping
* [x] Bonding Curve bundled buys
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Set Trading Tax <mark style="color:$info;">(Opt.)</mark>

CiaoTool now supports Fourmeme's latest tax fee function, making it convenient and fast to build exclusive tokenomics.

Trading tax fees will take effect after the token fills up the bonding curve and migrates to the DEX.

<figure><img src="../../../.gitbook/assets/image (1041).png" alt=""><figcaption></figcaption></figure>

* **Tax Receive Fee:** Auto-transfers a fixed rate of tokens to the fund address for project promotion.
* **Dividend Fee:** Distributes tax allocations to all LP token holders based on ownership percentages.
* **Burn Fee:** Distributes tax allocations to all LP token holders based on ownership percentages.
* **LP Fee:** Automatically injects a portion of tokens into the pool to sustain deep trading liquidity.
* **Dividend Threshold:** Limits rewards to holders meeting the minimum balance, driving holding confidence. Min: 10,000.
{% endstep %}

{% step %}
### **Add Socials Links&#x20;**<mark style="color:$info;">**(Opt.)**</mark>

This section is optional, but adding your website, X/Twitter, and Telegram is highly recommended. These links make it easier for users to follow the project and join your community.
{% endstep %}

{% step %}
### Select Project Tags

Select one tag below to define your project's scenario and direction. Single choice only.

`Meme / AI / DeFi / Game / Infra / DeSci / Social / DePin / Charity / Others`
{% endstep %}

{% step %}
### Bonding Curve Wallets

{% hint style="danger" %}
<mark style="color:red;">**Security Tips**</mark>

Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

These wallets will participate in bundled buys during the bonding-curve stage. Up to 20 wallets are supported.

1. Click the **"Import Private Key"** button to open the input pop-up.

<figure><img src="../../../.gitbook/assets/image (1005).png" alt=""><figcaption></figcaption></figure>

2. Manually enter or import the private key file, and click confirm once the private key is displayed in the confirmation box.

<figure><img src="../../../.gitbook/assets/image (984).png" alt=""><figcaption></figcaption></figure>

Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.\
Click to download and view the template:

{% file src="../../../.gitbook/assets/EVM_privateKey_demo.xlsx" %}
{% endstep %}

{% step %}
### Bonding Curve Buy Amount

{% hint style="info" %}
Keep at least 0.00011 BNB in each wallet to cover gas fees.

Clicking MAX auto-reserves \~0.0011 BNB for gas fees. You can still manually edit the final amount.
{% endhint %}

Set a buy amount for each wallet. If you only want to execute bundled buys during the bonding-curve stage, the combined amount across all wallets must not exceed **18.18 BNB** or the equivalent amount in the selected quote token.
{% endstep %}

{% step %}
### DEX Wallets <mark style="color:$info;">(Opt.)</mark>

These wallets will participate in the bundled buy during the migration stage. Up to five wallets are supported.

{% hint style="info" %}
To enable external-pool migration and multi-wallet sniping, the combined DEX purchase amount from the Dev wallet and Bonding Curve wallets must exceed the required threshold.
{% endhint %}
{% endstep %}

{% step %}
### DEX Buy Amount

Set the buy amount for each wallet participating in the migration stage. There is no limit on the purchase amount.
{% endstep %}

{% step %}
### **Confirm** <a href="#confirm" id="confirm"></a>

After verifying all details, click the **"Create Token and Buy"** button below and wait for the launch process to complete.
{% endstep %}
{% endstepper %}

***

## **FAQs**

<details>

<summary><strong>What is Fourmeme Bundler?</strong></summary>

A zero-code tool on BSC to launch tokens and deploy multi-wallet, same-block buys simultaneously.

</details>

<details>

<summary><strong>Why execute "creation" and "buying" bundled together?</strong></summary>

Bonding curves pump prices instantly. Bundling wipes out time gaps to completely stop front-running bots.

</details>

<details>

<summary><strong>Can this feature be used to optimize the early token-holding structure?</strong></summary>

Yes. Spreading buys across wallet matrices builds a naturally decentralized holder map at launch.

</details>

<details>

<summary><strong>Why does the "Bundler" operation prompt a failure?</strong></summary>

According to Four.meme's rules, the same token name can only have one token. If the token name is the same, it cannot be created.

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
