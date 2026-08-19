---
description: 方便快捷地将分散在多个账户中的原生代币或 ERC-20 代币统一归集到一个主账户，提高资金管理的效率，同时减少交易成本和时间。
metaLinks:
  alternates:
    - https://app.gitbook.com/s/b56FKZGe1viFi67H1pPQ/transfer/many-to-one
---

# EVM - 批量转账 | 多对一转账教程

{% hint style="info" %}
当前&#x662F;**「EVM - 多对一转账」**&#x6559;程页面以查看 **BSC、opBNB、Base、X Layer、IoTeX、Robinhood** 等 EVM 网络教程。

本教程演示基于 BSC（BNB Chain）功能页面，本功能 EVM 网络 CiaoTool 全链通用，请切换至对应公链进行一对多转账操作。

点击[**「Solana - 多对一转账」**](../../../chains/solana/multisender/many-to-one.md)查看 Solana 网络多对一转账教程。
{% endhint %}

## CiaoTool EVM 多对一转账是什么？ <a href="#definition" id="definition"></a>

<figure><img src="../../../.gitbook/assets/image (497).png" alt=""><figcaption></figcaption></figure>

**CiaoTool EVM 多对一转账**是一款专为 BSC (BNB Smart Chain) 及 EVM 兼容生态打造的高效链上资产回笼与多钱包资金管理工具。它允许用户在单次可视化操作中，将分散在成百上千个子钱包中的指定代币或原生代币（如 BNB），全自动地集中汇聚至一个主地址中。

相较于「逐笔复制地址、手动签名转账」的传统模式，该功能的核心机制在于「底层批量指令聚合」。系统会将海量的独立转账指令通过智能合约整合为一个不可分割的数据包提交至链上。这种机制不仅将原本需要耗费数小时的机械性工作缩短至一键秒级完成，更通过合并同类项大幅平摊了整体的网络矿工费。

立即在 EVM 网络上，用 CiaoTool​ 批量转账功能进行多对一转账操作：

<table data-view="cards"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/BSC.png" alt="" data-size="line">BSC (BNB Chain)</td><td><a href="https://bsc.ciaotool.io/zh-Hans/transfer/many-to-one">https://bsc.ciaotool.io/zh-Hans/transfer/many-to-one</a></td></tr><tr><td><img src="../../../.gitbook/assets/BSC.png" alt="" data-size="line">opBNB</td><td><a href="https://opbnb.ciaotool.io/zh-Hans/transfer/many-to-one">https://opbnb.ciaotool.io/zh-Hans/transfer/many-to-one</a></td></tr><tr><td><img src="../../../.gitbook/assets/Base3.png" alt="" data-size="line">Base</td><td><a href="https://base.ciaotool.io/zh-Hans/transfer/many-to-one">https://base.ciaotool.io/zh-Hans/transfer/many-to-one</a></td></tr><tr><td><img src="../../../.gitbook/assets/3 (1).png" alt="" data-size="line">X Layer</td><td><a href="https://xlayer.ciaotool.io/zh-Hans/transfer/many-to-one">https://xlayer.ciaotool.io/zh-Hans/transfer/many-to-one</a></td></tr><tr><td><img src="../../../.gitbook/assets/IoTex.png" alt="" data-size="line">IoTeX</td><td><a href="https://iotex.ciaotool.io/zh-Hans/transfer/many-to-one">https://iotex.ciaotool.io/zh-Hans/transfer/many-to-one</a></td></tr><tr><td><img src="../../../.gitbook/assets/BOT-2.png" alt="" data-size="line"> BOT</td><td><a href="https://iotex.ciaotool.io/zh-Hans/transfer/many-to-one">https://iotex.ciaotool.io/zh-Hans/transfer/many-to-one</a></td></tr><tr><td><img src="../../../.gitbook/assets/Group 1261152954.png" alt="" data-size="line"> Robinhood</td><td><a href="https://robinhood.ciaotool.io/zh-Hans/transfer/many-to-one">https://robinhood.ciaotool.io/zh-Hans/transfer/many-to-one</a></td></tr></tbody></table>

***

## 为什么选择 CiaoTool EVM 代币归集（多对一转账）？ <a href="#advantage" id="advantage"></a>

CiaoTool 为 EVM 网络上的海量资产调拨提供了一种兼顾绝对安全与极简操作的专业解决方案。对于需要高频、大批量分发代币或基础燃料的用户而言，该工具构建了高效且稳健的执行防线： ​ ​

**百倍提升效率：**\
彻底免去人工频繁切换账号、复制粘贴地址与重复授权签名的繁琐流程，支持一键并发执行成百上千笔转账，实现链上资产的极速归集。 ​

**灵活的矩阵配置：**\
支持通过 Excel 电子表格文件一键批量导入目标地址列表与对应的分发额度。支持自定义等额、定额或随机金额分配，完美适配复杂多变的空投策略与持币分布需求。 ​

**本地安全环境：**\
采用纯前端本地执行机制，私钥仅在本地环境中用于交易签名，在极速提升交易效率的同时，全方位保障多钱包资产的绝对安全。

***

## **视频教程** <a href="#solana-one-to-multi-guide" id="solana-one-to-multi-guide"></a>

{% embed url="https://www.youtube.com/watch?t=1s&v=GTF1O4n6Kmo" %}

***

## **图文指南 | EVM 批量转账 - 多对一转账**  <a href="#solana-one-to-multi-guide" id="solana-one-to-multi-guide"></a>

{% stepper %}
{% step %}
### **切换公链并绑定钱包**

点击右上角按钮，绑定支持 EVM 网络的钱包

<figure><img src="../../../.gitbook/assets/image (475).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择接收钱包

<figure><img src="../../../.gitbook/assets/image (498).png" alt=""><figcaption></figcaption></figure>

输入接收钱包地址，或直接点击右侧按钮，选择当前绑定钱包。
{% endstep %}

{% step %}
### 选择转账代币

选择代币或直接输入代币地址。

<figure><img src="../../../.gitbook/assets/image (479).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入转账钱包私钥

{% hint style="danger" %}
**「多对一转账」**&#x529F;能支持使用私钥导入以进行转账操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入发送钱包私钥的类型，选择以查看详细教程。

{% tabs %}
{% tab title="手动输入" %}
直接在输入框中，输入 / 粘贴发送钱包私钥。每行仅输入一个地址

<figure><img src="../../../.gitbook/assets/image (508).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 点&#x51FB;**「上传文件」**&#x6309;钮，弹出文件上传窗口导入发送钱包私钥。

<figure><img src="../../../.gitbook/assets/image (481).png" alt=""><figcaption></figcaption></figure>

2. 使用 CiaoTool 模板文件导入，并保存确定导入并显示在输入框内。\
   点击下载并查看模板：

{% file src="../../../.gitbook/assets/EVM_privateKey_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (500).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 再次确认接收地址

为确保资金归集地址的准确性，请再次确认接收地址信息。完成点击下一步继续操作。

<figure><img src="../../../.gitbook/assets/image (501).png" alt=""><figcaption></figcaption></figure>
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
   所有钱包将余额内指定的代币全部发送到归集地址。
3. **固定数量**\
   所有钱包根据同一数量将指定代币全部发送到归集地址。
4. **固定留存**\
   所有钱包留存指定数量代币，其余全部数量发送到归集地址。
{% endstep %}

{% step %}
### 核对

核对发送信息，并查看状态栏。

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

<summary><strong>什么是多对一批量转账？</strong></summary>

多对一批量归集指将多个钱包地址中持有的代币统一转入一个主地址，**便于集中管理资产、统一调配资金**。

</details>

<details>

<summary><strong>如何导入接收地址？</strong></summary>

你可以手动输入地址，也可以上传 Excel 文件导入目标地址列表（支持地址+金额格式），系统会自动识别并展示预览。

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

<summary><strong>一次可以多少个地址进行归集？</strong></summary>

得益于私钥导入的模式，多对一转账功能免除了逐一钱包签署的繁复工作，发送地址没有任何数量限制。

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
