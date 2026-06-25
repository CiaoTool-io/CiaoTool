---
description: >-
  A token launch and bundle buy tool built for Four.meme. Create tokens and
  execute multi-wallet buys within the same block to optimize early holder
  distribution and establish positions efficiently.
---

# Fourmeme - Bundler Tutorial (Create & Buy)

{% hint style="info" %}
**CiaoTool Fourmeme Bundler** fully supports all quote tokens, including **BNB, USD1 and UUSD**. Please switch to the specific token page to perform token launch operations based on your needs.&#x20;
{% endhint %}

## What is CiaoTool Fourmeme Bundler?

<figure><picture><source srcset="../../../.gitbook/assets/ScreenShot_2026-06-22_165108_209.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (1035).png" alt="CiaoTool BSC Toolkit Page about Four.meme Bundler Feature"></picture><figcaption></figcaption></figure>

**CiaoTool Fourmeme Bundler** is an automated token deployment and position-building tool built for the BSC **Four.meme platform**, enabling multi-wallet batch purchases alongside token creation in the same block.

Instead of traditional manual buying, it aggregates the creation and multi-address purchase instructions into an indivisible data package, executing buy orders instantly after deployment to wipe out time gaps.

This atomic execution completely blocks on-chain front-running bots, safeguarding your early asset configuration at the absolute lowest internal floor price.

Start Create and Buy Token on Fourmeme with CiaoTool now:

{% embed url="https://bsc.ciaotool.io/en/fourmeme/bnb/create-and-buy" %}

***

## Why Choose CiaoTool Fourmeme Bundler

CiaoTool provides a secure and efficient launch solution for Four.meme tokens, helping users optimize early token distribution and streamline the launch process.

* **Same-Block Execution**\
  Token creation and buying are bundled together for a faster and more efficient launch process.
* **Efficient Position Building**\
  Supports simultaneous purchases across multiple wallets to establish early positions quickly.
* **Optimized Holder Distribution**\
  Allows multiple addresses to participate in the initial buy, improving holder distribution.
* **One-Click Launch**\
  Automates token creation, parameter setup, and batch buying for a streamlined launch experience.
* **All-in-One Toolkit**\
  Smoothly transitions from bundled buys to market making or multisender within one platform.

***

## Video Tutorial

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
### Enter Token Information

<figure><img src="../../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

* **Token Name:** Full token name displayed in wallets and explorers (e.g., MyFirstToken).
* **Symbol:** Token abbreviation, usually 3–6 uppercase letters (e.g., MYT).
* **LOGO:** Upload the project badge image. Recommended size: 1000x1000 px.
* **Description (Opt.):** Brief background and goals to boost project trust and clarity.
* **Socials Links (Opt.):** Highly recommended: Website, X, and Telegram to build your community.
{% endstep %}

{% step %}
### Dev Buy

{% hint style="warning" %}
**Wallet Settings:**

The Dev wallet and bundled wallets cannot be shared; all business private keys must be unique.
{% endhint %}

The amount of tokens purchased using the token developer's wallet; on-chain monitoring platforms will display this as a developer purchase. Leaving it blank defaults to 0.

<figure><img src="../../../.gitbook/assets/image (1039).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select Project Tags

Select one tag below to define your project's scenario and direction. Single choice only.

`Meme / AI / DeFi / Game / Infra / DeSci / Social / DePin / Charity / Others`

<figure><img src="../../../.gitbook/assets/image (1040).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Set Trading Tax<sub><mark style="color:$info;">(opt.)<mark style="color:$info;"></sub>

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
### Import Trading Wallet Private Key

{% hint style="danger" %}
<mark style="color:red;">**Security Tips**</mark>

Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

Supports two import types for trading address private keys: "Manual Input" and "Upload File". Up to 20 addresses is supported.

1. Click the **"Import Private Key"** button to open the input pop-up.

<figure><img src="../../../.gitbook/assets/image (1005).png" alt=""><figcaption></figcaption></figure>

2. Manually enter or import the private key file, and click confirm once the private key is displayed in the confirmation box.

<figure><img src="../../../.gitbook/assets/image (984).png" alt=""><figcaption></figcaption></figure>

Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.\
Click to download and view the template:

{% file src="../../../.gitbook/assets/EVM_privateKey_demo.xlsx" %}
{% endstep %}

{% step %}
### Enter Buy Amount

{% hint style="info" %}
Keep at least 0.0008 BNB in each wallet to cover gas fees.

Clicking MAX auto-reserves \~0.001 BNB for gas fees. You can still manually edit the final amount.
{% endhint %}

Set custom buy amounts per address. The total combined volume **must not exceed 18 BNB.**
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
