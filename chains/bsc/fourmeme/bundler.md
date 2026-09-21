---
description: >-
  专为 Four.meme
  平台提供的代币发行与多地址捆绑买入工具。支持在同区块内同步完成代币创建、首笔批量买入与迁移外盘狙击，有效阻断机器人抢跑，支持税费经济。确保以极低成本建仓并优化早期持币分布。
metaLinks:
  alternates:
    - https://app.gitbook.com/s/b56FKZGe1viFi67H1pPQ/fourmeme/bnb-create-and-buy
---

# Fourmeme - 创建并买入指南

{% hint style="info" %}
**CiaoTool Fourmeme 创建并买入**现已全面支持官方 **BNB、USD1、UUSD 和 RWA** 全部的价值代币，请先切换到指定代币页面进行创建代币并捆绑买入操作，满足不同场景下的快捷开盘服务。
{% endhint %}

## 功能介绍

**CiaoTool Fourmeme 创建并迁移买入**是一款专为 BSC 生态 **Four.meme 平台**打造的代币发行与自动化建仓工具。覆盖代币创建、联合曲线买入及迁移后买入的两阶段自动化工具，可减少跨阶段手动操作与交易等待。

整个流程由两个独立捆绑包组成：

1. **创建与内盘买入：** 将代币创建和多个钱包的捆绑包买入交易按预设顺序打包，正常情况下在同一区块内连续执行。
2. **迁移与外盘买入：** 达到毕业条件后，将迁移至 PancakeSwap 和多个钱包的买入交易组成新的捆绑，正常情况下在同一区块内依次执行。

立即在 Fourmeme 上，用 CiaoTool​ 创建并买入功能进行一键开盘操作：

{% embed url="https://bsc.ciaotool.io/zh-Hans/fourmeme/bnb/create-and-buy" %}

***

## 核心优势

* **创建买入一体化：** 一次配置代币信息和各钱包买入金额
* **支持 Open 模式：** 独家支持最新 OpenFour，启用不同模板。
* **税费支持：**&#x652F;持最新税费代币，打造专属代币经济学。
* **外盘狙击：**&#x72EC;家外盘狙击，可选开盘即打满内盘，并在迁移时多地址狙击外盘。
* **多钱包配置：** 支持分别设置参与钱包及买入金额
* **自动化执行：** 完成资料上传、交易构建、钱包签名和 Bundle 提交

***

## 视频教程

{% embed url="https://www.youtube.com/watch?v=0w2oKTzzyoQ" %}

***

## **图文指南**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 BSC 链的钱包

<figure><img src="../../../.gitbook/assets/image (446).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 支付钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

输入用于发币的控制地址私钥，该地址将会作为 Four 创建代币的代币开发者地址，以及支付功能服务费用。

<figure><img src="../../../.gitbook/assets/image (653).png" alt=""><figcaption></figcaption></figure>
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
### 填写代币信息

<figure><img src="../../../.gitbook/assets/image (598).png" alt=""><figcaption></figcaption></figure>

* **代币名称：**&#x60A8;希望展示在钱包或区块浏览器中的完整代币名称（_例如：MyFirstToken_）。
* **简称：**&#x4EE3;币的缩写，通常为 3\~6 个大写字母（_例如：MYT_）。
* **LOGO：**&#x4E0A;传项目或代币的标志图像，建议尺寸 1000\*1000 像素。
* **描述：**&#x975E;必填项，简要介绍项目的背景、目标和用途。此描述将帮助用户理解您的代币的功能和项目愿景，提高项目真实性。
{% endstep %}

{% step %}
### Open 模式

全面支持 OpenFour 模板，让代币采用不同的发行、交易、分红、流动性或激励机制。

点击切换查看详情：

{% tabs %}
{% tab title="Royalty" %}
从交易税费中向创作者、社区或指定金库分配版税。

支持以下功能：

* [x] 募集代币支持：BNB / NVDAB / SPCXB / QQQB / GMEB / FLNCB / DJTB / MRNAB / HOODB
* [x] 代币税费
* [x] 反狙击
* [x] 内盘捆绑买入

该板块下，代币税费中，接收钱包分配比例必须 ＞10%，分红最低持币数量为 1。
{% endtab %}

{% tab title="Creator Incentives" %}
根据规则奖励代币创建者。创作者手续费随市值变化，在 **0.02%～1%** 的范围内动态调整，初期较低，随着市值增长逐渐提高。

支持以下功能：

* [x] 募集代币支持：BNB
* [x] 反狙击
* [x] 内盘捆绑买入
{% endtab %}

{% tab title="Likwid DEX" %}
代币毕业后迁移至 Likwid DEX，通过其统一流动性体系支持兑换、借贷，以及杠杆做多、做空等功能。

支持以下功能：

* [x] 募集代币支持：BNB
* [x] 反狙击
* [x] 内盘捆绑买入
{% endtab %}

{% tab title="Cubepeg" %}
Cubepeg 将可交易代币和 NFT 权益关联起来。每持有 100,000 枚代币对应 1 个 NFT，卖出代币时相关 NFT 也会按机制销毁。

* 用 NFT 展示持币身份。
* 将社区角色、收藏形象与持仓关联。
* 围绕持仓构建游戏或会员玩法。

支持以下功能：

* [x] 募集代币支持：BNB
* [x] 反狙击
* [x] 内盘捆绑买入
{% endtab %}

{% tab title="ListaYield" %}
ListaYield 将交易税费分配与 Lista 质押金库结合。符合条件的持有人获得的是**金库份额代币**，毕业后迁移至 ListaDEX。

* [x] 募集代币支持：BNB
* [x] 代币税费
* [x] 反狙击
* [x] 内盘捆绑买入
{% endtab %}

{% tab title="4STOCK" %}
将真实股票以 1:1 资产支持引入 BNB Chain，用于链上交易及作为股票主题 Meme 币的底池资产。

支持以下功能：

* [x] 募集代币支持：BNC4
* [x] 代币税费
* [x] 反狙击
* [x] 内盘捆绑买入
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 设置代币税费<sub><mark style="color:$info;">（可选）<mark style="color:$info;"></sub>

CiaoTool 现已支持 Fourmeme 最新税费功能，方便快捷打造专属代币经济学。交易税费将会在代币打满联合曲线并迁移至 DEX 之后生效。

<figure><img src="../../../.gitbook/assets/image (459).png" alt=""><figcaption></figcaption></figure>

* **营销税率**：交易中指定额度的代币将会自动转入指定的营销钱包中，用于进行其他营销活动。
* **分红税率**：交易中指定额度的代币会按持币比例分配给所有持币者，实现持币分红。
* **分红门槛：**&#x53EA;有持币数量达到持有门槛的持币者，才能开始享受分红税费带来的额外分红，吸引交易者持有更多代币，增强长期持有信心。最低门槛为 10000。
* **销毁税率**：交易中指定额度的代币将会被打入黑洞地址，变相实现通缩机制，变相拉升代币价值。
* **回流税率**：交易中指定额度的代币将会自动添加到流动池内，保证交易始终存在流动性。
{% endstep %}

{% step %}
### 添加社交链接

虽为可选项但强烈建议填写，**官网、X / Twitter、Telegram**，有助于用户关注和加入您的项目社区。
{% endstep %}

{% step %}
### 选择项目标签

* 从以下标签中选择适合你项目的定位，让其他用户更容易理解项目的方向和应用场景，系统不支持多选：

`Meme / AI / DeFi / Game / Infra / DeSci / Social / DePin / Charity / Others`

**示例用法：**&#x4F60;发的是狗狗币类 Meme，可选「Meme」；如果未来要做 NFT 或 Game 叙事，也可同步选「Game」。
{% endstep %}

{% step %}
### 内盘钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

{% hint style="warning" %}
<mark style="color:$warning;">**钱包设置**</mark>

Dev 钱包、内盘钱包、外盘钱包不能共用，所有业务私钥必须唯一
{% endhint %}

在联合曲线阶段捆绑买入的钱包，最多支持 20 个钱包捆绑买入。

1. 点&#x51FB;**「导入私钥」**&#x6309;钮，弹出上传弹窗。

<figure><img src="../../../.gitbook/assets/image (460).png" alt=""><figcaption></figcaption></figure>

2. 支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入钱包私钥的类型，最多支持 **20 个地址**捆绑买入。

<figure><img src="../../../.gitbook/assets/image (453).png" alt=""><figcaption></figcaption></figure>

使用 CiaoTool 模板文件导入，并保存确定导入并显示在输入框内。\
点击下载并查看模板：

{% file src="../../../.gitbook/assets/EVM_privateKey_demo.xlsx" %}
{% endstep %}

{% step %}
### 内盘买入金额

为每个地址设置**买入金额**，如只需捆绑买入联合曲线，所有地址总买入数量不得超过 18.18 BNB 或对应价值代币数额。

买入地址的 BNB 余额必须大于 0.0011，以预留支付 Gas 等网络费用；

当选择 MAX 时，系统将自动预留 0.0011 BNB 左右的余额于钱包内。
{% endstep %}

{% step %}
### 外盘钱包私钥<mark style="color:$info;">（可选）</mark>

{% hint style="warning" %}
<mark style="color:$warning;">**钱包设置**</mark>

Dev 钱包、内盘钱包、外盘钱包不能共用，所有业务私钥必须唯一
{% endhint %}

在迁移阶段捆绑买入的钱包，最多支持 5 个钱包捆绑买入。

{% hint style="info" %}
启动外盘迁移并多钱包狙击，需保证内盘（Dev 钱包 + 内盘钱包）买入数量大于规定值。
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (937).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 外盘买入金额

为迁移阶段的每个地址设置**买入金额**，金额数量没有限制。
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下&#x65B9;**「创建并买入」**&#x6309;钮，并等待开盘完成。
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>什么是 Fourmeme 创建并买入？</strong></summary>

这是专为 BSC (BNB Chain) 生态的 Fourmeme 发射平台打造的一体化部署与建仓工具。它支持在可视化界面中一键完成代币创建，并在代币部署上链的绝对初始区块内，自动联动多个预设钱包同步执行买入，实现代币上线与初始建仓的同步。

</details>

<details>

<summary><strong>为什么要将“创建”和“买入”捆绑在一起执行？</strong></summary>

Four.meme 采用联合曲线定价机制，代币价格会随着买入量的增加而迅速上涨。如果先发币再手动买入，中间产生的时间差极易被链上狙击机器人监控并抢先买入，导致您被迫以数倍的高价接盘。捆绑执行消除了时间差，彻底阻断了恶意抢跑，保护了初始建仓的资金成本。

</details>

<details>

<summary><strong>这项功能可以用来优化代币早期的持币结构吗？</strong></summary>

可以。由于该功能支持批量导入多个钱包地址同步执行买入，这些买入会在代币创建的瞬间独立完成。这能让代币在刚发布时就展现出健康、分散的持币者分布数据，避免筹码过于集中在单一地址中。

</details>

<details>

<summary><strong>为什么“创建并买入”操作会提示失败？</strong></summary>

根据 Four.meme 的规则，同一个代币名称只能有一种代币。如果代币名称一样，则无法创建。

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
