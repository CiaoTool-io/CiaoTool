---
description: >-
  专为 SushiSwap
  平台提供的多地址批量兑换与交易执行工具。支持快速将多个地址内的代币同步兑换为指定代币，大幅提升交易效率与时效性，特别适用于需要快速执行大量交易的场景。
---

# Base - V3 批量交易教程

{% hint style="info" %}
**CiaoTool SushiSwap 批量交易**现已全面支持 **V3 流动性池**类型。
{% endhint %}

## CiaoTool Base 批量交易什么？  <a href="#what-is-coinfactory-solana-multisender" id="what-is-coinfactory-solana-multisender"></a>

**CiaoTool Base 批量交易**是一款专为 Base 生态 **SushiSwap V3 流动性池**打造的多地址自动化交易执行工具。它允许用户通过批量导入多个钱包地址并设置交易参数，全自动且同步地执行代币买卖操作。

该功能的核心机制在于快速将多地址的代币批量兑换成指定的代币。相较于传统单地址的人工逐一操作，系统通过多地址并发执行，大幅提高了交易指令的响应速度与流转效率。它彻底改变了低效的手动执行模式，全面提升了多钱包交互的时效性，特别适用于需要极速完成大规模代币兑换与资产调拨的场景。

立即在 Base 上，用 CiaoTool 批量交易进行多地址批量兑换操作：

{% embed url="https://base.ciaotool.io/zh-Hans/swap/v3/batch-swap-v3" %}

***

## 为什么选择 CiaoTool Base 批量交易？ <a href="#why-use-coinfactory-multisender-for-solana" id="why-use-coinfactory-multisender-for-solana"></a>

CiaoTool 为 SushiSwap 平台上的多地址交易管理提供了一种兼顾极速与安全的专业解决方案。对于需要快速执行大量交易的用户而言，该工具能显著提升整体的执行效率：

* **极速并发执行：**&#x652F;持一键启动多钱包同步兑换指令，彻底免去人工频繁切换地址与重复签名的繁琐流程，大幅提升大规模交易的时效性。
* **高效资产兑换：**&#x80FD;够快速将多个独立地址中的代币同步兑换为指定的统一代币，满足各类高频、大体量的资产流转需求。
* **灵活参数配置：**&#x652F;持为不同钱包地址自定义交易规模，精准匹配各类复杂的多地址自动化交易策略。
* **本地安全环境：**&#x91C7;用纯前端本地执行机制，私钥仅在本地环境中用于交易签名，在极速提升交易效率的同时，全方位保障多钱包资产的绝对安全。

***

## **图文指南 |** Base 批量交易

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 Base 链的钱包

<figure><img src="../../../.gitbook/assets/image (386).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入币对地址

不同于 V2 流动性池，每个不同币对和税费的 V3 流动性池有专属的币对地址，请输入正确的币对地址以选择兑换币对。

<figure><img src="../../../.gitbook/assets/image (391).png" alt=""><figcaption></figcaption></figure>

**不知道如何查找 V3 币对地址？**

{% content-ref url="../../../start/find-v3-token-pair-address.md" %}
[find-v3-token-pair-address.md](../../../start/find-v3-token-pair-address.md)
{% endcontent-ref %}
{% endstep %}

{% step %}
### 输入支付钱包私钥

将用于支付市值操作手续费和网络gas费的钱包私钥导入。

<figure><img src="../../../.gitbook/assets/image (392).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入交易钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

当&#x524D;**「批量交易」**&#x529F;能仅支持 私钥导入以进行兑换操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入转账地址私钥的类型。

1. 点&#x51FB;**「导入私钥」**&#x6309;钮，弹出输入框。

<figure><img src="../../../.gitbook/assets/image (393).png" alt=""><figcaption></figcaption></figure>

2. 手动输入或导入私钥文件，确认框中显示私钥后点击确认。

<figure><img src="../../../.gitbook/assets/image (395).png" alt=""><figcaption></figcaption></figure>

使用 CiaoTool 模板文件导入，并保存确定导入并显示在输入框内。\
点击下载并查看模板：

{% file src="../../../.gitbook/assets/EVM_privateKey_demo.xlsx" %}
{% endstep %}

{% step %}
### 输入买入金额

支&#x6301;**「逐一输入」「固定数量」「固定留存」「全部数量」**&#x56DB;种转账金额类型。

1. **逐一输入**\
   在输入框中，逐一输入买入金额数量

* 若填写数量，则按照填写的数量进行交易。
* 若未填写数量，则按照交易数量中  设置的数量进行交易。

2. **固定数量**\
   所有钱包根据同一数量将代币全部兑换为指定代币。
3. **固定留存**\
   所有钱包留存指定数量代币，其余全部兑换为指定代币。
4. **全部数量**\
   所有钱包将把价值代币全部兑换为指定代币。
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下&#x65B9;**「开始交易」**&#x6309;钮，并等交易程序完成。
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>什么是 Base 批量交易？</strong></summary>

批量交易是指通过多地址自动执行买入或卖出操作。该功能主要用于大规模资金的快速换仓或资产转换。

</details>

<details>

<summary><strong>操作是否安全？</strong></summary>

平台采用纯前端签名机制，您的私钥绝不会被上传或储存在任何服务器上，所有交易均在本地浏览器完成签名，从技术层面确保平台无法访问您的私钥。

</details>

**💬 如遇到问题？加入社群实时咨询**：[https://t.me/ciaotool](https://t.me/ciaotool)

* **Email**：[support@ciaotool.io](mailto:support@ciaotool.io)
* **官网**：[https://ciaotool.io](https://ciaotool.io/)
* **X（Twitter）**：[https://x.com/CiaoTool](https://x.com/CiaoTool)
* **Medium**： [https://medium.com/@ciaotool](https://medium.com/@ciaotool)
* **Blog**：[https://www.ciaoailiquidity.com/zh/blog](https://www.ciaoailiquidity.com/zh/blog)
* **YouTube**：[https://www.youtube.com/@CiaoTool](https://www.youtube.com/@CiaoTool)
* **WhatsApp**：[https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J](https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J)

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
