---
description: >-
  专为 BONKfun
  平台提供的代币发行与多地址捆绑买入工具。支持在同区块内同步完成代币创建与首笔批量买入，有效阻断机器人抢跑，确保项目方以极低初始成本安全建仓并优化早期持币分布。
---

# Bonk - 创建并买入教程

{% hint style="info" %}
**CiaoTool Bonk 创建并买入**现已全面支持官方 **SOL** 和 **USD1** 全部的价值代币，请先切换到指定代币页面进行创建代币并捆绑买入操作，满足不同场景下的快捷开盘服务。
{% endhint %}

## CiaoTool Bonk 创建并买入是什么？

**CiaoTool Bonk 创建并买入**是一款专为 Solana 生态 **BONKfun 平台**打造的代币发行与自动化建仓工具。它允许用户在发布全新代币的同时，全自动调度多个钱包地址在同一区块内完成首笔批量买入。

相较于“先发币、后手动买入”的传统模式，该功能的核心机制在于“底层捆绑打包”。系统会将代币创建指令与多地址的买入指令聚合为一个不可分割的数据包提交至链上。这种机制确保了用户的买入交易紧跟在代币创建之后瞬间完成，彻底消除了时间差。它从根本上防止了链上狙击机器人的抢跑买入，保障项目方能够以内盘最底端的初始价格完成早期资产配置。

立即在Bonk 上，用 CiaoTool​ 创建并买入功能进行一键开盘操作：

{% embed url="https://ciaotool.io/zh-CN/bonk/create-and-buy" %}

***

## 为什么选择 CiaoTool Bonk 创建并买入？

CiaoTool 为 BONKfun 平台上的代币首发提供了一种兼顾安全性与极低成本的专业解决方案。对于需要精确控制早期筹码及防范恶意夹击的用户而言，该工具构建了稳健的执行防线：

* **彻底阻断抢跑：**&#x901A;过底层捆绑打包技术，将发币与买入指令在同区块内无缝聚合，有效防止链上狙击机器人提前买入推高价格。
* **锁定极低成本：**&#x786E;保多钱包买入指令作为创世区块的首批交易执行，使项目方能够以绝对的初始低价完成建仓，最大程度降低资金损耗。
* **优化早期分布：**&#x652F;持自定义配置多个独立地址同步买入，在代币发射的瞬间即完成基础的持币者结构分散，美化早期链上数据。
* **全自动极速部署：**&#x4E00;键自动完成代币信息上传、参数配置与多地址资产分发，彻底免去繁琐的人工切换与手动抢筹操作。

***

## 视频教程 | Bonk 创建并买入

{% embed url="https://www.youtube.com/watch?v=Ir3oB7Li7PM" %}

***

## **图文指南 |** Bonk 创建并买入&#x20;

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (396).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 填写代币基础信息

<figure><img src="../../../.gitbook/assets/image (398).png" alt=""><figcaption></figcaption></figure>

您可以手动填写代币信息，或者点击 **【克隆】** 按钮，克隆其他代币的信息

* **名称：**&#x60A8;希望展示在钱包或区块浏览器中的完整代币名称（_例如：MyFirstToken_）。
* **简称：**&#x4EE3;币的缩写，通常为 3\~6 个大写字母（_例如：MYT_）。
* **Logo：**&#x4E0A;传项目或代币的标志图像，建议尺寸 1000\*1000 像素。
* **描述：**&#x975E;必填项，简要介绍项目的背景、目标和用途。此描述将帮助用户理解您的代币的功能和项目愿景，提高项目真实性。
* **社交链接：**&#x6DFB;加与项目相关的社交媒体链接（如 官网、X/Twitter、Telegram）,有助于用户关注和加入您的项目社区。
{% endstep %}

{% step %}
### Dev 钱包买入

即当前绑定钱包进行买入操作，不填默认为 0。

<figure><img src="../../../.gitbook/assets/image (399).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入捆绑买入私钥地址

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

当&#x524D;**「创建并买入」**&#x529F;能仅支持 私钥导入以进行交易操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入接收地址的类型，选择以查看详细教程。最多支持 **8 个地址**捆绑买入。

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「手动输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (400).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (401).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x4E00;行仅输入一个地址，按回车键换行

<figure><img src="../../../.gitbook/assets/image (402).png" alt=""><figcaption></figcaption></figure>

3.

    点&#x51FB;**「确定」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (403).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 点&#x51FB;**「上传文件」**&#x6309;钮，弹出文件上传窗口。

<figure><img src="../../../.gitbook/assets/image (405).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (251).png" alt=""><figcaption></figcaption></figure>

2. 导入钱包地址信息文件，显示地址信息。\
   请通过 CiaoTool 模板文件导入，以确保私钥准确导入。

<figure><img src="../../../.gitbook/assets/image (247).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (404).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入买入金额

支&#x6301;**「逐一输入」「统一金额」「百分比」**&#x548C;**「全部」**&#x56DB;种买入金额类型。

<figure><img src="../../../.gitbook/assets/image (252).png" alt=""><figcaption></figcaption></figure>

1. **逐一输入**

* 在输入框中，逐一输入买入金额数量
* 若填写数量，则按照填写的数量进行交易。
* 若未填写数量，则按照交易数量中  设置的数量进行交易。

2. **统一金额**\
   击转账数量上方&#x7684;**「统一输入」**&#x6309;钮，选&#x62E9;**「统一金额」，**&#x6240;有选钱包根据同一数量将代币全部兑换为指定代币。
3. **百分比**\
   点击转账数量上方&#x7684;**「统一输入」**&#x6309;钮，选&#x62E9;**「百分比」，**&#x6240;有选钱包根据当前余额的百分比，兑换为指定代币。

* **全部**\
  所有钱包将把价值代币全部购买为指定代币。
{% endstep %}

{% step %}
### 自定义服务

#### 自定义合约地址

打造你的个性化代币地址，设置代币地址，**额外收费 0.01 SOL。**

<figure><img src="../../../.gitbook/assets/image (406).png" alt=""><figcaption></figcaption></figure>

**自定义代币地址**

* 提前生成您想要的钱包地址，可以是靓号地址。
* 将你提前生成的私钥粘贴导入（**地址必须要全新地址且没有付过SOL租金**）；
* 系统将使用该地址部署你的代币，确保合约地址与预期一致。

#### 提前生成代币合约

提前生成代币合约地址，当前编辑的代币信息将全部保留与链上，适用于需要在正式开盘前进行预热或对接的场景。
{% endstep %}

{% step %}
### Jito 小费设置

配置 Jito MEV 小费，用于加速打包交易，提高排序优先级。

{% hint style="danger" %}
此功能实现依赖于 Jito 的捆绑功能。由于网络环境、Jito节点、RPC节点和区块处理引擎的复杂影响，该功能可能面临较高的失败率。

若操作失败，不会开盘成功也不会产生任何费用，请尝试更换RPC节点，区块处理引擎，增加Jito的小费(建议0.001SOL)，并考虑在链上活跃度较低的时段再次尝试。
{% endhint %}
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下&#x65B9;**「创建并买入」**&#x6309;钮，并等待开盘完成。
{% endstep %}
{% endstepper %}

## **常见失败案例**

* 若因 Jito 小费低于市场均值或遭机器人抢跑导致失败，请适当提高 Jito 小费并重试。
* 若因 RPC 节点或区块引擎响应延迟导致错失打包时机，请切换至其他更稳定的节点。
* 若因主钱包余额不足以支付建币费与租金等隐藏消耗，请确保额外预留至少 0.05 SOL 的缓冲资金。
* 若因代币头像档案过大导致上传逾时，请将图片压缩至 1MB 以内再重新发起操作。
* 若遇 Solana 链上极度壅塞引发底层随机丢包，请直接避开交易尖峰时段，稍后再试。

***

## **常见问题 FAQ**

<details>

<summary><strong>什么是 Bonk 创建并买入功能？</strong></summary>

这是一款针对 BONKfun 平台的代币极速发行工具。它能够将“创建代币”与“多个地址买入”这两个独立动作打包在同一个区块内同步执行，确保您 100% 在底部买入筹码，实现开盘及多地址持仓分布。

</details>

<details>

<summary><strong>为什么要将“创建”和“买入”捆绑在一起执行？</strong></summary>

Bonk 采用联合曲线定价机制，代币价格会随着买入量的增加而迅速上涨。如果先发币再手动买入，中间产生的时间差极易被链上狙击机器人监控并抢先买入，导致您被迫以数倍的高价接盘。捆绑执行消除了时间差，彻底阻断了恶意抢跑，保护了初始建仓的资金成本。

</details>

<details>

<summary><strong>这项功能可以用来优化代币早期的持币结构吗？</strong></summary>

可以。由于该功能支持批量导入多个钱包地址同步执行买入，这些买入会在代币创建的瞬间独立完成。这能让代币在刚发布时就展现出健康、分散的持币者分布数据，避免筹码过于集中在单一地址中。

</details>

<details>

<summary><strong>为什么“创建并买入”操作会一直提示失败？</strong></summary>

失败是由于该功能依赖于 Jito 的捆绑打包机制。在网络拥堵或节点延迟时，Jito 捆绑包很难被验证者顺利打包上链，从而导致较高的失败率。\
完全不会扣钱。 该操作是绑定的，一旦失败，代币不会发行，本金和手续费也不会有任何损耗。若需提高成功率，建议尝试增加 Jito 小费（推荐 0.001 SOL）、更换 RPC 节点/区块引擎，或在链上交易低谷期重新操作。

</details>

<details>

<summary><strong>操作是否安全？</strong></summary>

平台采用纯前端签名机制，您的私钥绝不会被上传或储存在任何服务器上，所有交易均在本地浏览器完成签名，从技术层面确保平台无法访问您的私钥。

</details>

**💬 如遇到问题？加入社群实时咨询**：[https://t.me/ciaotool](https://t.me/ciaotool)

* **Email**：[support@ciaotool.io](mailto:support@ciaotool.io)
* **官网**：[https://ciaotool.io](https://ciaotool.io/)
* **X（Twitter）**：[https://x.com/CiaoTool](https://x.com/CiaoTool)
* **Medium**： [https://medium.com/@ciaotool](https://medium.com/@ciaotool)
* **Blog**：[https://www.ciaoailiquidity.com/zh/blog](https://www.ciaoailiquidity.com/zh/blog)
* **YouTube**：[https://www.youtube.com/@CiaoTool](https://www.youtube.com/@CiaoTool)
* **WhatsApp**：[https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J](https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J)

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
