---
description: >-
  专为 PumpSwap 打造的高效批量卖出工具，通过同区块聚合执行多地址卖出，有效降低 MEV
  夹击风险与资金损耗，优化团队资产出仓效率，是保障交易成本效益的专业利器。
---

# PumpSwap - 多地址捆绑卖出教程

{% hint style="info" %}
**CiaoTool PumpSwap 多地址捆绑卖出**现已全面支持官方 **SOL** 和 **USDC** 全部的价值代币，请先切换到指定代币页面进行多地址捆绑卖出操作，满足不同场景下的快捷卖出服务。
{% endhint %}

## CiaoTool PumpSwap 多地址捆绑卖出是什么？

**CiaoTool PumpSwap 多地址捆绑卖出**是一款专注于交易执行优化与链上流动性管理的高阶工具。它允许您通过底层智能聚合技术，在同一个区块内，自动让多个独立钱包同步完成 Pump.fun 上的代币批量卖出操作。&#x20;

相较于传统的分批手动交易，多地址捆绑卖出的核心优势在于有效降低 MEV 机器人的干扰与资金损耗。系统将多笔交易聚合于同一区块执行，最大程度减少交易“被夹”的风险，保障交易的成本效益。这不仅能显著提升批量出仓的执行效率，更能帮助团队安全、稳健地管理代币的链上流动性，是执行进阶做市与流动性调整策略的关键利器。 ​ 此工具尤其适用于：

* 专业做市的资产变现与流动性安全平仓
* 降低多钱包批量卖出时的滑点与 MEV 夹击风险
* 安全、稳健地管理及调整代币的链上分布状态
* 提升多地址链上资产配置与资金回笼的整体效率

立即在 PumpSwap 上，用 CiaoTool 进行多地址捆绑卖出操作：

{% embed url="https://ciaotool.io/zh-CN/pumpSwap/multi-address-sell" %}

***

## 为什么选择 CiaoTool PumpSwap 多地址捆绑卖出？

**CiaoTool** 为 **PumpSwap** 上的资产管理与流动性调整提供了一种兼顾效率与成本保护的专业方案。无论您是执行专业做市的资产变现、规避 MEV 夹击的批量卖出交易，还是稳健地管理代币的链上流动性，其多地址捆绑卖出功能都能通过同区块智能聚合技术，免去您在繁琐流程中频繁更换钱包地址的操作麻烦，成倍节省宝贵的运营时间，全方位保障交易的成本效益与执行安全。\
​\
专为 **PumpSwap** 交易环境打造，它能最大程度降低滑点损耗与链上机器人的干扰。结合自动化批处理引擎，它在免除人工换号操作的同时，极大提升了多钱包资产变现的效率，是 Web3 项目方和专业团队不可或缺的流动性管理利器。

***

## **图文指南 |** PumpSwap 多地址捆绑卖出

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (308).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择卖出代币

可以选择输入代币地址，也可以选择当前钱包拥有的代币进行卖出操作。

<figure><img src="../../../.gitbook/assets/image (384).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入卖出钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

当&#x524D;**「多地址捆绑卖出」**&#x529F;能仅支持 私钥导入以进行交易操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

{% hint style="info" %}
<mark style="color:$primary;">**捆绑包设置**</mark>

**PumpSwap 多地址捆绑卖出**导入钱包没有数量限制，每组交易最多支持 20 个地址捆绑卖出。

多地址捆绑卖出的服务费均由每组第一个地址支付，Jito 小费由导入的最后一个地址支付，调整导入的第一个和最后一个地址中有足够余额。
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入钱包私钥的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「手动输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (19).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (310).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包私钥，**&#x4E00;行仅输入一个私钥，按回车键换行

<figure><img src="../../../.gitbook/assets/image (263).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 点&#x51FB;**「上传文件」**&#x6309;钮，弹出文件上传窗口。

<figure><img src="../../../.gitbook/assets/image (20).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (251).png" alt=""><figcaption></figcaption></figure>

2. 导入钱包私钥信息文件，显示私钥信息。\
   请通过 CiaoTool 模板文件导入，以确保私钥准确导入。

<figure><img src="../../../.gitbook/assets/image (317).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (22).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下&#x65B9;**「捆绑卖出」**&#x6309;钮，并等待卖出程序完成。
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>什么是 PumpSwap 多地址捆绑卖出功能？</strong></summary>

多地址捆绑卖出是指通过多个钱包在同一区块内同步执行卖出操作。通过将多笔交易打包执行，可以减少时间差带来的价格波动，从而降低滑点并提升整体执行效率，适用于退出、止盈等关键交易阶段。

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
