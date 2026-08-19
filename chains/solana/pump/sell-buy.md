---
description: >-
  专为 PumpFun 打造的高效交易换仓工具，通过同区块聚合执行卖出与多钱包买入，模拟真实盘口交易形式让换仓行为更自然。在有效降低 MEV
  夹击风险与资金损耗的同时，安全优化链上资产轨迹。
---

# PumpFun - 卖出并多地址捆绑买入教程

{% hint style="info" %}
**CiaoTool PumpFun 多地址捆绑卖出**现已全面支持官方 **SOL** 和 **USDC** 全部的价值代币，请先切换到指定代币页面进行多地址捆绑买卖操作，满足不同场景下的快捷交易服务。
{% endhint %}

## CiaoTool PumpFun 卖出并多地址捆绑买入是什么？

**CiaoTool PumpFun 卖出并多地址捆绑买入**是一款专注于交易连贯性与链上流动性管理的高阶工具。它允许您通过底层智能聚合技术，在同一个区块内，自动让指定钱包完成 Pump.fun 上的代币卖出操作，并同步触发多个独立钱包的批量买入行为。

相较于传统的分步手动交易或直接批量转账，该功能的核心优势在于以真实的盘口交易形式让换仓行为更自然。系统将买卖双向交易聚合于同一区块执行，不仅最大程度减少了交易被 MEV 机器人“夹击”的风险与资金磨损，更免去了您在繁琐流程中频繁切换钱包地址的操作麻烦。这能在成倍节省运营时间的同时，帮助团队安全、稳健地优化代币的持币者分布，是执行进阶做市与流动性平移策略的关键利器。

此工具尤其适用于：

* 专业做市的流动性平移与资产安全重组
* 以真实盘口买卖取代直接转账，让筹码转移轨迹更符合市场自然逻辑
* 降低买卖双向交易时的滑点损耗与 MEV 夹击风险
* 免除频繁切换钱包的繁琐操作，大幅节省团队运营时间
* 安全、稳健地促进代币地址的健康分布与链上数据优化

立即在 PumpFun 上，用 CiaoTool 通过卖出并多地址捆绑买入进行交易换仓操作：

{% embed url="https://ciaotool.io/zh-CN/pump/bundled-sell" %}

***

## 为什么选择 CiaoTool PumpFun 卖出并捆绑买入？

**CiaoTool** 为 **PumpFun** 上的资产调拨与流动性重组提供了一种兼顾安全与低损耗的专业“交易换仓”方案。相较于容易被追踪的直接批量转账，该功能通过同区块智能聚合技术，将筹码转移巧妙转化为真实的盘口买卖，让多钱包的换仓行为更自然、更符合市场逻辑，有效优化链上数据的聚类呈现。\
​\
买卖双向交易的无缝衔接，不仅大幅降低了 PumpFun 中的滑点损耗与 MEV 机器人的夹击风险，更免去了您在繁琐流程中频繁切换钱包地址的操作麻烦。在成倍节省运营时间的同时，为 Web3 项目方与专业团队构建了一道坚实的流动性安全防线。

***

## **图文指南 | PumpFun** 卖出并捆绑买入

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (308).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择卖出代币

可以选择输入代币地址，也可以选择当前钱包拥有的代币进行卖出操作。

<figure><img src="../../../.gitbook/assets/image (352).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入卖出钱包私钥 并 设置卖出金额

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

当&#x524D;**「卖出并捆绑买入」**&#x529F;能仅支持 私钥导入以进行交易操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (324).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入买入钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

当&#x524D;**「卖出并捆绑买入」**&#x529F;能仅支持 私钥导入以进行交易操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

{% hint style="info" %}
<mark style="color:$primary;">**捆绑包设置**</mark>

**PumpFun 卖出并捆绑买入**导入钱包没有数量限制，每组交易最多支持 20 个地址捆绑买入。

多地址捆绑卖出的服务费均由每组第一个地址支付，Jito 小费由导入的最后一个地址支付，调整导入的第一个和最后一个地址中有足够余额。
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入钱包私钥的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「手动输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (326).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (310).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包私钥，**&#x4E00;行仅输入一个私钥，按回车键换行

<figure><img src="../../../.gitbook/assets/image (263).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (329).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 点&#x51FB;**「上传文件」**&#x6309;钮，弹出文件上传窗口。

<figure><img src="../../../.gitbook/assets/image (327).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (251).png" alt=""><figcaption></figcaption></figure>

2. 导入钱包私钥信息文件，显示私钥信息。\
   请通过 CiaoTool 模板文件导入，以确保私钥准确导入。

<figure><img src="../../../.gitbook/assets/image (317).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (328).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入买入金额

支&#x6301;**「逐一输入」盒「统一金额」**&#x4E24;种交易金额类型。

1. **逐一输入**\
   在输入框中，逐一输入转账金额数量

<figure><img src="../../../.gitbook/assets/image (252).png" alt=""><figcaption></figcaption></figure>

2. **统一金额**\
   点击转账数量上方&#x7684;**「统一输入」**&#x6309;钮，输入金额数量，所有地址将统一买入数量

<figure><img src="../../../.gitbook/assets/image (331).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下&#x65B9;**「卖出并捆绑买入」**&#x6309;钮，并等交易程序完成。
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>什么是 PumpFun 卖出并捆绑买入功能？</strong></summary>

这是 CiaoTool 专为 PumpFun 平台打造的高阶「交易换仓」工具。它允许用户在同一个区块内，无缝衔接指定钱包的代币卖出操作与多个子钱包的批量买入行为。透过同区块智能聚合技术，将资产的跨钱包平移巧妙转化为真实的盘口买卖交互。

</details>

<details>

<summary><strong>该功能与「冷换仓」有什么区别？</strong></summary>

两者的核心区别在于资产迁移的链上行为形式不同，分别适用于不同的营运场景：

**冷换仓**（纯转帐形式）：纯粹透过链上转帐将代币从源钱包打散分发到多个新地址，绝不涉及任何盘口交易。其优点是完全不影响市场价格，适合悄无声息地隐匿分仓。

**卖出并捆绑买入**（交易换仓形式）：筹码转移不通过直接转帐，而是通过盘口卖出 & 多钱包同步买入的真实交易来完成。它会在链上留下正常的市场买卖轨迹，让多钱包的换仓行为显得更加真实自然，完美切断了钱包之间的直接转帐关联。

</details>

<details>

<summary><strong>交易换仓会对代币的市场数据产生什么影响？</strong></summary>

由于整个换仓过程是通过在 PumpFun 盘口进行真实的买卖交互完成的，因此它在自然完成资产平移的同时，还会为代币贡献真实的交易笔数与盘口活跃度，并安全、稳健地优化代币的持币者分布与独立交易地址结构。

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
