---
description: 一对多转账是一种高效便捷的代币分发工具，支持将同一钱包中的代币批量发送至无限个接收地址，适用于空投、奖励发放和批量结算等场景。
metaLinks:
  alternates:
    - https://app.gitbook.com/s/b56FKZGe1viFi67H1pPQ/transfer/one-to-many
---

# EVM - 批量转账 | 一对多转账教程

{% hint style="info" %}
当前&#x662F;**「EVM - 一对多转账」**&#x6559;程页面以查看 **BSC、opBNB、Base、X Layer、IoTeX、BOT、Robinhood** 等 EVM 网络教程。

本教程演示基于 BSC（BNB Chain）功能页面，本功能 EVM 网络 CiaoTool 全链通用，请切换至对应公链进行一对多转账操作。

点击[**「Solana - 一对多转账」**](../../../chains/solana/multisender/one-to-many.md)查看 Solana 网络一对多转账教程。
{% endhint %}

## CiaoTool EVM 一对多转账是什么？ <a href="#definition" id="definition"></a>

<figure><img src="../../../.gitbook/assets/image (476).png" alt="CiaoTool BSC 批量转账 一对多转账页面"><figcaption></figcaption></figure>

**CiaoTool EVM 一对多转账**是一款专为是一款专为 BSC (BNB Smart Chain) 及 EVM 兼容生态打造的高效链上资产分发工具。它允许用户突破传统单笔转账的限制，全自动调度将单个主钱包中的原生代币（BNB / ETH...）或各类 BEP-20 / ERC-20...标准代币，在同一次操作中批量发送至数百个不同的接收地址。

相较于「逐笔复制地址、手动签名转账」的传统模式，该功能的核心机制在于「底层批量指令聚合」。系统会将海量的独立转账指令通过智能合约整合为一个不可分割的数据包提交至链上。这种机制不仅将原本需要耗费数小时的机械性工作缩短至一键秒级完成，更通过合并同类项大幅平摊了整体的网络矿工费，是项目方进行空投分发、团队结算或做市前置分仓的核心基建。

此工具尤其适用于：

* 空投和代币分发
* DAO收益和奖励
* 向用户批量付款
* 营销活动和Web3增长策略

立即在 EVM 网络上，用 CiaoTool​ 批量转账功能进行一对多转账操作：

<table data-view="cards"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/BSC.png" alt="" data-size="line">BSC (BNB Chain)</td><td><a href="https://bsc.ciaotool.io/zh-Hans/transfer/one-to-many">https://bsc.ciaotool.io/zh-Hans/transfer/one-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/BSC.png" alt="" data-size="line">opBNB</td><td><a href="https://opbnb.ciaotool.io/zh-Hans/transfer/one-to-many">https://opbnb.ciaotool.io/zh-Hans/transfer/one-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/Base3.png" alt="" data-size="line">Base</td><td><a href="https://base.ciaotool.io/zh-Hans/transfer/one-to-many">https://base.ciaotool.io/zh-Hans/transfer/one-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/3 (1).png" alt="" data-size="line">X Layer</td><td><a href="https://xlayer.ciaotool.io/zh-Hans/transfer/one-to-many">https://xlayer.ciaotool.io/zh-Hans/transfer/one-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/IoTex.png" alt="" data-size="line">IoTeX</td><td><a href="https://iotex.ciaotool.io/zh-Hans/transfer/one-to-many">https://iotex.ciaotool.io/zh-Hans/transfer/one-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/BOT-2.png" alt="" data-size="line"> BOT</td><td><a href="https://bot.ciaotool.io/zh-Hans/transfer/one-to-many">https://bot.ciaotool.io/zh-Hans/transfer/one-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/Group 1261152954.png" alt="" data-size="line"> Robinhood</td><td><a href="https://robinhood.ciaotool.io/zh-Hans/transfer/one-to-many">https://robinhood.ciaotool.io/zh-Hans/transfer/one-to-many</a></td></tr></tbody></table>

***

## 为什么选择 CiaoTool EVM 代币空投（一对多转账）？ <a href="#advantage" id="advantage"></a>

CiaoTool 为 EVM 网络上的海量资产调拨提供了一种兼顾绝对安全与极简操作的专业解决方案。对于需要高频、大批量分发代币或基础燃料的用户而言，该工具构建了高效且稳健的执行防线： ​ ​

**百倍提升效率：**\
彻底免去人工频繁切换账号、复制粘贴地址与重复授权签名的繁琐流程，支持一键并发执行成百上千笔转账，实现链上资产的极速流转。 ​

**极致削减成本：**\
通过底层智能合约的多重调用与批量打包技术，将多笔转账聚合为单次链上交互，最大程度摊薄网络费用，显著降低大规模分发的资金损耗。 ​

**灵活的矩阵配置：**\
支持通过 Excel 电子表格文件一键批量导入目标地址列表与对应的分发额度。支持自定义等额、定额或随机金额分配，完美适配复杂多变的空投策略与持币分布需求。 ​

**本地安全环境：**\
采用纯前端本地执行机制，私钥仅在本地环境中用于交易签名，在极速提升交易效率的同时，全方位保障多钱包资产的绝对安全。

***

## 视频教程 | EVM 批量转账 - 一对多转账 <a href="#video-guide" id="video-guide"></a>

{% embed url="https://www.youtube.com/watch?v=fEIzmEVup6E" %}

***

## **图文指南 | EVM 批量转账 - 一对多转账**  <a href="#solana-one-to-multi-guide" id="solana-one-to-multi-guide"></a>

{% stepper %}
{% step %}
### **切换公链并绑定钱包**

点击右上角按钮，绑定支持 EVM 网络的钱包

<figure><img src="../../../.gitbook/assets/image (475).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择转账钱包

{% hint style="danger" %}
**「一对多转账」**&#x529F;能支持使用当前钱包和私钥导入以进行转账操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (477).png" alt=""><figcaption></figcaption></figure>

**自用钱包：**&#x5373;使用当前钱包直接进行转账操作，无需使用私钥，资金更安全。由于签名限制，单次转账最多只能支持最多 200 个钱包。

**其他钱包：**&#x5373;使用私钥的形式进行转账操作，快捷方便调用备用钱包。由于不需要签名限制，单次转账地址数量没有限制，支持设置转账间隔。
{% endstep %}

{% step %}
### 选择转账代币

可以选择 BNB，也可以选择当前钱包拥有的代币进行转账。

<figure><img src="../../../.gitbook/assets/image (479).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入接收地址

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入接收地址的类型，选择以查看详细教程。

{% tabs %}
{% tab title="手动输入" %}
直接在输入框中，输入 / 粘贴接收钱包地址。每行仅输入一个地址

<figure><img src="../../../.gitbook/assets/image (480).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 点&#x51FB;**「上传文件」**&#x6309;钮，弹出文件上传窗口导入接收钱包地址。

<figure><img src="../../../.gitbook/assets/image (481).png" alt=""><figcaption></figcaption></figure>

2. 使用 CiaoTool 模板文件导入，并保存确定导入并显示在输入框内。\
   点击下载并查看模板：

{% file src="../../../.gitbook/assets/EVM_address_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (482).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入转账金额

<figure><img src="../../../.gitbook/assets/image (483).png" alt=""><figcaption></figcaption></figure>

支&#x6301;**「相同数量」和「自定义数量」**&#x4E24;种转账金额类型，选择以查看详细教程。

{% tabs %}
{% tab title="相同数量" %}
在地址输入栏下方，输入统一转账的代币数量。

<figure><img src="../../../.gitbook/assets/image (485).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="自定义数量" %}
1. **通过表格导入：**\
   在表格里额外起一列，输入每个地址接收的代币数量。

<figure><img src="../../../.gitbook/assets/image (488).png" alt=""><figcaption></figcaption></figure>

2. **通过手写输入：**\
   在每个钱包地址后面输入代币数量，用英文逗号隔开地址和转账数量。

```
例如：0x0000000000000000000000000000000000000000,300
```

<figure><img src="../../../.gitbook/assets/image (487).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 慢速转账设置

{% hint style="warning" %}
&#x4EC5;**「其他钱包」**&#x9002;配，可设置各地址转账执行间隔时间
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (489).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下&#x65B9;**「发送」**&#x6309;钮，并等待转账程序完成。
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>什么是一对多批量转账？</strong></summary>

一对多批量转账是指从一个钱包地址，向多个目标地址**同时发送代币**的操作，常用于空投、奖励发放、资产分发等场景。

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

<summary><strong>一次可以发送到多少个地址？</strong></summary>

取决于选择钱包的形式，若使用私钥导入的模式，一对多转账功能免除了逐一钱包签署的繁复工作，接收地址没有任何数量限制。

</details>

<details>

<summary><strong>可以同时转多种代币吗？</strong></summary>

当前版本支持选择单一代币进行批量转账；如需多种资产分发，可多次执行操作或使用[「批量一转多」功能](one-to-many-multi.md)。

</details>

***

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
