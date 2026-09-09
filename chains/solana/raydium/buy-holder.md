---
description: >-
  专为 Raydium
  平台提供的自动化新地址买入工具。支持全自动生成新地址并执行买入，真实交易助力优化链上数据。稳步提升链上持币人数，全面优化代币分布的数据呈现。
---

# Solana - 提升持币人数教程

{% hint style="info" %}
**CiaoTool Raydium 提升持币人数功能**现已全面支持 **AMM V4、CLMM、CPMM** 全部的流动性池类型
{% endhint %}

## 功能介绍

**CiaoTool Solana 提升持币人数**是一款面向 Raydium 的多地址代币分配工具。系统可批量生成新钱包、分配交易资金，并由各钱包分别买入指定代币，使代币保留在对应地址中，形成持续有效的持币账户。

立即在 Solana 上，用 CiaoTool 进提升持币人数操作：

{% embed url="https://ciaotool.io/zh-Hans/raydium/new-address-holders" %}

***

## 核心优势

* **批量创建钱包：** 自动生成并管理多个独立地址
* **自动分配资金：** 为各钱包配置买入所需的 SOL
* **多地址买入：** 根据预设金额分别执行代币购买
* **保留代币余额：** 买入后代币继续存放在各钱包中
* **结果统一导出：** 导出钱包信息、持仓数量及交易记录
* **本地签名：** 私钥仅在浏览器本地用于交易授权

***

## 「**提升持币人数**」**与**「**提升交易人数**」**有什么区别？**

| 功能         | 提升类型     | 提升重点       |
| ---------- | -------- | ---------- |
| **提升持币人数** | 持币地址数量   | 共识分布、长期持有人 |
| **提升交易人数** | 交易过的地址数量 | 活跃度、成交参与感  |

***

## **图文指南**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角【连接钱包】按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (748).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择交易对及池模式

#### 交易币对

可以选择输入代币地址，也可以选择当前钱包拥有的代币进行交易操作。

* **价值代币：**&#x6267;行交易操作时，用以支付币对价格的代币地址
* **做市代币：**&#x6267;行交易操作时，用以实现市值管理策略目标的代币地址

<figure><img src="../../../.gitbook/assets/image (843).png" alt=""><figcaption></figcaption></figure>

#### 池模式

选择要进行做市的池子，并确保该池子存在所选交易币对。

<figure><img src="../../../.gitbook/assets/image (845).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 注资钱包

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

买入所产生的链上费用、SOL账户租金（自动退回）及平台服务费均由**主钱包**统一支付。页面底部会显示所需余额预估，请务必确保主钱包余额**高于预估金额**，否则可能导致交易失败。

每个新地址 **SOL 账户租金** 还需支付 **0.00203928 SOL**。

<figure><img src="../../../.gitbook/assets/image (881).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 生成与买入设置

{% hint style="danger" %}
<mark style="color:$danger;">**钱包下载**</mark>

所有钱包内均会保留代币以实现持有代币状态。为避免给您带来资金损失，请务必将私钥文件下载并妥善保管，以便您后续继续使用该钱包进行做市、转账、回收资金、关闭账户等操作。
{% endhint %}

{% tabs %}
{% tab title="生成钱包" %}
生成指定数量的新钱包，并完成买入操作，提升交易人数。

<figure><img src="../../../.gitbook/assets/image (883).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="交易金额" %}
设置每个新钱包的买入金额

<figure><img src="../../../.gitbook/assets/image (882).png" alt=""><figcaption></figcaption></figure>

* 固定数量：所有新钱包按照指定的数量，完成代币买入。
* 随机数量：每个新钱包均在规定范围内随机买入完成。
{% endtab %}

{% tab title="交易间隔" %}
可自由设置新地址完成交易的执行间隔时间。

<figure><img src="../../../.gitbook/assets/image (855).png" alt=""><figcaption></figcaption></figure>

* **固定时间**\
  所有交易按固定时间提交广播。
* **随机时间**\
  将会在指定的时间范围内随机提交，模拟真实交易。
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 发送设置

* **RPC 发送**\
  通过 RPC 节点统一广播交易，无需支付 Jito 小费。
* **Jito Bundle**\
  通过 Jito 小费提升上链优先级。

<figure><img src="../../../.gitbook/assets/image (857).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 核实信息

程序自动运行，查看确认页面并核对：

* [x] 新地址数量
* [x] 买入本金
* [x] 预计费用消耗

<figure><img src="../../../.gitbook/assets/image (884).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 启动交易

{% hint style="danger" %}
关闭 / 刷新页面，机器人策略亦会**立即停止**。请保持策略执行期间，将网页持续处于后台并运行状态。为保证策略执行之必要，**该功能不推荐于**「**移动电子设备**」**使用。**
{% endhint %}

确认信息无误后，点击下方「**开始**」按钮，即可开启交易程序。
{% endstep %}
{% endstepper %}

***

## **常见问题**

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

***

## **寻求支持**

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
