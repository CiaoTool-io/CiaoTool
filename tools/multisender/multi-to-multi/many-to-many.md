---
description: >-
  批量处理多个钱包地址原生代币或 ERC-20
  合约代币的资金转账，模拟真实转账，有效打乱地址关联，优化气泡图检测，提升多地址资金管理效率，丰富您的资产管理策略。
metaLinks:
  alternates:
    - https://app.gitbook.com/s/b56FKZGe1viFi67H1pPQ/transfer/many-to-many
---

# EVM - 批量转账 | 多对多转账教程

{% hint style="info" %}
当前&#x662F;**「EVM - 多对多转账」**&#x6559;程页面以查看 **BSC、opBNB、Base、X Layer、IoTeX、Robinhood** 等 EVM 网络教程。

本教程演示基于 BSC（BNB Chain）功能页面，本功能 EVM 网络 CiaoTool 全链通用，请切换至对应公链进行一对多转账操作。

点击[**「Solana - 多对多转账」**](../../../chains/solana/multisender/many-to-many.md)查看 Solana 网络多对多转账教程。
{% endhint %}

## CiaoTool EVM 多对多转账是什么？ <a href="#definition" id="definition"></a>

<figure><img src="../../../.gitbook/assets/image (504).png" alt="CiaoTool EVM 多对多转账页面"><figcaption></figcaption></figure>

**CiaoTool EVM 多对多转账**是一款专为 BSC (BNB Smart Chain) 及 EVM 兼容生态打造的高阶并行资产流转与财务分发工具。它允许用户在单次操作中，将多个独立源钱包（发送方）中的原生代币（如 BNB）或任意 BEP-20 / ERC-20 标准代币，交叉且批量地发送至多个目标接收钱包。

相较于传统单向的「一转多」或「多转一」模式，该功能的核心机制在于「全方位交叉矩阵流转」。系统打破了地址映射的单一性限制，在底层自动建立多源头到多目标的交叉网状关系。这意味着：源地址 A 与源地址 B 可以同时向目标地址 A 打款；同理，源地址 A 与源地址 B 也可同时向目标地址 B 分发。此功能完美适配项目方在进行复杂的社区定向交叉奖励分发、多地址矩阵资金重组、防追踪深度混淆链上资金轨迹，或大规模测试账户退款等高度复杂的账本处理场景。

立即在 EVM 网络上，用 CiaoTool​ 批量转账功能进行多对多转账操作：

<table data-view="cards"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/BSC.png" alt="" data-size="line">BSC (BNB Chain)</td><td><a href="https://bsc.ciaotool.io/zh-Hans/transfer/many-to-many">https://bsc.ciaotool.io/zh-Hans/transfer/many-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/BSC.png" alt="" data-size="line">opBNB</td><td><a href="https://opbnb.ciaotool.io/zh-Hans/transfer/many-to-many">https://opbnb.ciaotool.io/zh-Hans/transfer/many-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/Base3.png" alt="" data-size="line">Base</td><td><a href="https://base.ciaotool.io/zh-Hans/transfer/many-to-many">https://base.ciaotool.io/zh-Hans/transfer/many-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/3 (1).png" alt="" data-size="line">X Layer</td><td><a href="https://xlayer.ciaotool.io/zh-Hans/transfer/many-to-many">https://xlayer.ciaotool.io/zh-Hans/transfer/many-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/IoTex.png" alt="" data-size="line">IoTeX</td><td><a href="https://iotex.ciaotool.io/zh-Hans/transfer/many-to-many">https://iotex.ciaotool.io/zh-Hans/transfer/many-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/BOT-2.png" alt="" data-size="line"> BOT</td><td><a href="https://bot.ciaotool.io/zh-Hans/transfer/many-to-many">https://bot.ciaotool.io/zh-Hans/transfer/many-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/Group 1261152954.png" alt="" data-size="line"> Robinhood</td><td><a href="https://rb.ciaotool.io/zh-Hans/transfer/many-to-many">https://rb.ciaotool.io/zh-Hans/transfer/many-to-many</a></td></tr></tbody></table>

***

## 为什么选择 CiaoTool EVM 多对多转账？ <a href="#advantage" id="advantage"></a>

处理跨越几十甚至上百个独立源地址到多目标地址的资金交叉分发，通常伴随着极高的操作失误率与私钥管理风险。CiaoTool 为 BSC 链上的复杂矩阵调拨构建了兼顾极简交互与绝对安全的执行防线：

**复杂矩阵一键执行**\
支持多个发送地址与多个接收地址同时参与转账，无需逐个钱包重复操作。一次配置即可批量完成复杂资金调拨，大幅提升多账户协同管理效率。

**百倍提升效率：**\
彻底免去人工频繁切换账号、复制粘贴地址与重复授权签名的繁琐流程，支持一键并发执行成百上千笔转账，实现链上资产的极速归集。 ​

**优化资金分布结构**\
通过多地址交叉转账与随机金额分配机制，有效打散单一路径的大额资金流向，使整体资金迁移更加自然，帮助优化链上地址之间的关联结构。

**灵活的矩阵配置：**\
支持通过 Excel 电子表格文件一键批量导入目标地址列表与对应的分发额度。支持自定义等额、定额或随机金额分配，完美适配复杂多变的空投策略与持币分布需求。 ​

**本地安全环境：**\
采用纯前端本地执行机制，私钥仅在本地环境中用于交易签名，在极速提升交易效率的同时，全方位保障多钱包资产的绝对安全。

***

## **图文指南 | EVM 批量转账 - 多对多转账**  <a href="#solana-one-to-multi-guide" id="solana-one-to-multi-guide"></a>

{% stepper %}
{% step %}
### **切换公链并绑定钱包**

点击右上角按钮，绑定支持 EVM 网络的钱包

<figure><img src="../../../.gitbook/assets/image (475).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择转账代币

选择代币或直接输入代币地址。

<figure><img src="../../../.gitbook/assets/image (479).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入发送钱包私钥

{% hint style="danger" %}
**「多对多转账」**&#x529F;能支持使用私钥导入以进行转账操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

{% hint style="info" %}
发送钱包数量需要和接收钱包数量保持一致
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入发送钱包私钥的类型，选择以查看详细教程。

{% tabs %}
{% tab title="手动输入" %}
直接在输入框中，输入 / 粘贴发送钱包私钥。每行仅输入一个地址

<figure><img src="../../../.gitbook/assets/image (505).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 点&#x51FB;**「上传文件」**&#x6309;钮，弹出文件上传窗口导入发送钱包私钥。

<figure><img src="../../../.gitbook/assets/image (506).png" alt=""><figcaption></figcaption></figure>

2. 使用 CiaoTool 模板文件导入，并保存确定导入并显示在输入框内。\
   点击下载并查看模板：

{% file src="../../../.gitbook/assets/EVM_privateKey_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (507).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 导入接收钱包地址

{% hint style="info" %}
发送钱包数量需要和接收钱包数量保持一致
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入接收地址的类型，选择以查看详细教程。

{% tabs %}
{% tab title="手动输入" %}
直接在输入框中，输入 / 粘贴接收钱包地址。每行仅输入一个地址

<figure><img src="../../../.gitbook/assets/image (511).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 点&#x51FB;**「上传文件」**&#x6309;钮，弹出文件上传窗口导入接收钱包地址。

<figure><img src="../../../.gitbook/assets/image (512).png" alt=""><figcaption></figcaption></figure>

2. 使用 CiaoTool 模板文件导入，并保存确定导入并显示在输入框内。\
   点击下载并查看模板：

{% file src="../../../.gitbook/assets/EVM_address_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (509).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入转账金额

支&#x6301;**「自定义」「全部数量」「固定数量」「固定留存」**&#x56DB;种转账金额类型。

<figure><img src="../../../.gitbook/assets/image (502).png" alt=""><figcaption></figcaption></figure>

1. **自定义输入**\
   在输入框中，逐一输入转账金额数量

* 若填写数量，则按照填写的数量进行转账。
* 若未填写数量，则按照发送数量中  设置的数量进行转账。

2. **全部数量**\
   所有钱包将余额内指定的代币全部发送到接收地址。
3. **固定数量**\
   所有钱包根据同一数量将指定代币全部发送到接收地址。
4. **固定留存**\
   所有钱包留存指定数量代币，其余全部数量发送到接收地址。
{% endstep %}

{% step %}
### 核对

点击下一步，核对发送信息，并查看状态栏。

<figure><img src="../../../.gitbook/assets/image (503).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下&#x65B9;**「发送」**&#x6309;钮，并等待转账程序完成。
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>什么是多对多批量转账？</strong></summary>

EVM 多对多批量转账工具是一款可视化服务工具。无需代码即可允许您同时从多个发送钱包向多个目标地址并发分发代币。通过网状交叉的转账模式，它能打破单一的资金轨迹，比手动操作更精准、更具隐蔽性。

</details>

<details>

<summary><strong>如何导入地址？</strong></summary>

你可以手动输入地址，也可以上传 Excel 文件导入目标地址列表，系统会自动识别并展示预览。

</details>

<details>

<summary><strong>是否支持不同地址转不同数量？</strong></summary>

可以。你可以为每个地址设置不同的转账数量，也可以设置统一的金额和制定金额分发给所有目标地址。

</details>

<details>

<summary><strong>操作是否安全？</strong></summary>

平台采用纯前端签名机制，您的私钥绝不会被上传或储存在任何服务器上，所有交易均在本地浏览器完成签名，从技术层面确保平台无法访问您的私钥。

</details>

<details>

<summary><strong>一次可以发送到多少个地址？</strong></summary>

得益于私钥导入的模式，多对多转账功能免除了逐一钱包签署的繁复工作，发送地址没有任何数量限制。

</details>

<details>

<summary><strong>可以同时转多种代币吗？</strong></summary>

当前版本支持选择单一代币进行批量转账；如需多种资产分发，可多次执行操作。

</details>

***

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
