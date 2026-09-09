---
description: >-
  专为 Pump.fun 平台深度定制的代币首发、捆绑建仓与外盘狙击的一体化执行工具。支持在同一区块内瞬间完成代币创建、多钱包内盘买入，并在迁移至
  PumpSwap 的同时狙击建仓，全方位保障早期筹码的安全锁定与连续性策略执行。
---

# PumpFun - 创建并迁移买入教程

{% hint style="info" %}
**CiaoTool PumpFun 创建并迁移买入**现已全面支持官方 **SOL** 和 **USDC** 全部的价值代币
{% endhint %}

## CiaoTool PumpFun 创建并迁移买入是什么？

<figure><picture><source srcset="../../../.gitbook/assets/屏幕截图 2026-09-09 173554.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/屏幕截图 2026-09-09 173545.png" alt="CiaoTool Solana Chain Pump 创建并迁移买入页面"></picture><figcaption></figcaption></figure>

**CiaoTool PumpFun 创建并迁移买入**是一款将「创建代币部署」与「多阶段自动化买入」深度结合的高阶开盘与建仓工具。它打破了传统工具只能分段操作的局限，将“内盘诞生”到“外盘迁移”的整个核心跨度，压缩在公链的同一个区块内完成，旨在协助项目团队在代币发行的最初期，建立起兼顾防抢跑与筹码分散的自动化执行防线。

该功能将整个代币发射周期拆分为两个核心执行阶段：

1. **内盘捆绑阶段：**&#x7CFB;统在底层通过 Jito 捆绑机制，将部署代币的指令与首批独立买入钱包的指令无缝打包在同一个区块内。这确保了代币创建的瞬间，项目方设定的钱包能够抢先执行买入，打满联合曲线触发迁移机制，从而锁定联合曲线最底部的初始价格。
2. **迁移狙击阶段：**&#x5F53;官方将流动性迁移至 PumpSwap 的瞬间，预设的狙击钱包交易指令已在同区块的尾端严密锁死。这意味着在外盘资金池刚刚建立、外界狙击机器人甚至还没来得及同步到链上数据的瞬间，项目方的资金已经在外盘完成了首笔抢筹，完美跑通全生命周期的筹码闭环。

立即在 PumpFun 上，用 CiaoTool​ 创建并迁移买入功能进行一键开盘操作：

{% embed url="https://ciaotool.io/zh-Hans/pump/graduation-sniper" %}

***

## 为什么选择 CiaoTool PumpFun 创建并迁移买入？

**CiaoTool 全网独家首创的核心底层功能。**&#x8BE5;功能代表了当前 Solana 链开盘管理的技术上限。对于需要绝对掌控项目从内盘到外盘全流程筹码分布、阻断任何外部狙击手干扰的团队而言，它构建了无懈可击的技术壁垒：

* **独家全流程同区块聚合：**&#x901A;常代币从内盘毕业迁移到外盘开盘的瞬间，极易被海量外部狙击机器人通过监控抢入低价筹码并高位砸盘。CiaoTool 独家实现了发币、打满内盘、官方迁移、外盘首笔狙击在同一区块内聚合，外部机器人无法在中间插入任何交易，彻底废除外部机器人的抢跑空间。
* **消除内盘垃圾时间：**&#x5F53;代币在内盘流转时，极易吸引恶意波段盘，导致项目难以平稳毕业。该功能支持一键买满曲线，瞬间把代币推向外盘，消除内盘不确定性；同时确保团队分别锁定内盘曲线最底部及外盘开盘瞬间的绝对最优价格，将做市开盘损耗降至零点。
* **矩阵钱包自动化调度：**&#x4F20;统的跨盘做市需要团队在内盘达标后再去外盘抢开盘，极易因为网络延迟、节点速度差导致策略断层。通过 CiaoTool，完成多钱包资产配置，内盘买入份额测算以及外盘狙击额度分配，实现从「内盘创建」向「外盘狙击」的绝对连续性。
* **纯前端本地绝对安全：**&#x4E25;苛遵守本地化安全规范，所有参与矩阵调度的私钥和签名流程均在用户的浏览器本地环境安全运行。平台技术上不触碰、不上传任何敏感数据，从源头上保障资金的绝对安全。

***

## 视频教程

{% embed url="https://www.youtube.com/watch?v=Id8Wrebby_Y" %}

***

## **技术实现示意**

### 传统发射代币

{% columns %}
{% column %}
代币创建、多地址买入、迁移至 DEX 以及迁移后的买入交易分别广播、独立上链，无法保证执行顺序或进入相邻区块。

执行期间若有其他交易插入，可能改变代币价格，导致后续钱包的买入成本和实际获得数量发生变化。

在迁移时，极容易被机器人狙击抢跑，实际获得的代币数量减少，造成损失。
{% endcolumn %}

{% column %}
<figure><img src="../../../.gitbook/assets/Frame 1321314908.png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}
{% endcolumns %}

### 捆绑发射代币

{% columns %}
{% column %}
整体流程分为两个捆绑执行：

* **发射阶段**：将代币创建与 6 个钱包的买入交易打包，按预设顺序在同一区块内连续执行，直接打满联合曲线，使代币进入迁移程序。
* **迁移阶段**：将迁移至 DEX 与指定钱包的买入交易再次打包，按预设顺序在同一区块内执行。

完美减少交易间隙及迁移过程中被其他交易插入的风险，提升发射与买入的执行一致性及上链优先级，提升利润空间。
{% endcolumn %}

{% column %}
<figure><img src="../../../.gitbook/assets/Frame 1321314909.png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}
{% endcolumns %}

***

## **图文指南**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角【连接钱包】按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (748).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 填写代币信息

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**克隆：** 点击克隆按钮，克隆其他代币的信息。
{% endhint %}

* **代币名称：**&#x60A8;希望展示在钱包或区块浏览器中的完整代币名称（_例如：MyFirstToken_）。
* **代币简称：**&#x4EE3;币的缩写，通常为 3\~6 个大写字母（_例如：MYT_）。
* **LOGO：**&#x4E0A;传项目或代币的标志图像，建议尺寸 1000\*1000 像素。
* **描述：** 简要介绍代币用途、故事或 Meme 背景（选填）。
{% endstep %}

{% step %}
### 添加链接<mark style="color:$info;">（可选）</mark>

虽然为可选项，但强烈建议填写，**官网、X / Twitter、Telegram。**&#x589E;加项目可信度。

<figure><img src="../../../.gitbook/assets/image (13).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Mint 地址<mark style="color:$info;">（可选）</mark>

生成自定义代币地址，提升代币辨识度。

{% tabs %}
{% tab title="靓号地址" %}
可以设置希望出现在钱包地址开头或结尾的字符，例如以 `soL` 开头、以 `pump` 结尾，工具会持续生成随机密钥对，直到找到符合条件的地址。

<figure><img src="../../../.gitbook/assets/image (817).png" alt=""><figcaption></figcaption></figure>

详细工作原理及教程请查看

{% content-ref url="../wallet-tool/vanity-address.md" %}
[vanity-address.md](../wallet-tool/vanity-address.md)
{% endcontent-ref %}
{% endtab %}

{% tab title="自定义地址" %}
* 提前生成您想要的钱包地址，可以是靓号地址。
* 将你提前生成的私钥粘贴导入（**地址必须要全新地址且没有付过SOL租金**）；
* 系统将使用该地址部署你的代币，确保合约地址与预期一致。
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 创建参数

#### 报价代币

Pump.Fun 现支持 SOL 和 USDC 作为报价代币，点击切换选择。

#### Meyhem 模式

发币后 24 小时内，机器人随机买卖，增加交易活跃度和价格波动，不保证上涨。将额外发行 10 亿代币供机器人使用，结束后销毁其剩余持仓。

点击查看 [**PumpFun 详细规则**](https://pump.fun/docs/mayhem-mode-disclaimer)

#### 返现奖励

开启后，原本给发币者的创作者手续费会返还给交易者，按各自交易量累积领取；仅持币不产生返现。

点击查看 [**PumpFun 创作者费率**](https://pump.fun/docs/fees)
{% endstep %}

{% step %}
### 开发者钱包买入

即当前绑定钱包进行买入操作，不填默认为 0。在 GMGN、DEXScreener 等链上监控平台会被标记为 Dev 钱包。

<figure><img src="../../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 内盘钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入接收地址的类型，选择以查看详细教程。最多支持 **6 个地址**在联合曲线阶段捆绑买入。

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

支&#x6301;**「逐一输入」「输入金额」**&#x4E24;种交易金额类型。开发者钱包买入 + 捆绑钱包买入代币数量必须超过 86 SOL。

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
* 若因代币头像档案过大导致上传逾时，请将图片压缩至 1MB 以内再重新发起操作。
* 若遇 Solana 链上极度壅塞引发底层随机丢包，请直接避开交易尖峰时段，稍后再试。

***

## **常见问题**

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

## **寻求支持**

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
