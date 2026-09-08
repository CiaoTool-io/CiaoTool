---
description: 专为 PumpFun 和 PumpSwap 平台提供的自动化做市与交易执行工具。有效提升代币交易活跃度，模拟真实链上交易行为，全面优化盘口数据表现的自然度。
---

# Pump - 市值管理教程

{% hint style="info" %}
**CiaoTool Pump 市值管理**现已全面支持官方 **SOL** 和 **USDC** 全部的价值代币，输入代币地址将自动切换适配和价值代币。
{% endhint %}

## CiaoTool Pump 市值管理是什么？

<figure><picture><source srcset="../../../.gitbook/assets/屏幕截图 2026-09-08 164910.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (895).png" alt="CiaoTool Solana Chain Pump 市值管理页面"></picture><figcaption></figcaption></figure>

**CiaoTool Pump 市值管理**是一款专为 Solana 生态打造的高阶自动化做市与流动性优化工具。它允许项目方和专业团队通过自定义交易参数，在 **Pump.fun** 和 **PumpSwap** 上全自动执行进阶的做市策略，从而安全、稳健地管理代币的盘口深度与市场活跃度。

相较于繁琐且难以精确控制的手动交易，该功能的核心优势在于其全自动化的策略执行引擎。系统能够根据设定的频率与规模，智能调度多个钱包地址进行持续的自然双向买卖交互。这不仅能有效优化代币的持币者分布与独立交易地址结构，更能使链上交易行为更接近真实的自然市场参与，全面提升整体数据表现的自然度。

该功能主要支持以下核心做市策略：

* 智能价格提振：通过合理的盘口交互参数，稳步优化代币的价格呈现。
* 平稳有序回调：平稳管理价格回落轨迹，避免市场出现剧烈波动。
* 持续活跃度提升：通过多地址与随机间隔机制执行买卖操作，稳步提升交易量，全面优化盘口数据表现的自然度。

立即在 PumpFun 或 PumpSwap上，用 CiaoTool 进行市值管理操作：

{% embed url="https://ciaotool.io/zh-Hans/pump/market-making" %}

***

## 为什么选择 CiaoTool Pump 市值管理？

**CiaoTool** 为 **Pump.fun** 和 **PumpSwap** 上的资产管理与长效增长提供了一种兼顾智慧化与安全性的专业做市方案。无论您是需要优化初期的流动性呈现、稳步提升日常的链上活跃度，还是执行复杂的多地址交易策略，其市值管理功能都能透过全自动化的参数配置，保障策略的精准与高效执行。\
​\
专为 **Pump.fun** 和 **PumpSwap** 交易环境打造，它将复杂的做市逻辑转化为一键启动的智慧化流程。结合纯前端本地私钥签名的安全机制，它在成倍节省团队营运时间、免除繁琐人工操作的同时，为 Web3 项目方构建了一套安全、合规且极具成本效益的流动性管理防线。

***

## **视频教程**

{% hint style="info" %}
**CiaoTool** Solana 链所有平台的市值管理功能页面**完全相同**，您可以观看下&#x65B9;**「Solana 市值管理」视频教程**，了解更多关于市值管理功能的详细步骤。
{% endhint %}

{% embed url="https://youtu.be/3P0st98XZwo" %}

## **图文指南**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角【连接钱包】按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (748).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择交易代币

可以选择输入代币地址，也可以选择当前钱包拥有的代币进行交易。系统将自动识别锚定价值代币并匹配所在池位置。

<figure><img src="../../../.gitbook/assets/image (896).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入钱包私钥

{% hint style="danger" %}
请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

{% hint style="info" %}
<mark style="color:$primary;">**操作钱包设置**</mark>

导入钱包没有数量限制。交易手续费由每个钱包独立支付。
{% endhint %}

导入钱包数量没有限制，支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入来源地址的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「批量输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (846).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x6BCF;行仅输入一个钱包私钥，可在私钥后追加数量。

```
privateKey, 300
```

<figure><img src="../../../.gitbook/assets/image (737).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (850).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 下载 CiaoTool 模板文件，并将信息导入到文件内。

<figure><img src="../../../.gitbook/assets/image (847).png" alt=""><figcaption></figcaption></figure>

2. 点击![](<../../../.gitbook/assets/image (848).png>)**「导入文件」**&#x6309;钮，弹出文件上传窗口。
3. 点&#x51FB;**「确定导入」**，将所有地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (849).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 选择交易模式

根据不同的做市策略需求，自行选择不同的机器人类型，并切换至对应策略机器人页面。

<figure><img src="../../../.gitbook/assets/image (851).png" alt=""><figcaption></figcaption></figure>

* **上升策略：**&#x4EA4;易钱包持续买入，逐步完成建仓、增加买盘活跃度，帮助形成上涨趋势。
* **下降策略：**&#x4EA4;易钱包持续卖出，平缓减持或回收资金，帮助形成下跌趋势。
* **交易量：**&#x5728;买入和卖出之间随机切换，持续产生双向成交，保持盘口活跃和交易数据更新。
{% endstep %}

{% step %}
### 交易设置

{% hint style="danger" %}
关闭 / 刷新页面，机器人策略亦会**立即停止**。请保持策略执行期间，将网页持续处于后台并运行状态。为保证策略执行之必要，**该功能不推荐于**「**移动电子设备**」**使用。**
{% endhint %}

点击下方做市策略，以显示完整机器人设置教程。

{% tabs %}
{% tab title="上升策略" %}
#### 单笔交易量

每笔交易的买入量，&#x4EE5;**「价值代币」**&#x7684;设置为锚定。

若左右区间相同，则为固定金额；若区间金额不同，每笔交易为该区间的随机金额。

#### **条件参数**

提供 **目标价格、累计最大交易额、运行时长** 三个条件参数。若不填将持续进行交易，若填写任一参数，则当满足条件时，会自动停止任务。

* **目标价格：**&#x6BD4;对价格达&#x5230;**「做市代币」**&#x8BBE;定值时，立即停止执行策略。
* **累计最大交易额：**&#x4EE5;**「价值代币」**&#x7684;设置为锚定，累计达到设定值时，立即停止执行策略。
* **运行时长：**&#x4EE5;分钟为单位，达到设定值时，立即停止执行策略。

<figure><img src="../../../.gitbook/assets/image (852).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="下行策略" %}
#### 单笔交易量

每笔交易的卖出量，&#x4EE5;**「做市代币」**&#x7684;设置为锚定。

若左右区间相同，则为固定金额；若区间金额不同，每笔交易为该区间的随机金额。

#### **条件参数**

提供 **目标价格、累计最大交易额、运行时长** 三个条件参数。若不填将持续进行交易，若填写任一参数，则当满足条件时，会自动停止任务。

* **目标价格：**&#x6BD4;对价格达&#x5230;**「目标代币」**&#x8BBE;定值时，立即停止执行策略。
* **累计最大交易额：**&#x4EE5;**「做市代币」**&#x7684;设置为锚定，累计达到设定值时，立即停止执行策略。
* **运行时长：**&#x4EE5;分钟为单位，达到设定值时，立即停止执行策略。

<figure><img src="../../../.gitbook/assets/image (853).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="交易策略" %}
#### 单笔交易量

每笔交易的卖出量，&#x4EE5;**「价值代币」**&#x7684;设置为锚定。

若左右区间相同，则为固定金额；若区间金额不同，每笔交易为该区间的随机金额。

#### **条件参数**

提供 **累计最大交易额、运行时长** 两个条件参数。若不填将持续进行交易，若填写任一参数，则当满足条件时，会自动停止任务。

* **累计最大交易额：**&#x4EE5;**「价值代币」**&#x7684;设置为锚定，累计达到设定值时，立即停止执行策略。
* **运行时长：**&#x4EE5;分钟为单位，达到设定值时，立即停止执行策略。

<figure><img src="../../../.gitbook/assets/image (854).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 通用参数设置

{% tabs %}
{% tab title="交易间隔" %}
可自由设置各地址交易执行间隔时间。

<figure><img src="../../../.gitbook/assets/image (855).png" alt=""><figcaption></figcaption></figure>

* **固定时间**\
  所有交易按固定时间提交广播。
* **随机时间**\
  将会在指定的时间范围内随机提交，模拟真实交易，但需要保持页面以持续执行。
{% endtab %}

{% tab title="滑点" %}
在执行交易时，实际成交价格与预期价格之间的存在差距。如果滑点范围设置过小，可能会错过有利的交易机会；设置过大，则可能会承担较大的价格波动风险。

<figure><img src="../../../.gitbook/assets/image (856).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="发送设置" %}
* **RPC 发送**\
  通过 RPC 节点统一广播转账交易，无需支付 Jito 小费。
* **Jito Bundle**\
  通过 Jito 小费提升上链优先级。

<figure><img src="../../../.gitbook/assets/image (857).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 启动交易

交易费用将由各钱包独立承担。

确认信息无误后，点击下方「**确认并发送**」按钮，即可开启做市程序。

<figure><img src="../../../.gitbook/assets/image (858).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 核实信息

{% hint style="danger" %}
关闭 / 刷新页面，机器人策略亦会**立即停止**。请保持策略执行期间，将网页持续处于后台并运行状态。为保证策略执行之必要，**该功能不推荐于**「**移动电子设备**」**使用。**
{% endhint %}

程序自动运行，查看确认页面并核对：

* [x] 当前币对价格
* [x] 成功交易数
* [x] 累计交易量等信息

<figure><img src="../../../.gitbook/assets/image (859).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## **常见失败案例**

* 过度拉升，导致抛压集中引发暴跌
* 流动性不足，价格波动剧烈
* 筹码过于集中，被单点砸盘影响
* 节奏失控，频繁操作导致市场信任下降
* 忽视外部行情，逆势操作失败

***

## **常见问题**

<details>

<summary><strong>什么是 Pump 市值管理？</strong></summary>

该功能用于在 **Pump.fun 及 PumpSwap 平台**中执行自动化交易策略与做市策略，通过多地址买卖操作，提升交易活跃度，使项目在市场中保持持续的交易表现和关注度。通过多地址与随机间隔机制，使交易行为更接近真实市场参与，提升整体数据表现的自然度。

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
