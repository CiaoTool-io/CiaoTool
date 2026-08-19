---
description: >-
  专为 Flap.sh
  平台提供的代币发行与多地址捆绑买入工具。支持在同区块内同步完成代币创建、首笔批量买入与迁移外盘狙击，有效阻断机器人抢跑，支持税费经济。确保以极低初始成本安全建仓并优化早期持币分布。
metaLinks:
  alternates:
    - https://app.gitbook.com/s/b56FKZGe1viFi67H1pPQ/flap/usd1-create-and-buy
---

# Flap - 创建并买入教程

{% hint style="info" %}
**CiaoTool Flap 创建并买入**现已全面支持官方 **BNB、USD1、UUSD、USDT**  和 **RWA** 全部的价值代币，请先切换到指定代币页面进行创建代币并捆绑买入操作，满足不同场景下的快捷开盘服务。
{% endhint %}

## CiaoTool Flap 创建并买入是什么？

<figure><img src="../../../.gitbook/assets/image (456).png" alt="CiaoTool Flap.sh 创建并买入页面"><figcaption></figcaption></figure>

**CiaoTool Flap 创建并买入**功能将「创建代币部署」与「多阶段自动化买入」深度结合的高阶开盘与建仓工具。它打破了传统工具只能分段操作的局限，将「内盘诞生」到「外盘迁移」的整个核心跨度，压缩在公链的同一个区块内完成，旨在协助项目团队在代币发行的最初期，建立起兼顾防抢跑与筹码分散的自动化执行防线。

该功能将整个代币发射周期拆分为两个核心执行阶段：

1. **内盘捆绑阶段：**&#x7CFB;统在底层通过捆绑机制，将部署代币的指令与首批独立买入钱包的指令无缝打包在同一个区块内。这确保了代币创建的瞬间，项目方设定的钱包能够抢先执行买入，打满联合曲线触发迁移机制，从而锁定联合曲线最底部的初始价格。
2. **迁移狙击阶段：**&#x5F53;官方将流动性迁移至 PancakeSwap 的瞬间，预设的狙击钱包交易指令已在同区块的尾端严密锁死。这意味着在外盘资金池刚刚建立、外界狙击机器人甚至还没来得及同步到链上数据的瞬间，项目方的资金已经在外盘完成了首笔抢筹，完美跑通全生命周期的筹码闭环。

立即在 Flap 上，用 CiaoTool​ 创建并买入功能进行一键开盘操作：

{% embed url="https://bsc.ciaotool.io/zh-Hans/flap/bnb/create-and-buy" %}

***

## 为什么选择 CiaoTool Flap 创建并买入？

**CiaoTool 全网独家首创的核心底层功能。**&#x8BE5;功能代表了当前 BSC 链开盘管理的技术上限。对于需要绝对掌控项目从内盘到外盘全流程筹码分布、阻断任何外部狙击手干扰的团队而言，它构建了无懈可击的技术壁垒：

* **独家全流程聚合：**\
  通常代币从内盘毕业迁移到外盘开盘的瞬间，极易被海量外部狙击机器人通过监控抢入低价筹码并高位砸盘。CiaoTool 独家实现了发币、打满内盘、官方迁移、外盘首笔狙击在同一区块内聚合，外部机器人无法在中间插入任何交易，彻底废除外部机器人的抢跑空间。
* **锁定极低成本：**\
  确保多钱包买入指令作为创世区块的首批交易执行，使项目方能够以绝对的初始低价完成建仓，最大程度降低资金损耗。
* **优化早期分布：**\
  支持自定义配置多个独立地址同步买入，在代币发射的瞬间即完成基础的持币者结构分散，美化早期链上数据。
* **全自动极速部署：**\
  一键自动完成代币信息上传、参数配置与多地址资产分发，彻底免去繁琐的人工切换与手动抢筹操作。
* **矩阵钱包自动化调度：**\
  传统的跨盘做市需要团队在内盘达标后再去外盘抢开盘，极易因为网络延迟、节点速度差导致策略断层。通过 CiaoTool，完成多钱包资产配置，内盘买入份额测算以及外盘狙击额度分配，实现从「内盘创建」向「外盘狙击」的绝对连续性。
* **纯前端本地绝对安全：**\
  严苛遵守本地化安全规范，所有参与矩阵调度的私钥和签名流程均在用户的浏览器本地环境安全运行。平台技术上不触碰、不上传任何敏感数据，从源头上保障资金的绝对安全。

***

## **图文指南 | Flap** 创建并买入&#x20;

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 BSC 链的钱包

<figure><img src="../../../.gitbook/assets/image (446).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入支付钱包私钥

输入用于发币的控制地址私钥，该地址将会作为 Four 创建代币的代币开发者地址，以及支付功能服务费用。

<figure><img src="../../../.gitbook/assets/image (653).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 填写代币基础信息

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

当&#x524D;**「创建并买入」**&#x529F;能仅支持 私钥导入以进行开盘操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (458).png" alt=""><figcaption></figcaption></figure>

* **代币名称：**&#x60A8;希望展示在钱包或区块浏览器中的完整代币名称（_例如：MyFirstToken_）。
* **简称：**&#x4EE3;币的缩写，通常为 3\~6 个大写字母（_例如：MYT_）。
* **LOGO：**&#x4E0A;传项目或代币的标志图像，建议尺寸 1000\*1000 像素。
* **描述：**&#x975E;必填项，简要介绍项目的背景、目标和用途。此描述将帮助用户理解您的代币的功能和项目愿景，提高项目真实性。
* **社交链接：**&#x867D;为可选项但强烈建议填写，**官网、X / Twitter、Telegram**，有助于用户关注和加入您的项目社区。
{% endstep %}

{% step %}
### Dev 钱包买入

{% hint style="warning" %}
<mark style="color:$warning;">**钱包设置**</mark>

Dev 钱包、内盘钱包、外盘钱包不能共用，所有业务私钥必须唯一
{% endhint %}

用代币开发者钱包买入的代币数量，链上监控平台会显示为开发者买入。不填默认为 0。

<figure><img src="../../../.gitbook/assets/image (450).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 设置代币税费

{% hint style="info" %}
Flap 主网当前仅开放含税代币（Tax Token V3）创建，最新非税代币（newTokenV7）适配完成前暂不可用。
{% endhint %}

CiaoTool 现已支持 Flap 最新税费功能，方便快捷打造专属代币经济学。不同于 Fourmeme，Flap 的交易税费在联合曲线阶段即开始生效。

<figure><img src="../../../.gitbook/assets/image (459).png" alt=""><figcaption></figcaption></figure>

* **营销税率**：交易中指定额度的代币将会自动转入指定的营销钱包中，用于进行其他营销活动。
* **分红税率**：交易中指定额度的代币会按持币比例分配给所有持币者，实现持币分红。
* **分红门槛：**&#x53EA;有持币数量达到持有门槛的持币者，才能开始享受分红税费带来的额外分红，吸引交易者持有更多代币，增强长期持有信心。最低门槛为 10000。
* **销毁税率**：交易中指定额度的代币将会被打入黑洞地址，变相实现通缩机制，变相拉升代币价值。
* **回流税率**：交易中指定额度的代币将会自动添加到流动池内，保证交易始终存在流动性。
{% endstep %}

{% step %}
### 导入内盘买入钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

当&#x524D;**「创建并买入」**&#x529F;能仅支持 私钥导入以进行多地址交易操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

{% hint style="warning" %}
<mark style="color:$warning;">**钱包设置**</mark>

外盘要同步捆绑买入时，内盘捆绑钱包数量必须 ≥ 2。\
Dev 钱包、内盘钱包、外盘钱包不能共用，所有业务私钥必须唯一。
{% endhint %}

内盘钱包设置，即代币创建在 Flap.sh 联合曲线时，同步买入的钱包地址

1. 点&#x51FB;**「导入私钥」**&#x6309;钮，弹出上传弹窗。

<figure><img src="../../../.gitbook/assets/image (460).png" alt=""><figcaption></figcaption></figure>

2. 支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入钱包私钥的类型，最多支持 **20 个地址**捆绑买入。

<figure><img src="../../../.gitbook/assets/image (453).png" alt=""><figcaption></figcaption></figure>

使用 CiaoTool 模板文件导入，并保存确定导入并显示在输入框内。\
点击下载并查看模板：

{% file src="../../../.gitbook/assets/EVM_privateKey_demo.xlsx" %}

3. 系统将自动读取每个私钥的 **BNB 余额，**&#x5E76;输入买入金额

{% hint style="danger" %}
买入地址的 BNB 余额必须大于 0.0008，以预留支付 Gas 等网络费用；

当选择 MAX 时，系统将自动预留 0.001 BNB 左右的余额于钱包内，您可手动调整范围。
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (461).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入外盘买入钱包私钥<sub><mark style="color:$info;">（可选）<mark style="color:$info;"></sub>

{% hint style="danger" %}
当&#x524D;**「创建并买入」**&#x529F;能仅支持 私钥导入以进行多地址交易操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

{% hint style="warning" %}
<mark style="color:$warning;">**钱包设置**</mark>

外盘要同步捆绑买入时，内盘捆绑钱包数量必须 ≥ 2。

Dev 钱包、内盘钱包、外盘钱包不能共用，所有业务私钥必须唯一
{% endhint %}

外盘钱包设置，即代币在 Flap.sh 联合曲线被打满毕业迁移至 PancakeSwap 时，同步买入的钱包地址。最多支持 **5 个**钱包于外盘捆绑买入。

若要在 Flap.sh 上创建代币时，外盘同步捆绑买入，**必须要让【Dev 钱包 + 内盘钱包】买入数量大于 16.16 BNB 以触发毕业迁移机制**，否则将会导致程序失败。

由于 Flap.sh 官方合约代码限制，外盘同步捆绑狙击**必须使用 WBNB 进行买入操作**，请提前将原生 BNB 代币兑换为 WBNB 以满足功能运行需要。但您仍需确保 BNB 余额大于 0.0008 以支付 Gas 等网络费用。
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下&#x65B9;**「创建并买入」**&#x6309;钮，并等待开盘完成。
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>什么是 Flap 创建并买入？</strong></summary>

这是一套针对 Flap.sh 全生命周期深度定制的高阶自动化工具。它允许项目方通过一次操作，将「代币部署」、「多钱包内盘买入」以及「外盘狙击」等多个阶段的指令聚合打包，确保代币在内盘发射与外盘流转的过程中实现无缝衔接。

</details>

<details>

<summary><strong>为什么要在同一区块内完成内盘部署与外盘狙击的聚合？</strong></summary>

因为代币从 Flap.sh 内盘毕业迁移至外盘的瞬间，极易被海量的外部狙击机器人监控并抢入低价筹码。将核心流程压缩在同一区块内进行捆绑打包，能够彻底阻断外部机器人在中间插入交易的空间，确保项目方的资金始终处于最优先的执行层级，有效防止被夹击或抢跑。

</details>

<details>

<summary><strong>这项功能可以用来优化代币早期的持币结构吗？</strong></summary>

可以。由于该功能支持批量导入多个钱包地址同步执行买入，这些买入会在代币创建的瞬间独立完成。这能让代币在刚发布时就展现出健康、分散的持币者分布数据，避免筹码过于集中在单一地址中。

</details>

<details>

<summary><strong>如果开盘在链上执行失败，我的资金会受损吗？</strong></summary>

完全不会。该功能底层基于捆绑机制，具有严格的防损保护。如果遇到网络极度拥堵、节点响应延迟或未能成功打包，整组操作将被直接回滚。您的本金将安全保留在原钱包中，不会产生部分买入、滑点磨损或资金卡住的风险，您可以调整参数后重新发起。

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
