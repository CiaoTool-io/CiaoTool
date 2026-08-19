---
description: >-
  专为 Raydium
  平台提供的自动化新地址买入工具。支持全自动生成新地址并执行买入，真实交易助力优化链上数据。稳步提升链上持币人数，全面优化代币分布的数据呈现。
---

# Solana - 提升持币人数教程

{% hint style="info" %}
**CiaoTool Raydium 提升持币人数功能**现已全面支持 **AMM、CLMM、CPMM** 全部的流动性池类型，请先切换到指定池子功能页面进行机器人操作，满足不同场景下的快捷做市服务。
{% endhint %}

## CiaoTool Solana 提升持币人数功能是什么？

**CiaoTool Solana 提升持币人数功能**是一款专为 Solana 生态 **Raydium 平台**打造的链上数据与资产分布优化工具。它允许用户通过设定参数，全自动批量生成全新钱包地址，并控制这些地址在盘口独立执行代币买入操作。

与「提升交易人数」在交易后回集资金并销毁账户的机制截然不同，该功能在完成盘口买入后，会将购买的代币永久保留在这些新生成的独立地址中。这不仅能在盘口产生真实的自然买入记录，更直接增加了代币的链上独立持币地址数，从而有效打散筹码，使代币的整体分布结构更加均匀、健康。

立即在 Solana 上，用 CiaoTool 进提升持币人数操作：

{% embed url="https://ciaotool.io/zh-CN/raydium/newaddr-buyers-holders" %}

***

## 为什么选择 CiaoTool Solana 提升持币人数功能？

CiaoTool 为 Raydium 平台上的持币数据优化提供了一种兼顾真实性与高效执行的专业解决方案。对于需要完善早期筹码分布或稳步提升项目数据健康度的用户，该工具构建了稳健的自动化防线：

* **真实提升持币人数：**&#x901A;过大量新地址在盘口进行真实的资金买入并独立持有代币，稳步且真实地增加链上持币地址总数。
* **优化筹码分布结构：**&#x5C06;买入的代币合理分散在众多完全独立的钱包中，有效避免单一地址筹码过度集中，美化代币分布气泡图。
* **全自动执行闭环：**&#x4E00;键自动完成“批量生成地址、主钱包分发 SOL、独立执行买入”的全流程，彻底免去人工逐一创建与转账的繁琐操作。
* **本地安全与数据导出：**&#x91C7;用纯前端本地执行机制，所有新生成的私钥仅在本地运行。系统支持一键导出所有新地址的私钥表格，方便用户后续对分散资产进行安全管理。

***

## 「**提升持币人数**」**与**「**提升交易人数**」**有什么区别？**

| 功能         | 提升类型     | 提升重点       |
| ---------- | -------- | ---------- |
| **提升持币人数** | 持币地址数量   | 共识分布、长期持有人 |
| **提升交易人数** | 交易过的地址数量 | 活跃度、成交参与感  |

***

## **图文指南 |** Solana **提升持币人数**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (308).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择交易代币

可以选择输入代币地址，也可以选择当前钱包拥有的代币进行买入操作。

<figure><img src="../../../.gitbook/assets/image (368).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择买入地址数量

选择或输入买入地址数量，以增加交易人数。

<figure><img src="../../../.gitbook/assets/image (369).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入买入金额

每个新建钱包买入所花费的金额，可设置特定交易范围，在范围内随机买入代币。
{% endstep %}

{% step %}
### 生成钱包并下载私钥文件

由于「**提升持币人数**」与「**提升交易人数**」不同，所有钱包内均会保留代币以实现持有代币状态。为避免给您带来资金损失，请务必将私钥文件下载并妥善保管，以便您后续继续使用该钱包进行做市、转账、回收资金、关闭账户等操作。
{% endstep %}

{% step %}
### 导入主钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

当&#x524D;**「提升持币人数功能」**&#x529F;能支持仅支持私钥导入以进行交易操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

{% hint style="info" %}
<mark style="color:$primary;">**主钱包设置**</mark>

买入所产生的链上费用、SOL账户租金及平台服务费均由**主钱包**统一支付。页面底部会显示所需余额预估，请务必确保主钱包余额**高于预估金额**，否则可能导致交易失败。

每个新地址 **SOL 账户租金** 需支付 **0.00203928 SOL**，将独立存储于每个交易地址中，根据您的策略按需关闭账户并退回租金。
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (370).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 确认交易

{% hint style="danger" %}
关闭 / 刷新页面，机器人策略亦会**立即停止**。请保持策略执行期间，将网页持续处于后台并运行状态。为保证策略执行之必要，**该功能不推荐于**「**移动电子设备**」**使用。**
{% endhint %}

确认信息无误后，点击下&#x65B9;**「开始」**&#x6309;钮，并等交易程序完成。
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>什么是 Solana 提升持币人数？</strong></summary>

这是一款链上数据优化工具。系统会自动创建大量全新的钱包地址，向其分配所需资金并在盘口执行代币买入操作。买入的代币将直接保留在这些新地址中，主要用于真实提升代币的持币人数与优化筹码分布。

</details>

<details>

<summary><strong>这与直接向多个地址批量转账（一对多转账）有什么区别？</strong></summary>

批量转账（一对多转账）仅在链上产生简单的代币转移记录，不会影响市场价格，也不会增加交易热度。而“新地址买入”是通过每个新钱包在 Raydium 盘口执行真实的 DEX 交易。这不仅增加了持币人数，还能同时提升盘口总交易额和交易者数量，是一种更全面、更自然的链上数据优化方式。

</details>

<details>

<summary><strong>生成的大量新地址私钥去哪了？我以后如何管理这些代币？</strong></summary>

在执行流程完毕后，系统会在本地为您生成一份包含所有新地址及其对应私钥的表格文件。您可以一键下载并妥善保管该文件，以便未来随时导入 CiaoTool 的“批量交易”或“批量归集”等功能中，对这些分散的资产进行统一管理。

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
