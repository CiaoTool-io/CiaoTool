---
description: >-
  CiaoTool provides a no-code PancakeSwap V3 liquidity adding tool. Supports
  CLMM pools and single-sided liquidity additions for efficient liquidity
  management.
---

# BSC - V3 Liquidity Adder Tutorial

{% hint style="info" %}
This page covers **PancakeSwap V3 Liquidity Pool Adder**, which adds a V3 liquidity pool with concentrated liquidity and custom price ranges.

If you want to add a V2 liquidity pool featuring ease of use and full-range coverage, please refer to the [**PancakeSwap V2 Liquidity Pool Adder**](liquidity-adder-v2.md) guide.
{% endhint %}

## What is PancakeSwap V3 Liquidity Adder?

<figure><picture><source srcset="../../../.gitbook/assets/ScreenShot_2026-06-18_175516_891.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (2).png" alt="CiaoTool BSC Toolkit Page about PancakeSwap V3 Liquidity Pool Adder Feature"></picture><figcaption></figcaption></figure>

Adding PancakeSwap V3 Liquidity refers to the operation of appending market-making capital into an already deployed V3 liquidity pool. The V3 protocol adopts a "concentrated liquidity" mechanism, requiring market makers to set a specific price range when adding capital.

Common Use Cases:

* **Dynamic Tuning**\
  Constantly adjusts and adds liquidity during price fluctuations to secure tight trading depth around current market rates.
* **Single-Sided Walls**\
  Deploys targeted low-price buy walls or high-price sell pressure using V3’s precise single-sided liquidity mechanics.

Start your V3 Liquidity Pool Adder on BNB Smart Chain with CiaoTool now:

{% embed url="https://bsc.ciaotool.io/en/swap/v3/add-liquidity-v3" %}

***

## Why Choose CiaoTool PancakeSwap V3 Liquidity Adder?

For professional teams needing strict control over chip distribution, CiaoTool builds an extremely secure and efficient infrastructure:

* **No-Code V3 Tool**\
  Visual web panel replaces complex V3 range calculations for barrier-free, seamless pool updates.
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

<figure><img src="../../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>
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
### Enter Token Pair Address

Each V3 liquidity pool for different token pairs / different fee tiers has an independent pair address. Input the pair address into the box, and the system will automatically display the pair information.

<figure><img src="../../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Set Price Range

<figure><img src="../../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

1. Range size determines the level of yield (applicable to both LP fee yields and CAKE yields):

* The narrower it is, the higher the yield, and the greater the impermanent loss;
* The wider it is, the lower the yield, and the smaller the impermanent loss;
* A full-range setting operates similarly to V2, and the yield will be very small.

2. When out of range:

* The V3 pool generates no yield;
* The liquidity position will turn into a single token;
* You can remove liquidity and add it again, or wait for the price to return to the range;
* You can add a V2 liquidity pool to ensure base liquidity outside the V3 range.

1. Single-Sided Rule:

* Single-sided deposits on Uniswap/Pancake V3 only apply when the current price is outside your designated range. Full-range mode cannot be single-sided.
{% endstep %}

{% step %}
### Enter Pool-Adding Token Amount

<figure><img src="../../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

The system will automatically calculate the pool-adding amount of the value token / project token based on the current pair price and the price range for adding liquidity.

You can freely enter the amount of pool-adding tokens to display the status of the pool-adding pair amounts.
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
