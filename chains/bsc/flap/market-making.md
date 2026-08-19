---
description: 专为 BSC 生态 Flap.sh 平台提供的自动化做市与交易执行工具。有效提升代币交易活跃度，模拟真实链上交易行为，全面优化盘口数据表现的自然度。
---

# Flap - 市值管理教程

{% hint style="info" %}
**CiaoTool Flap 市值管理**现已全面支持官方 **BNB、USD1、UUSD** 和 **USDT** 全部的价值代币，满足不同场景下的快捷做市服务。
{% endhint %}

## Flap 市值管理是什么？

<figure><img src="../../../.gitbook/assets/image (566).png" alt=""><figcaption></figcaption></figure>

**CiaoTool Flap 市值管理**是一款专为 BSC 生态打造的高阶自动化做市与流动性优化工具。它允许项目方和专业团队通过自定义交易参数，在 **Flap.sh** 上全自动执行进阶的做市策略，从而安全、稳健地管理代币的盘口深度与市场活跃度。

相较于繁琐且难以精确控制的手动交易，该功能的核心优势在于其全自动化的策略执行引擎。系统能够根据设定的频率与规模，智能调度多个钱包地址进行持续的自然双向买卖交互。这不仅能有效优化代币的持币者分布与独立交易地址结构，更能使链上交易行为更接近真实的自然市场参与，全面提升整体数据表现的自然度。

该功能主要支持以下核心做市策略：

* 智能价格提振：通过合理的盘口交互参数，稳步优化代币的价格呈现。
* 平稳有序回调：平稳管理价格回落轨迹，避免市场出现剧烈波动。
* 持续活跃度提升：通过多地址与随机间隔机制执行买卖操作，稳步提升交易量，全面优化盘口数据表现的自然度。

立即在 Flap 上，用 CiaoTool 进行市值管理操作：

{% embed url="https://bsc.ciaotool.io/zh-Hans/flap/market-making-manage" %}

***

## 为什么选择 CiaoTool Flap 市值管理？

**CiaoTool** 为 Flap 上的资产管理与长效增长提供了一种兼顾智慧化与安全性的专业做市方案。无论您是需要优化初期的流动性呈现、稳步提升日常的链上活跃度，还是执行复杂的多地址交易策略，其市值管理功能都能透过全自动化的参数配置，保障策略的精准与高效执行。\
​\
专为 Flap.sh 交易环境打造，它将复杂的做市逻辑转化为一键启动的智慧化流程。结合纯前端本地私钥签名的安全机制，它在成倍节省团队营运时间、免除繁琐人工操作的同时，为 Web3 项目方构建了一套安全、合规且极具成本效益的流动性管理防线。

***

## 视频教程 | Flap 市值管理

{% hint style="info" %}
如果你更偏好视频形式的学习，该功能页面与 Flap 页面结构类似，参考并观看本教程
{% endhint %}

{% embed url="https://www.youtube.com/watch?v=YKa1RO7n-ZI" %}

***

## **图文指南 |** Flap 市值管理

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 BSC 链的钱包

<figure><img src="../../../.gitbook/assets/image (467).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入支付钱包私钥

将用于支付市值操作手续费的钱包私钥导入。

<figure><img src="../../../.gitbook/assets/image (551).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入做市代币地址

可以选择输入代币地址，也可以选择当前钱包拥有的代币进行买入操作。\
点击中间箭头可快速切换兑换目标。

<figure><img src="../../../.gitbook/assets/image (469).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入交易钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

**「批量交易」**&#x529F;能多地址导入仅支持 私钥导入以进行兑换操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入交易地址私钥的类型。最多支持 20 个地址。

1. 点&#x51FB;**「导入私钥」**&#x6309;钮，弹出输入框。

<figure><img src="../../../.gitbook/assets/image (562).png" alt=""><figcaption></figcaption></figure>

2. 手动输入或导入私钥文件，确认框中显示私钥后点击确认。

<figure><img src="../../../.gitbook/assets/image (474).png" alt=""><figcaption></figcaption></figure>

使用 CiaoTool 模板文件导入，并保存确定导入并显示在输入框内。\
点击下载并查看模板：

{% file src="../../../.gitbook/assets/EVM_privateKey_demo.xlsx" %}
{% endstep %}

{% step %}
### 输入买入金额

{% hint style="info" %}
每个交易的钱包中，需要保留一些 BNB（每笔至少0.0008 BNB） 用于支付交易 Gas。
{% endhint %}

支&#x6301;**「逐一输入」「固定数量」「固定留存」「全部数量」**&#x56DB;种交易金额类型。

<figure><img src="../../../.gitbook/assets/image (472).png" alt=""><figcaption></figcaption></figure>

1. **逐一输入**\
   在输入框中，逐一输入买入金额数量
   * 若填写数量，则按照填写的数量进行交易。
   * 若未填写数量，则按照交易数量中     设置的数量进行交易。
2. **固定数量**\
   所有钱包根据同一数量将代币全部兑换为指定代币。
3. **固定留存**\
   所有钱包留存指定数量代币，其余全部兑换为指定代币。
4. **全部数量**\
   所有钱包将把价值代币全部兑换为指定代币。
{% endstep %}

{% step %}
### 交易参数设置

{% hint style="danger" %}
关闭 / 刷新页面，机器人策略亦会**立即停止**。请保持策略执行期间，将网页持续处于后台并运行状态。为保证策略执行之必要，**该功能不推荐于**「**移动电子设备**」**使用。**
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (565).png" alt=""><figcaption></figcaption></figure>

**滑点：**&#x5728;执行交易时，实际成交价格与预期价格之间的存在差距。如果滑点范围设置过小，可能会错过有利的交易机会；设置过大，则可能会承担较大的价格波动风险。

**停止方式：**

* **运行次数：**&#x5F53;导入钱包执行循环到指定阈值时，市值管理机器人随即停止。
* 价格范围：当做市代币价格超出指定范围时，市值管理机器人随即停止。

**交易间隔：**&#x6307;各钱包买入 / 卖出的执行间隔，通过随机时间范围，模拟真实交易。
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下&#x65B9;**「开始交易」**&#x6309;钮，并等交易程序完成。
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>什么是 Flap 市值管理？</strong></summary>

该功能用于在 Flap.sh 中执行自动化交易策略与做市策略，通过多地址买卖操作，提升交易活跃度，使项目在市场中保持持续的交易表现和关注度。通过多地址与随机间隔机制，使交易行为更接近真实市场参与，提升整体数据表现的自然度。

</details>

<details>

<summary><strong>运行中随时能暂停吗？</strong></summary>

可以，CiaoTool 是纯前端开发者工具，刷新当前页面，进程随即停止并关闭。

</details>

<details>

<summary><strong>为什么市值管理建议使用多钱包？</strong></summary>

可以有效优化持仓分布，模拟用户真实交易。

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
