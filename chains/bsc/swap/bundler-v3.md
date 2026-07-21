---
description: >-
  Create a CLMM liquidity pool and execute multi-address buys within the same
  block on BSC. Helps reduce MEV interference while providing a secure and
  efficient token launch experience.
---

# BSC - V3 Liquidity Bundler Tutorial

{% hint style="info" %}
This page covers **PancakeSwap V3 Liquidity Bundler**, which creates a V3 liquidity pool with concentrated liquidity and custom price ranges.

If you want to create a V2 liquidity pool featuring ease of use and full-range coverage, please refer to the [**PancakeSwap V2 Liquidity Bundler**](bundler-v2.md) guide.
{% endhint %}

## What is PancakeSwap V3 Liquidity Pool Bundler?

<figure><picture><source srcset="../../../.gitbook/assets/ScreenShot_2026-06-18_175516_891 (6).png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (1030).png" alt="CiaoTool BSC Toolkit Page about PancakeSwap V3 Liquidity Bundler Feature"></picture><figcaption></figcaption></figure>

**PancakeSwap V3 liquidity pools** use Concentrated Liquidity (CLMM), allowing liquidity to be deployed within custom price ranges for higher capital efficiency and deeper liquidity. Unlike V2, V3 supports Concentrated Liquidity (CLMM), allowing liquidity to be deployed within specific price ranges for improved capital efficiency and deeper liquidity.

In traditional launches, manual liquidity addition is easily sniped by MEV bots in the same block, forcing real users to buy at a high position.

CiaoTool packages "V3 pool creation" and "initial buy-in" into a single transaction, locking out MEV front-runners completely. Eliminates same-block front-running risks, ensuring your project team and users enter at the true base price.

Common Use Cases:

* **Token Launches**: Create a liquidity pool and establish initial positions.
* **Meme Token Launches**: Quickly deploy liquidity and build early holdings.
* **Simplified Launch Process**: Reduce operational steps and improve execution efficiency.
* **Faster Market Entry**: Bring tokens to decentralized exchanges more efficiently.

Start your V3 Liquidity Bundler on BNB Smart Chain with CiaoTool now:

{% embed url="https://bsc.ciaotool.io/en/swap/v3/create-liquidity-and-buy-v3" %}

***

## How to Choose Between V2 and V3 Liquidity Pools?

<table><thead><tr><th width="134">Dimension</th><th>V3 Pool</th><th>V2 Pool</th></tr></thead><tbody><tr><td>Liquidity Distribution</td><td>Concentrated liquidity (custom price ranges)</td><td>Full-range coverage.</td></tr><tr><td>Capital Efficiency</td><td>Extremely high. Compared to V2, capital efficiency can be increased by up to 4,000 times.</td><td>Relatively low. Large amounts of capital sit idle at extreme prices without being effectively utilized.</td></tr><tr><td>User Threshold</td><td>Relatively high. Requires manually setting and adjusting the upper and lower price limits of liquidity.</td><td>Extremely low. Requires only entering the token amount and BNB ratio to create a pool with one click.</td></tr><tr><td>Fee Mechanism</td><td>Provides multiple tier levels (e.g., 0.01%, 0.05%, 0.25%, 1%), customizable based on asset volatility.</td><td>Fixed 0.25% trading fee.</td></tr><tr><td>Impermanent Loss Risk</td><td>Higher risk. Due to concentrated capital, if the price falls out of your set range, it will break through instantly.</td><td>Standard risk. Losses brought by asset price changes are relatively predictable.</td></tr><tr><td>Slippage Performance</td><td>Within the set liquidity range, slippage is extremely low, delivering an excellent trading experience.</td><td>Prone to causing larger slippage during large-volume trades.</td></tr><tr><td>Tokenomics Compatibility</td><td>Perfectly compatible with all types of tokens.</td><td>Some tokens with complex mechanisms may encounter compatibility issues when deployed on V3.</td></tr></tbody></table>

***

## Why Choose CiaoTool to Create V3 Liquidity Pool?

For professional teams needing strict control over chip distribution, CiaoTool builds an extremely secure and efficient infrastructure:

* **No-Code V3 Tool**\
  Visual web panel replaces complex V3 range calculations for barrier-free, seamless pool creation.
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
### Fee Tier Setup

<figure><img src="../../../.gitbook/assets/image (1020).png" alt=""><figcaption></figcaption></figure>

Trading fees vary: \
V3 has four different trading fee tiers, which can reduce trading fees by up to 25 times compared to V2; for V2, a 0.25% fee will be paid for every single transaction. You can also choose 1% to obtain higher LP yields.
{% endstep %}

{% step %}
### Set the Initial Price & Price Range

<figure><img src="../../../.gitbook/assets/image (1021).png" alt=""><figcaption></figcaption></figure>

1. Range size determines the level of yield (applicable to both LP fee yields and CAKE yields):

* The narrower it is, the higher the yield, and the greater the impermanent loss;
* The wider it is, the lower the yield, and the smaller the impermanent loss;
* A full-range setting operates similarly to V2, and the yield will be very small.

2. When out of range:

* The V3 pool generates no yield;
* The liquidity position will turn into a single token;
* You can remove liquidity and add it again, or wait for the price to return to the range;
* You can add a V2 liquidity pool to ensure base liquidity outside the V3 range.
{% endstep %}

{% step %}
### Enter Pool-Adding Token Amount

<figure><img src="../../../.gitbook/assets/image (1022).png" alt=""><figcaption></figcaption></figure>

Entering an initial price and range auto-calculates token amounts. Conversely, modifying token amounts auto-adjusts your price range.
{% endstep %}

{% step %}
### Import Trading Wallet Private Key

{% hint style="danger" %}
<mark style="color:red;">**Security Tips**</mark>

Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

Supports two import types for trading address private keys: "Manual Input" and "Upload File". Up to 20 addresses is supported.

1. Click the **"Import Private Key"** button to open the input pop-up.

<figure><img src="../../../.gitbook/assets/image (1001).png" alt=""><figcaption></figcaption></figure>

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

Supports two trading amount types: **"Custom Input"**, and **"All"**.

<figure><img src="../../../.gitbook/assets/image (1002).png" alt=""><figcaption></figcaption></figure>

1. **Custom Input**\
   Enter the transfer amount for each wallet individually.
   * If an amount is filled in, the transfer will use that specific amount.
   * If an amount is left blank, the transfer will default to the amount configured in the global settings.
2. **All**\
   Swaps the entire wallet balance into the target token.
{% endstep %}

{% step %}
### **Confirm** <a href="#confirm" id="confirm"></a>

After verifying all details, click the **"Start Swap"** button below and wait for the transaction process to complete.

{% hint style="danger" %}
Each V3 liquidity pool for different token pairs / different fee tiers has a different pair address. Please be sure to save the pair contract address information and save the LP credentials to your Web3 wallet.
{% endhint %}
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>为什么创建流动性并捆绑买入会失败？</strong></summary>

请确认钱包内 BNB / WBNB 余额是否充足，以覆盖加池，捆绑买入所需资金及 Gas 费用。

</details>

<details>

<summary><strong>为什么要将“创建”和“买入”捆绑在一起执行？</strong></summary>

如果先创建池子再手动买入，中间产生的时间差极易被链上狙击机器人监控并抢先买入，导致您被迫以数倍的高价接盘。捆绑执行消除了时间差，彻底阻断了恶意抢跑，保护了初始建仓的资金成本。

</details>

<details>

<summary><strong>这项功能可以用来优化代币早期的持币结构吗？</strong></summary>

可以。由于该功能支持批量导入多个钱包地址同步执行买入，这些买入会在代币创建的瞬间独立完成。这能让代币在刚发布时就展现出健康、分散的持币者分布数据，避免筹码过于集中在单一地址中。

</details>

<details>

<summary><strong>操作是否安全？</strong></summary>

平台采用纯前端签名机制，您的私钥绝不会被上传或储存在任何服务器上，所有交易均在本地浏览器完成签名，从技术层面确保平台无法访问您的私钥。

</details>

***

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
