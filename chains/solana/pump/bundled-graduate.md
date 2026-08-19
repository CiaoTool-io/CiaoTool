---
description: >-
  专为 Pump.fun
  平台已发行的代币打造的狙击工具。支持在代币发行后的任意阶段，将“多钱包买满内盘联合曲线”与“流动性迁移外盘时的首笔狙击”聚合在同一区块内执行，实现内盘毕业到外盘开盘的无缝筹码锁定。
---

# PumpFun - 捆绑并迁移买入教程

{% hint style="info" %}
**CiaoTool PumpFun 捆绑并迁移买入**现已全面支持官方 **SOL** 和 **USDC** 全部的价值代币，请先切换到指定代币页面进行捆绑买入及外盘狙击建仓操作，满足不同场景下的快捷狙击服务。
{% endhint %}

## CiaoTool PumpFun 捆绑并迁移买入是什么？

PumpFun 捆绑并迁移买入是一款针对已在 Pump.fun 平台上线、但尚未完成流动性迁移的代币打造的高阶流动性调度程序。

与 meme 代币部署工具不同，该功能专注于“内盘向外盘跨越”的特定时刻。它允许项目方在代币运行的任意合适阶段，将两个核心动作通过 Jito 捆绑机制强行绑定，并在公链的同一个区块内原子性执行：

1. **多地址打满内盘：**&#x6D4B;算联合曲线的剩余额度，调度多个预设地址精准买入剩余份额，瞬间将进度推至 85 SOL 的毕业临界值，从而触发平台底层的自动迁移机制。
2. **外盘同步狙击：**&#x5728;官方将流动性池部署至 PumpSwap 的同一瞬间，预设的狙击钱包会在同区块内完成外盘的首笔买入。

立即在 PumpFun 上，用 CiaoTool​ 捆绑并迁移买入功能进行一键开盘操作：

{% embed url="https://ciaotool.io/zh-CN/pump/bundled-graduate" %}

***

## 为什么选择 CiaoTool PumpFun 捆绑并迁移买入？

**CiaoTool 全网独家首创的核心底层功能。**&#x8BE5;功能代表了当前 Solana 链开盘管理的技术上限。对于需要绝对掌控项目从内盘到外盘全流程筹码分布、阻断任何外部狙击手干扰的团队而言，它构建了无懈可击的技术壁垒：

* **更广的场景覆盖：**&#x4F20;统的开盘工具往往在代币部署的瞬间就锁死了后续路线，而该功能无论代币最初是否通过 CiaoTool 发射，只要其仍处于内盘流转阶段，团队便可在开盘后的任意时刻灵活介入。
* **独家同区块聚合：**&#x4F20;统的满切与外盘买入是断裂的，导致外盘开盘瞬间极易被外部机器人低价抢筹。CiaoTool 独家通过同区块捆绑，实现内盘结算与外盘狙击的无缝衔接，彻底阻绝了外部恶意程序的插入空间。
* **策略执行的高自由度：**&#x5B8C;全不强制绑定发币动作。项目团队可以先在内盘进行早期的社区建设、筹码沉淀与盘口观察。待时机完全成熟时，随时调用该工具一键完成“满切与狙击”，大幅提升了运营周期的灵活性。
* **纯前端本地绝对安全：**&#x4E25;苛遵守本地化安全规范，所有参与矩阵调度的私钥和签名流程均在用户的浏览器本地环境安全运行。平台技术上不触碰、不上传任何敏感数据，从源头上保障资金的绝对安全。

***

## **图文指南 |** PumpFun 捆绑并迁移买入

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (396).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入代币地址

输入或选择您想要进行「捆绑并迁移买入」的代币地址，系统将自动获取该代币的曲线信息

<figure><img src="../../../.gitbook/assets/image (428).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入买入钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

**「捆绑并迁移买入」**&#x529F;能仅支持 私钥导入以进行交易操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

在 PumpFun 联合曲线买入的钱包地址，最多支持 **12 个地址**捆绑买入。捆绑钱包买入数量需**大于 曲线所需数量显示**，以触发迁移程序。

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入钱包私钥的类型，选择以查看详细教程。

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「手动输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (434).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (401).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x4E00;行仅输入一个地址，按回车键换行

<figure><img src="../../../.gitbook/assets/image (402).png" alt=""><figcaption></figcaption></figure>

3.

    点&#x51FB;**「确定」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (437).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 点&#x51FB;**「上传文件」**&#x6309;钮，弹出文件上传窗口。

<figure><img src="../../../.gitbook/assets/image (435).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (251).png" alt=""><figcaption></figcaption></figure>

2. 导入钱包地址信息文件，显示地址信息。\
   请通过 CiaoTool 模板文件导入，以确保私钥准确导入。

<figure><img src="../../../.gitbook/assets/image (247).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (436).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入买入金额

支&#x6301;**「逐一输入」「统一金额」和「百分比」**&#x4E09;种交易金额类型。

<figure><img src="../../../.gitbook/assets/image (438).png" alt=""><figcaption></figcaption></figure>

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
* 若遇 Solana 链上极度壅塞引发底层随机丢包，请直接避开交易尖峰时段，稍后再试。

***

## **常见问题 FAQ**

<details>

<summary><strong>“捆绑并迁移买入”与“创建并迁移买入”有什么本质区别？</strong></summary>

“创建并迁移买入”包含了代币的初始链上部署；而“捆绑并迁移买入”不包含发币操作，它专门服务于已经上线内盘且正在交易中的代币，允许项目方在开盘后的任意窗口期介入，为其提供后续的打满内盘与跨盘狙击服务。

</details>

<details>

<summary><strong>如果我的 Pump 代币不是通过 CiaoTool 发射的，还能使用这个功能吗？</strong></summary>

可以。只要目标代币当前仍处于 Pump.fun 的内盘流转阶段，无论其最初通过何种平台或代码部署，您都可以随时调用该功能执行同区块的捆绑买入与外盘狙击操作。

</details>

<details>

<summary><strong>打满内盘所需的资金是如何计算和分配的？</strong></summary>

系统会实时读取当前代币联合曲线的剩余进度。确保您导入的多捆绑买入钱包只需确保拥有充足的 SOL 余额（涵盖购买本金、预估滑点），以完成内盘捆绑买入指令。

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
