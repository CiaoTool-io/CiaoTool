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

<figure><picture><source srcset="../../../.gitbook/assets/屏幕截图 2026-09-09 173516.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (934).png" alt="CiaoTool Solana Chain PumpFun 捆绑买入并狙击页面"></picture><figcaption></figcaption></figure>

PumpFun 捆绑并迁移买入是一款针对已在 Pump.fun 平台上线、但尚未完成流动性迁移的代币打造的高阶流动性调度程序。

与 meme 代币部署工具不同，该功能专注于“内盘向外盘跨越”的特定时刻。它允许项目方在代币运行的任意合适阶段，将两个核心动作通过 Jito 捆绑机制强行绑定，并在公链的同一个区块内原子性执行：

1. **多地址打满内盘：**&#x6D4B;算联合曲线的剩余额度，调度多个预设地址精准买入剩余份额，瞬间将进度推至 85 SOL 的毕业临界值，从而触发平台底层的自动迁移机制。
2. **外盘同步狙击：**&#x5728;官方将流动性池部署至 PumpSwap 的同一瞬间，预设的狙击钱包会在同区块内完成外盘的首笔买入。

立即在 PumpFun 上，用 CiaoTool​ 捆绑并迁移买入功能进行一键开盘操作：

{% embed url="https://ciaotool.io/zh-Hans/pump/bundled-graduate" %}

***

## 为什么选择 CiaoTool PumpFun 捆绑并迁移买入？

**CiaoTool 全网独家首创的核心底层功能。**&#x8BE5;功能代表了当前 Solana 链开盘管理的技术上限。对于需要绝对掌控项目从内盘到外盘全流程筹码分布、阻断任何外部狙击手干扰的团队而言，它构建了无懈可击的技术壁垒：

* **更广的场景覆盖：**&#x4F20;统的开盘工具往往在代币部署的瞬间就锁死了后续路线，而该功能无论代币最初是否通过 CiaoTool 发射，只要其仍处于内盘流转阶段，团队便可在开盘后的任意时刻灵活介入。
* **独家同区块聚合：**&#x4F20;统的满切与外盘买入是断裂的，导致外盘开盘瞬间极易被外部机器人低价抢筹。CiaoTool 独家通过同区块捆绑，实现内盘结算与外盘狙击的无缝衔接，彻底阻绝了外部恶意程序的插入空间。
* **策略执行的高自由度：**&#x5B8C;全不强制绑定发币动作。项目团队可以先在内盘进行早期的社区建设、筹码沉淀与盘口观察。待时机完全成熟时，随时调用该工具一键完成“满切与狙击”，大幅提升了运营周期的灵活性。
* **纯前端本地绝对安全：**&#x4E25;苛遵守本地化安全规范，所有参与矩阵调度的私钥和签名流程均在用户的浏览器本地环境安全运行。平台技术上不触碰、不上传任何敏感数据，从源头上保障资金的绝对安全。

***

## **技术实现示意**

### 传统发射代币

{% columns %}
{% column %}
多地址买入、迁移至 DEX 以及迁移后的买入交易分别广播、独立上链，无法保证执行顺序或进入相邻区块。

执行期间若有其他交易插入，可能改变代币价格，导致后续钱包的买入成本和实际获得数量发生变化。

在迁移时，极容易被机器人狙击抢跑，实际获得的代币数量减少，造成损失。
{% endcolumn %}

{% column %}
<figure><img src="../../../.gitbook/assets/Frame 1321314910.png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}
{% endcolumns %}

### 捆绑发射代币

{% columns %}
{% column %}
整体流程分为两个捆绑执行：

* **发射阶段**：将 8 个钱包的买入交易打包，按预设顺序在同一区块内连续执行，直接打满联合曲线，使代币进入迁移程序。
* **迁移阶段**：将迁移至 DEX 与指定钱包的买入交易再次打包，按预设顺序在同一区块内执行。

完美减少交易间隙及迁移过程中被其他交易插入的风险，提升发射与买入的执行一致性及上链优先级，提升利润空间。
{% endcolumn %}

{% column %}
<figure><img src="../../../.gitbook/assets/Frame 1321314911.png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}
{% endcolumns %}

***

***

## **图文指南**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角【连接钱包】按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (748).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 内盘钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入接收地址的类型，选择以查看详细教程。最多支持 **8 个地址**在联合曲线阶段捆绑买入。

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「批量输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (887).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x6BCF;行仅输入一个钱包私钥，可在私钥后追加数量。

```
privateKey, 300
```

<figure><img src="../../../.gitbook/assets/image (737).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 下载 CiaoTool 模板文件，并将信息导入到文件内。

<figure><img src="../../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

2. 点击![](<../../../.gitbook/assets/image (848).png>)**「导入文件」**&#x6309;钮，弹出文件上传窗口。
3. 点&#x51FB;**「确定导入」**，将所有地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入交易金额

支&#x6301;**「逐一输入」「输入金额」**&#x4E24;种交易金额类型。系统会实时获取当前联合曲线状态并计算打满所需数量，开发者钱包买入 + 捆绑钱包买入代币数量必须超过显示数。

<figure><img src="../../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

1. **逐一输入**\
   在输入框中，逐一输入交易金额数量。
2. **统一金额**\
   点击交易数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「输入金额」**&#x9009;项，所有地址将统一交易数量。
{% endstep %}

{% step %}
### 迁移狙击钱包

当代币迁移至外盘 PumpSwap 时，同步狙击的钱包私钥，获得底部筹码的同时活跃代币。

外盘买入数量没有限制。

<figure><img src="../../../.gitbook/assets/image (932).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Jito 小费设置

{% hint style="danger" %}
此功能实现依赖于 Jito 的捆绑功能。由于网络环境、Jito节点、RPC节点和区块处理引擎的复杂影响，该功能可能面临较高的失败率。

若操作失败，不会开盘成功也不会产生任何费用，请尝试更换RPC节点，区块处理引擎，增加Jito的小费(建议0.01SOL)，并考虑在链上活跃度较低的时段再次尝试。
{% endhint %}

通过 Jito 小费，将创建代币+多地址交易打包为一个捆绑包，确保交易不被狙击，并提升上链优先级，但需要消耗更多费用。

<figure><img src="../../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>
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
* 若遇 Solana 链上极度壅塞引发底层随机丢包，请直接避开交易尖峰时段，稍后再试。

***

## **常见问题**

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

## **寻求支持**

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
