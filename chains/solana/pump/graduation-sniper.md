---
description: >-
  专为 Pump.fun 平台深度定制的代币首发、捆绑建仓与外盘狙击的一体化执行工具。支持在同一区块内瞬间完成代币创建、多钱包内盘买入，并在迁移至
  PumpSwap 的同时狙击建仓，全方位保障早期筹码的安全锁定与连续性策略执行。
---

# PumpFun - 创建并迁移买入教程

{% hint style="info" %}
**CiaoTool PumpFun 创建并迁移买入**现已全面支持官方 **SOL** 和 **USDC** 全部的价值代币，请先切换到指定代币页面进行创建代币、捆绑买入及外盘狙击建仓操作，满足不同场景下的快捷开盘服务。
{% endhint %}

## CiaoTool PumpFun 创建并迁移买入是什么？

**CiaoTool PumpFun 创建并迁移买入**是一款将「创建代币部署」与「多阶段自动化买入」深度结合的高阶开盘与建仓工具。它打破了传统工具只能分段操作的局限，将“内盘诞生”到“外盘迁移”的整个核心跨度，压缩在公链的同一个区块内完成，旨在协助项目团队在代币发行的最初期，建立起兼顾防抢跑与筹码分散的自动化执行防线。

该功能将整个代币发射周期拆分为两个核心执行阶段：

1. **内盘捆绑阶段：**&#x7CFB;统在底层通过 Jito 捆绑机制，将部署代币的指令与首批独立买入钱包的指令无缝打包在同一个区块内。这确保了代币创建的瞬间，项目方设定的钱包能够抢先执行买入，打满联合曲线触发迁移机制，从而锁定联合曲线最底部的初始价格。
2. **迁移狙击阶段：**&#x5F53;官方将流动性迁移至 PumpSwap 的瞬间，预设的狙击钱包交易指令已在同区块的尾端严密锁死。这意味着在外盘资金池刚刚建立、外界狙击机器人甚至还没来得及同步到链上数据的瞬间，项目方的资金已经在外盘完成了首笔抢筹，完美跑通全生命周期的筹码闭环。

立即在 PumpFun 上，用 CiaoTool​ 创建并迁移买入功能进行一键开盘操作：

{% embed url="https://ciaotool.io/zh-CN/pump/graduation-sniper" %}

***

## 为什么选择 CiaoTool PumpFun 创建并迁移买入？

**CiaoTool 全网独家首创的核心底层功能。**&#x8BE5;功能代表了当前 Solana 链开盘管理的技术上限。对于需要绝对掌控项目从内盘到外盘全流程筹码分布、阻断任何外部狙击手干扰的团队而言，它构建了无懈可击的技术壁垒：

* **独家全流程同区块聚合：**&#x901A;常代币从内盘毕业迁移到外盘开盘的瞬间，极易被海量外部狙击机器人通过监控抢入低价筹码并高位砸盘。CiaoTool 独家实现了发币、打满内盘、官方迁移、外盘首笔狙击在同一区块内聚合，外部机器人无法在中间插入任何交易，彻底废除外部机器人的抢跑空间。
* **消除内盘垃圾时间：**&#x5F53;代币在内盘流转时，极易吸引恶意波段盘，导致项目难以平稳毕业。该功能支持一键买满曲线，瞬间把代币推向外盘，消除内盘不确定性；同时确保团队分别锁定内盘曲线最底部及外盘开盘瞬间的绝对最优价格，将做市开盘损耗降至零点。
* **矩阵钱包自动化调度：**&#x4F20;统的跨盘做市需要团队在内盘达标后再去外盘抢开盘，极易因为网络延迟、节点速度差导致策略断层。通过 CiaoTool，完成多钱包资产配置，内盘买入份额测算以及外盘狙击额度分配，实现从「内盘创建」向「外盘狙击」的绝对连续性。
* **纯前端本地绝对安全：**&#x4E25;苛遵守本地化安全规范，所有参与矩阵调度的私钥和签名流程均在用户的浏览器本地环境安全运行。平台技术上不触碰、不上传任何敏感数据，从源头上保障资金的绝对安全。

***

## 视频教程 | PumpFun 创建并迁移买入

{% embed url="https://www.youtube.com/watch?v=Id8Wrebby_Y" %}



***

## **图文指南 |** PumpFun 创建并迁移买入

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (396).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 填写代币基础信息

您可以手动填写代币信息，或者点击 **【克隆】** 按钮，克隆其他代币的信息

* **名称：**&#x60A8;希望展示在钱包或区块浏览器中的完整代币名称（_例如：MyFirstToken_）。
* **简称：**&#x4EE3;币的缩写，通常为 3\~6 个大写字母（_例如：MYT_）。
* **Logo：**&#x4E0A;传项目或代币的标志图像，建议尺寸 1000\*1000 像素。
* **描述：**&#x975E;必填项，简要介绍项目的背景、目标和用途。此描述将帮助用户理解您的代币的功能和项目愿景，提高项目真实性。

<figure><img src="../../../.gitbook/assets/image (398).png" alt=""><figcaption></figcaption></figure>

* **社交链接：**&#x6DFB;加与项目相关的社交媒体链接（如 官网、X/Twitter、Telegram）,有助于用户关注和加入您的项目社区。
{% endstep %}

{% step %}
### Dev 钱包买入

即当前绑定钱包进行买入操作，不填默认为 0。

<figure><img src="../../../.gitbook/assets/image (399).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入内盘买入钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

当&#x524D;**「创建并迁移买入」**&#x529F;能仅支持 私钥导入以进行交易操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

在 PumpFun 联合曲线买入的钱包地址，最多支持 **9 个地址**捆绑买入。Dev 钱包买入数量和捆绑钱包买入数量需**大于 85 SOL**，以触发迁移程序。

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入钱包私钥的类型，选择以查看详细教程。

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「手动输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (429).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (401).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x4E00;行仅输入一个地址，按回车键换行

<figure><img src="../../../.gitbook/assets/image (402).png" alt=""><figcaption></figcaption></figure>

3.

    点&#x51FB;**「确定」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (433).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 点&#x51FB;**「上传文件」**&#x6309;钮，弹出文件上传窗口。

<figure><img src="../../../.gitbook/assets/image (431).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (251).png" alt=""><figcaption></figcaption></figure>

2. 导入钱包地址信息文件，显示地址信息\
   请通过 CiaoTool 模板文件导入，以确保私钥准确导入。

<figure><img src="../../../.gitbook/assets/image (247).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (432).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入买入金额

支&#x6301;**「逐一输入」「统一金额」和「百分比」三**种交易金额类型。

<figure><img src="../../../.gitbook/assets/image (439).png" alt=""><figcaption></figcaption></figure>

1. **逐一输入**

* 在输入框中，逐一输入买入金额数量
* 若填写数量，则按照填写的数量进行交易。
* 若未填写数量，则按照交易数量中  设置的数量进行交易。

2. **统一金额**\
   击转账数量上方&#x7684;**「统一输入」**&#x6309;钮，选&#x62E9;**「统一金额」，**&#x6240;有选钱包根据同一数量将代币全部兑换为指定代币。
3. **百分比**\
   点击转账数量上方&#x7684;**「统一输入」**&#x6309;钮，选&#x62E9;**「百分比」，**&#x6240;有选钱包根据当前余额的百分比，兑换为指定代币。
{% endstep %}

{% step %}
### 输入外盘买入钱包私钥

在代币迁移至 PumpSwap 时，狙击买入的钱包地址。并设置买入数量

<figure><img src="../../../.gitbook/assets/image (425).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 自定义服务

#### 自定义合约地址

<figure><img src="../../../.gitbook/assets/image (406).png" alt=""><figcaption></figcaption></figure>

打造你的个性化代币地址，设置代币地址，**额外收费 0.01 SOL。**

1. **以「pump」结尾：**
   * 代币地址以「pump」结尾
2. **自定义代币地址**
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

确认信息无误后，点击下&#x65B9;**「创建并迁移买入」**&#x6309;钮，并等待开盘完成。
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

<summary><strong>什么是 PumpFun 创建并迁移狙击？</strong></summary>

这是一套针对 Pump.fun 全生命周期深度定制的高阶自动化工具。它允许项目方通过一次操作，将“代币部署”、“多钱包内盘买入”以及“外盘首笔狙击”等多个阶段的指令聚合打包，确保代币在内盘发射与外盘流转的过程中实现无缝衔接。

</details>

<details>

<summary><strong>为什么要在同一区块内完成内盘部署与外盘狙击的聚合？</strong></summary>

因为代币从 Pump.fun 内盘毕业迁移至外盘的瞬间，极易被海量的外部狙击机器人监控并抢入低价筹码。将核心流程压缩在同一区块内进行捆绑打包，能够彻底阻断外部机器人在中间插入交易的空间，确保项目方的资金始终处于最优先的执行层级，有效防止被夹击或抢跑。

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

<summary><strong>如果开盘在链上执行失败，我的资金会受损吗？</strong></summary>

完全不会。该功能底层基于 Jito 的捆绑机制，具有严格的防损保护。如果遇到网络极度拥堵、节点响应延迟或未能成功打包，整组操作将被直接回滚。您的 SOL 本金将安全保留在原钱包中，不会产生部分买入、滑点磨损或资金卡住的风险，您可以调整参数后重新发起。

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
