---
description: 快速将单个地址中的代币分散至多个全新地址，降低前排持仓权重，优化链上分布结构，提升图表自然度和项目可信度。
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/b56FKZGe1viFi67H1pPQ/migration/assert-migration-cold
---

# EVM - 冷换仓教程

{% hint style="info" %}
当前&#x662F;**「EVM - 冷换仓」**&#x6559;程页面以查看 **BSC、Base、X Layer、IoTeX** 等 EVM 网络教程。

本教程演示基于 BSC（BNB Chain）功能页面，本功能 EVM 网络 CiaoTool 全链通用，请切换至对应公链进行冷换仓操作。

点击[**「Solana - 冷换仓」**](../../chains/solana/asset-migration/fragmentation.md)查看 Solana 网络冷换仓教程。
{% endhint %}

## CiaoTool EVM 冷换仓是什么？ <a href="#definition" id="definition"></a>

<figure><img src="../../.gitbook/assets/image (613).png" alt="CiaoTool BSC生态 冷换仓 功能页面"><figcaption></figcaption></figure>

**BSC 冷换仓，**&#x5728;区块链基础设施中被称为 Token 持仓打散与碎片化资产迁移，是指项目方或大额流动性持有者，在不通过中心化交易平台或去中心化交易池的前提下，通过智能合约并发转账技术，将原本集中在少数核心地址中的代币，按设定比例或随机均匀地分散分发到数百个完全独立的、全新生成的 BSC 原生钱包地址中的全自动链上行为。

在区块链浏览器的数据聚类分析中，持仓分布是外部评估项目生态成熟度、去中心化水平和社区健康度的核心指标。冷换仓能在极短的时间内优化链上筹码气泡图的分布，显著增强项目的去中心化底层数据表现。

冷换仓机制贯穿代币运营的全生命周期，是专业 Web3 project 矩阵规范化运作的基石：

* Token 上线前的生态初始化：\
  在代币发行后、正式注入 PancakeSwap 流动性池之前，将初始发行的代币合理分散至不同梯队的项目库房与早期贡献者账户，构建健康的代币经济学持仓结构。
* 筹码气泡图优化： \
  针对第三方链上聚类分析工具，切断中心化巨鲸地址的强关联特征，美化前排持币占比。
* 大规模链上分仓建仓储备： \
  提前为自动市值管理或长线流动性引导机器人储备好足额、高隔离性的分散子钱包账户基础，避免单一核心钱包暴露带来的财务集中风险。

立即在 EVM 网络上，用 CiaoTool​ 冷换仓功能进行持仓打散与碎片化资产迁移操作：

<table data-view="cards"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td><img src="../../.gitbook/assets/BSC.png" alt="" data-size="line">BSC (BNB Chain)</td><td><a href="https://bsc.ciaotool.io/zh-Hans/assert-migration/assert-migration-cold">https://bsc.ciaotool.io/zh-Hans/assert-migration/assert-migration-cold</a></td></tr><tr><td><img src="../../.gitbook/assets/Base3.png" alt="" data-size="line">Base</td><td><a href="https://base.ciaotool.io/zh-Hans/assert-migration/assert-migration-cold">https://base.ciaotool.io/zh-Hans/assert-migration/assert-migration-cold</a></td></tr><tr><td><img src="../../.gitbook/assets/3 (1).png" alt="" data-size="line">X Layer</td><td><a href="https://xlayer.ciaotool.io/zh-Hans/assert-migration/assert-migration-cold">https://xlayer.ciaotool.io/zh-Hans/assert-migration/assert-migration-cold</a></td></tr><tr><td><img src="../../.gitbook/assets/IoTex.png" alt="" data-size="line">IoTeX</td><td><a href="https://iotex.ciaotool.io/zh-Hans/assert-migration/assert-migration-cold">https://iotex.ciaotool.io/zh-Hans/assert-migration/assert-migration-cold</a></td></tr><tr><td><img src="../../.gitbook/assets/Group 1261152954.png" alt="" data-size="line"> Robinhood</td><td><a href="https://robinhood.ciaotool.io/zh-Hans/assert-migration/assert-migration-cold">https://robinhood.ciaotool.io/zh-Hans/assert-migration/assert-migration-cold</a></td></tr></tbody></table>

***

## 为什么选择 CiaoTool 执行 BSC 冷换仓？ <a href="#advantage" id="advantage"></a>

在资产高速流转的区块链网络中，分仓的速度与私钥的底层安全决定了操作的成败。CiaoTool 为专业团队构筑了极致安全的链上运营防线： ​

**极致削减成本：**\
通过底层智能合约的多重调用与批量打包技术，将多笔转账聚合为单次链上交互，最大程度摊薄网络费用，显著降低大规模分发的资金损耗。 ​

**本地安全环境：**\
采用纯前端本地执行机制，私钥仅在本地环境中用于交易签名，在极速提升交易效率的同时，全方位保障多钱包资产的绝对安全。

***

## **图文指南 | EVM 冷换仓** <a href="#solana-one-to-multi-guide" id="solana-one-to-multi-guide"></a>

{% stepper %}
{% step %}
### **切换公链并绑定钱包**

点击右上角按钮，绑定支持 EVM 网络的钱包

<figure><img src="../../.gitbook/assets/image (475).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择转账代币

可以输入代币地址，也可以选择代币进行换仓。

<figure><img src="../../.gitbook/assets/image (479).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入换仓钱包

{% hint style="danger" %}
**「冷换仓」**&#x529F;能支持使用当前钱包和私钥导入以进行换仓操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../security-guide.md)**。**
{% endhint %}

导入需要换仓的钱包地址，支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入接收地址的类型，选择以查看详细教程。

{% tabs %}
{% tab title="手动输入" %}
直接在输入框中，输入 / 粘贴钱包私钥。每行仅输入一个钱包私钥

<figure><img src="../../.gitbook/assets/image (616).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 点&#x51FB;**「上传文件」**&#x6309;钮，弹出文件上传窗口导入换仓钱包私钥。

<figure><img src="../../.gitbook/assets/image (614).png" alt=""><figcaption></figcaption></figure>

2. 使用 CiaoTool 模板文件导入，并保存确定导入并显示在输入框内。\
   点击下载并查看模板：

{% file src="../../.gitbook/assets/EVM_privateKey_demo.xlsx" %}

<figure><img src="../../.gitbook/assets/image (615).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入换仓地址数量

输入每个钱包换仓碎片化的地址数量，每个钱包将所有指定代币转账到该数量钱包内。一个地址最多支持换仓碎片化至 **200 个新地址。**

点击「开始创建」，系统会自动下载所有碎片化新地址。若没有自动下载，您也可点击「下载表格」手动下载所有新地址。

<figure><img src="../../.gitbook/assets/image (618).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入转账金额

支&#x6301;**「自定义」「全部数量」「固定数量」「固定留存」**&#x56DB;种转账金额类型。

<figure><img src="../../.gitbook/assets/image (619).png" alt=""><figcaption></figcaption></figure>



1. **自定义输入**\
   在输入框中，逐一输入转账金额数量

* 若填写数量，则按照填写的数量进行转账。
* 若未填写数量，则按照发送数量中 设置的数量进行转账。

2. **全部数量**\
   所有钱包将余额内指定的代币全部碎片化转账到换仓地址。
3. **固定数量**\
   所有钱包根据同一数量将指定代币全部碎片化转账到换仓地址。
4. **固定留存**\
   所有钱包留存指定数量代币，其余全部数量碎片化转账到换仓地址。
{% endstep %}

{% step %}
### 确认交易

<figure><img src="../../.gitbook/assets/image (620).png" alt=""><figcaption></figcaption></figure>

确认信息无误后，点击下&#x65B9;**「发送」**&#x6309;钮，并等待转账程序完成。
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>冷换仓的作用是什么？</strong></summary>

冷换仓可将代币从当前地址分散转移至大量新地址，降低单一地址持仓比例，优化链上分布结构，增强项目安全性和隐蔽性。

</details>

<details>

<summary><strong>为什么换仓后要使用新生成的钱包地址？</strong></summary>

新地址无历史交易记录，可避免被链上工具标记为“关联钱包”，更适合用于策略重建和分散操作。

</details>

<details>

<summary><strong>操作是否安全？</strong></summary>

平台采用纯前端签名机制，您的私钥绝不会被上传或储存在任何服务器上，所有交易均在本地浏览器完成签名，从技术层面确保平台无法访问您的私钥。

</details>

<details>

<summary><strong>可以同时换仓多种代币吗？</strong></summary>

当前版本支持选择单一代币进行碎片化换仓；如需多种资产分发，可多次执行操作。

</details>

***

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
