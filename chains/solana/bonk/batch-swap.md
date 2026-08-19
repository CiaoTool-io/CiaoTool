---
description: >-
  专为 BONKfun
  平台提供的多地址批量兑换与交易执行工具。支持快速将多个地址内的代币同步兑换为指定代币，大幅提升交易效率与时效性，特别适用于需要快速执行大量交易的场景。
---

# Bonk - 批量交易教程

{% hint style="info" %}
**CiaoTool Bonk 批量交易**现已全面支持官方 **SOL** 和 **USD1** 全部的价值代币，请先切换到指定代币页面进行批量交易操作，满足不同场景下的快捷兑换服务。
{% endhint %}

## CiaoTool Bonk 批量交易什么？&#x20;

**CiaoTool Bonk 批量交易**是一款专为 **BONKfun 平台**打造的多地址自动化交易执行工具。它允许用户通过批量导入多个钱包地址并设置交易参数，全自动且同步地执行代币买卖操作。

该功能的核心机制在于快速将多地址的代币批量兑换成指定的代币。相较于传统单地址的人工逐一操作，系统通过多地址并发执行，大幅提高了交易指令的响应速度与流转效率。它彻底改变了低效的手动执行模式，全面提升了多钱包交互的时效性，特别适用于需要极速完成大规模代币兑换与资产调拨的场景。

立即在 Bonk 上，用 CiaoTool 市值管理进行多地址批量兑换操作：

{% embed url="https://ciaotool.io/zh-CN/bonk/batch-swap" %}

***

## 为什么选择 CiaoTool Bonk 批量交易？

CiaoTool 为 BONKfun 平台上的多地址交易管理提供了一种兼顾极速与安全的专业解决方案。对于需要快速执行大量交易的用户而言，该工具能显著提升整体的执行效率：

* **极速并发执行：**&#x652F;持一键启动多钱包同步兑换指令，彻底免去人工频繁切换地址与重复签名的繁琐流程，大幅提升大规模交易的时效性。
* **高效资产兑换：**&#x80FD;够快速将多个独立地址中的代币同步兑换为指定的统一代币，满足各类高频、大体量的资产流转需求。
* **灵活参数配置：**&#x652F;持为不同钱包地址自定义交易规模，精准匹配各类复杂的多地址自动化交易策略。
* **本地安全环境：**&#x91C7;用纯前端本地执行机制，私钥仅在本地环境中用于交易签名，在极速提升交易效率的同时，全方位保障多钱包资产的绝对安全。

***

## **图文指南 |** Bonk 批量交易

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (308).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择兑换代币

可以选择输入代币地址，也可以选择当前钱包拥有的代币进行买入操作。点击中间箭头可快速切换兑换目标。

<figure><img src="../../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入交易钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

当&#x524D;**「批量交易」**&#x529F;能仅支持 私钥导入以进行兑换操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

{% hint style="info" %}
<mark style="color:$primary;">**交易钱包设置**</mark>

**Bonk 批量交易**导入钱包没有数量限制。交易手续费由每个钱包独立支付。
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入钱包私钥的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「手动输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (358).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (310).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包私钥，**&#x4E00;行仅输入一个私钥，按回车键换行

<figure><img src="../../../.gitbook/assets/image (263).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (362).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 点&#x51FB;**「手动输入」**&#x6309;钮，弹出文件上传窗口。

<figure><img src="../../../.gitbook/assets/image (359).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (251).png" alt=""><figcaption></figcaption></figure>

2. 导入钱包私钥信息文件，显示私钥信息。\
   请通过 CiaoTool 模板文件导入，以确保私钥准确导入。

<figure><img src="../../../.gitbook/assets/image (317).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (361).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入买入金额

支&#x6301;**「逐一输入」「全部金额」「固定金额」「随机金额」「随机百分比」**&#x4E94;种转账金额类型。

1. **逐一输入**\
   在输入框中，逐一输入买入金额数量

* 若填写数量，则按照填写的数量进行交易。
* 若未填写数量，则按照交易数量中  设置的数量进行交易。

2. **全部金额**\
   所有钱包将把代币全部兑换为指定代币。
3. **固定金额**\
   所有钱包根据同一数量将代币全部兑换为指定代币。
4. **随机金额**\
   所有钱包根据设定范围，将随机数量的代币全部兑换为指定代币。
5. **随机百分比**\
   所有钱包根据设定范围，将各钱包余额百分比的代币全部兑换为指定代币。
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下&#x65B9;**「开始」**&#x6309;钮，并等交易程序完成。
{% endstep %}
{% endstepper %}

## **常见失败案例**

* 滑点设置过低，币对价格超出额定范围
* 流动性不足，价格波动剧烈
* Jito 小费设置过低，被 MEV 机器人抢跑

***

## **常见问题 FAQ**

<details>

<summary><strong>什么是 Bonk 批量交易？</strong></summary>

批量交易是指通过多地址自动执行买入或卖出操作，在设定的滑点范围内完成代币交换。该功能主要用于大规模资金的快速换仓或资产转换，在保证成交效率的同时尽量降低因滑点带来的损耗。

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
