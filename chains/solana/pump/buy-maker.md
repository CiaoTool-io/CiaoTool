---
description: >-
  专为 PumpFun
  平台提供的自动化新地址买入工具。支持全自动生成新地址并执行买入，完成后自动将资产回集至主钱包并关闭账户。以极低成本有效提升代币的独立买家数量，全面优化盘口数据表现。
---

# PumpFun - 提升交易人数教程

{% hint style="info" %}
**CiaoTool PumpFun 提升交易人数**现已全面支持官方 **SOL** 和 **USDC** 全部的价值代币，请先切换到指定代币页面进行机器人操作，满足不同场景下的快捷做市服务。
{% endhint %}

## CiaoTool PumpFun 提升交易人数功能是什么？

**CiaoTool PumpFun 提升交易人数功能**是一款专为 **Pump.fun 平台**打造的链上数据优化与自动化执行工具。它旨在帮助用户以极低的资金损耗，快速提升指定代币的独立钱包购买数量。

该功能的核心机制在于完整的“全自动执行闭环”：系统在底层全自动批量创建全新的钱包地址，并控制这些新地址在盘口执行代币的买入操作。在买入交互完成后，系统会自动将所购代币及剩余资金安全转入用户指定的主钱包中，并同步向 Solana 网络发送关闭这些临时账户的指令。这种机制不仅在链上留下了真实的新地址买入记录，更通过销毁账户回收了链上租金，从而以极低的成本使项目的活跃度数据在市场中脱颖而出。

立即在 PumpFun 上，用 CiaoTool 进提升交易人数操作：

{% embed url="https://ciaotool.io/zh-CN/pump/newaddr-buyers-markers" %}

***

## 为什么选择 CiaoTool PumpFun 提升交易人数功能？

CiaoTool 为 PumpFun 平台上的数据优化提供了一种兼顾极低成本与高执行效率的专业解决方案。对于需要快速提升盘口活跃买家指标的用户，该工具构建了稳健的自动化防线：

* **全自动执行闭环**：一键自动完成“生成新地址、执行买入、资产回集、关闭账户”的全流程，彻底免去繁琐的人工地址管理与资金归集操作。
* **极低成本提升交易人数：**&#x901A;过执行完毕即关闭临时账户的底层机制，有效回收 Solana 链上的账户租金，以极低的资金消耗快速增加独立买家数量。
* **优化市场数据表现：**&#x901A;过海量真实的新地址买入交互，显著提升代币在各类行情平台上的活跃交易者指标，改善市场数据呈现。
* **本地安全环境：**&#x91C7;用纯前端本地执行机制，所有临时生成的私钥及主钱包私钥仅在本地环境中用于交易签名，全方位保障回集资产的绝对安全。

***

## 「**提升交易人数**」**与**「**提升持币人数**」**有什么区别？**

| 功能         | 提升类型     | 提升重点       |
| ---------- | -------- | ---------- |
| **提升交易人数** | 交易过的地址数量 | 活跃度、成交参与感  |
| **提升持币人数** | 持币地址数量   | 共识分布、长期持有人 |

***

## **图文指南 |** PumpFun **提升交易人数**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (308).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择交易代币

可以选择输入代币地址，也可以选择当前钱包拥有的代币进行买入操作。

<figure><img src="../../../.gitbook/assets/image (373).png" alt=""><figcaption></figcaption></figure>
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
### 导入主钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

当&#x524D;**「提升交易人数功能」**&#x529F;能仅支持私钥导入以进行交易操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

{% hint style="info" %}
<mark style="color:$primary;">**主钱包设置**</mark>

买入所产生的链上费用、SOL账户租金（自动退回）及平台服务费均由**主钱包**统一支付。页面底部会显示所需余额预估，请务必确保主钱包余额**高于预估金额**，否则可能导致交易失败。

每个新地址 **SOL 账户租金** 需支付 **0.00203928 SOL**，在交易进程完成后自动退回主钱包。
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

<summary><strong>什么是 PumpFun 提升交易人数？</strong></summary>

这是一款自动化链上数据优化工具。它能够自动创建大量新钱包地址去执行代币买入操作，并在买入完成后自动将资产转回主钱包并注销新地址。其主要目的是增加代币的独立买家数量。

</details>

<details>

<summary><strong>为什么要“关闭账户”？</strong></summary>

在 Solana 网络中，创建任何新代币账户都需要抵押一笔极少的 SOL 作为“账户租金”。该工具在完成买入和资金回集后，会自动执行关闭账户的指令。此操作能够将先前抵押的租金全额赎回，从而将增加独立买家数量的资金损耗降至最低。

</details>

<details>

<summary><strong>新地址买入的代币去哪里了？</strong></summary>

资金绝不会丢失。系统在执行完买入操作后，会立即触发转账程序，将新地址中购买的代币全自动、无缝地全额转入您提前设定好的“主钱包”中统一集中管理。

</details>

<details>

<summary><strong>新地址买入和普通买入有什么区别？</strong></summary>

普通买入通常使用您现有的、带有交易历史的单一主钱包执行，所有的资金流向和持仓变化都会集中反映在该地址上，极易被链上工具追踪。

而“新地址买入”则是通过系统全自动生成全新的钱包地址来执行买入。这些新地址在链上呈现为完全独立的全新参与者，与您的主钱包无任何直接的转账前置关联。这种机制能有效隐匿真实的资金流向与筹码分布，在提供高隐私保护的同时，更适合专业团队用于链上数据优化与流动性管理的场景。

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
