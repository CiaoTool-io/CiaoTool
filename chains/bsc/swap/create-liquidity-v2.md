---
description: >-
  CiaoTool provides a PancakeSwap V2 liquidity pool creation tool. Deploy AMM
  liquidity pools with one click and launch token trading with ease.
---

# BSC - V2 Liquidity Pool Creator Tutorial

{% hint style="info" %}
This page covers **PancakeSwap V2 Liquidity Pool Creator**, which creates a full-range V2 liquidity pool without requiring price range configuration.

If you want concentrated liquidity and custom price ranges, please refer to the [**PancakeSwap V3 Liquidity Pool Creator**](create-liquidity-v3.md) guide.
{% endhint %}

## What is PancakeSwap V2 Liquidity Pool?

<figure><picture><source srcset="../../../.gitbook/assets/屏幕截图 2026-06-18 165317.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (1014).png" alt="CiaoTool BSC Toolkit Page about PancakeSwap V2 Liquidity Pool Creator Feature"></picture><figcaption></figcaption></figure>

**PancakeSwap V2 Liquidity Pool** is a decentralized trading foundation based on the most classic AMM mechanism on the BNB Chain (BSC). Through the constant product formula $$x \times y = k$$, it provides initial trading pricing and buy/sell depth for tokens.

For any newly issued token, creating a V2 liquidity pool is the inevitable path for the token to transform into a "circulating asset." By injecting a certain proportion of base assets (such as BNB or USDT) and project tokens, project teams can anchor the initial price for the asset and build a permissionless buying and selling market.

Common Use Cases:

* **Initial Launch**\
  Establishes token opening prices and opens permissionless public trading on BSC instantly.
* **Base Liquidity**\
  Builds foundational pool depth to support subsequent on-chain market making and protocol integration.

Start your V2 Liquidity Pool Creator on BNB Smart Chain with CiaoTool now:

{% embed url="https://bsc.ciaotool.io/en/swap/v2/create-liquidity-v2" %}

***

## How to Choose Between V2 and V3 Liquidity Pools?

<table><thead><tr><th width="134">Dimension</th><th>V2 Pool</th><th>V3 Pool</th></tr></thead><tbody><tr><td>Liquidity Distribution</td><td>Full-range coverage.</td><td>Concentrated liquidity (custom price ranges)</td></tr><tr><td>Capital Efficiency</td><td>Relatively low. Large amounts of capital sit idle at extreme prices without being effectively utilized.</td><td>Extremely high. Compared to V2, capital efficiency can be increased by up to 4,000 times.</td></tr><tr><td>User Threshold</td><td>Extremely low. Requires only entering the token amount and BNB ratio to create a pool with one click.</td><td>Relatively high. Requires manually setting and adjusting the upper and lower price limits of liquidity.</td></tr><tr><td>Fee Mechanism</td><td>Fixed 0.25% trading fee.</td><td>Provides multiple tier levels (e.g., 0.01%, 0.05%, 0.25%, 1%), customizable based on asset volatility.</td></tr><tr><td>Impermanent Loss Risk</td><td>Standard risk. Losses brought by asset price changes are relatively predictable.</td><td>Higher risk. Due to concentrated capital, if the price falls out of your set range, it will break through instantly.</td></tr><tr><td>Slippage Performance</td><td>Prone to causing larger slippage during large-volume trades.</td><td>Within the set liquidity range, slippage is extremely low, delivering an excellent trading experience.</td></tr><tr><td>Tokenomics Compatibility</td><td>Some tokens with complex mechanisms may encounter compatibility issues when deployed on V3.</td><td>Perfectly compatible with all types of tokens.</td></tr></tbody></table>

***

## Why Choose CiaoTool to Create V2 Liquidity Pool?

For professional teams needing strict control over chip distribution, CiaoTool builds an extremely secure and efficient infrastructure:

* **No-Code**\
  Visual web panel replaces complex AMM scripts for secure, precise liquidity pool initialization.
* **Local Privacy**\
  Pure client-side local signing ensures total key privacy and multi-wallet safety.
* **All-in-One Toolkit**\
  Seamlessly pairs pool creation with native market making or batch swaps for all-in-one on-chain scaling.

***

## **Step by Step**

{% stepper %}
{% step %}
### **Connect Wallet**

Click the button in the top right corner to connect a wallet that supports the EVM network.

<figure><img src="../../../.gitbook/assets/image (1015).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Enter Payment Wallet Private Key <a href="#enter-payment-wallet-private-key" id="enter-payment-wallet-private-key"></a>

{% hint style="danger" %}
<mark style="color:red;">**Security Tips**</mark>

Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

This wallet address will be used to pay fees and will hold ownership of the pool.

<figure><img src="../../../.gitbook/assets/image (1016).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Enter Pool-Adding Token Addresses

Input the token addresses into the boxes as the quote token and project token; there is no specific entry order.

<figure><img src="../../../.gitbook/assets/image (1017).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Enter Pool-Adding Token Amount

<figure><img src="../../../.gitbook/assets/image (1032).png" alt=""><figcaption></figcaption></figure>

Enter the token amounts of the two pool-adding tokens to be placed into the liquidity pool respectively. Please calculate the appropriate ratio yourself and determine the initial pair price before creating liquidity.

Initial Pair Price: `Project Token / Quote Token = Initial Price`
{% endstep %}

{% step %}
### **Confirm** <a href="#confirm" id="confirm"></a>

After verifying all details, click the **"Start Swap"** button below and wait for the transaction process to complete.
{% endstep %}
{% endstepper %}

***

**Need help? Join our community for real-time support:**

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
