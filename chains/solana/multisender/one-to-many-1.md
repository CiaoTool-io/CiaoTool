---
description: 一对多转账是一种高效便捷的代币分发工具，支持将同一钱包中的 SOL 或 SPL 代币批量发送至无限个接收地址，适用于空投、奖励发放和批量结算等场景。
hidden: true
---

# Solana - 批量转账 | 一对多转账教程

{% hint style="info" %}
当前&#x662F;**「Solana - 一对多转账」**&#x6559;程页面，点击[**「EVM - 一对多转账」**](../../../tools/multisender/one-to-multi/one-to-many.md)以查看 BSC、opBNB、Base、X Layer、IoTeX、BOT、Robinhood Chain 等 EVM 网络一对多转账教程
{% endhint %}

## CiaoTool Solana 一对多转账是什么？ <a href="#definition" id="definition"></a>

<figure><picture><source srcset="../../../.gitbook/assets/屏幕截图 2026-09-04 142205.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (711).png" alt="CiaoTool BSC 批量转账 一对多转账页面"></picture><figcaption></figcaption></figure>

**CiaoTool Solana 一对多转账**是一款高效链上资产分发工具。它允许用户突破传统单笔转账的限制，全自动调度将单个主钱包中的 **SOL（原生代币）**&#x6216;**任何 SPL 代币**，在同一次操作中批量发送至数百个不同的接收地址。

相较于「逐笔复制地址、手动签名转账」的传统模式，该功能的核心机制在于「底层批量指令聚合」。系统会将海量的独立转账指令通过智能合约整合为一个不可分割的数据包提交至链上。这种机制不仅将原本需要耗费数小时的机械性工作缩短至一键秒级完成，更通过合并同类项大幅平摊了整体的网络矿工费，是项目方进行空投分发、团队结算或做市前置分仓的核心基建。

此工具尤其适用于：

* 空投和代币分发
* DAO收益和奖励
* 向用户批量付款
* 营销活动和Web3增长策略

立即在 Solana 上，用 CiaoTool​ 批量转账功能进行一对多转账操作：

{% embed url="https://ciaotool.io/zh-hans/transfer/one-to-many" %}

***

## 为什么选择 CiaoTool 代币空投（一对多转账）？ <a href="#advantage" id="advantage"></a>

CiaoTool 为 Solana Chain 上的海量资产调拨提供了一种兼顾绝对安全与极简操作的专业解决方案。对于需要高频、大批量分发代币或基础燃料的用户而言，该工具构建了高效且稳健的执行防线： ​ ​

**百倍提升效率：** 彻底免去人工频繁切换账号、复制粘贴地址与重复授权签名的繁琐流程，支持一键并发执行成百上千笔转账，实现链上资产的极速流转。 ​

**极致削减成本：** 通过底层智能合约的多重调用与批量打包技术，将多笔转账聚合为单次链上交互，最大程度摊薄网络费用，显著降低大规模分发的资金损耗。 ​

**灵活的矩阵配置：** 支持通过 Excel 电子表格文件一键批量导入目标地址列表与对应的分发额度。支持自定义等额、定额或随机金额分配，完美适配复杂多变的空投策略与持币分布需求。 ​

**本地安全环境：** 采用纯前端本地执行机制，私钥仅在本地环境中用于交易签名，在极速提升交易效率的同时，全方位保障多钱包资产的绝对安全。

***

## **图文指南** <a href="#solana-one-to-multi-guide" id="solana-one-to-multi-guide"></a>

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角【连接钱包】按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (712).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择转账钱包

{% hint style="danger" %}
使用其他私钥钱包模式时，请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (715).png" alt=""><figcaption></figcaption></figure>

**当前连接钱包：**&#x76F4;接使用当前钱包直接进行转账操作，无需使用私钥，资金更安全。

**其他私钥钱包：**&#x4F7F;用私钥的形式进行转账操作，无需切换当前钱包快速调用备用钱包。
{% endstep %}

{% step %}
### 选择转账代币

可以选择 SOL，也可以选择当前钱包拥有的代币进行转账。

<figure><img src="../../../.gitbook/assets/image (716).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入接收地址

接收钱包数量没有限制，支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入接收地址的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「批量输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (717).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x6BCF;行仅输入一个钱包地址，可在地址后追加数量。

```
address, 300
```

<figure><img src="../../../.gitbook/assets/image (719).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (720).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 下载 CiaoTool 模板文件，并将信息导入到文件内。

<figure><img src="../../../.gitbook/assets/image (722).png" alt=""><figcaption></figcaption></figure>

2. 点&#x51FB;**「导入文件」**&#x6309;钮，弹出文件上传窗口。

<figure><img src="../../../.gitbook/assets/image (721).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (720).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入转账金额

支&#x6301;**「逐一输入」「统一金额」**&#x548C;**「随机范围」**&#x4E09;种转账金额类型。

<figure><img src="../../../.gitbook/assets/image (726).png" alt=""><figcaption></figcaption></figure>

1. **逐一输入**\
   在输入框中，逐一输入转账金额数量。
2. **统一金额**\
   点击转账数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「输入金额」**&#x9009;项，所有地址将统一转账数量。

<figure><img src="../../../.gitbook/assets/image (725).png" alt=""><figcaption></figcaption></figure>

3. **随机范围**\
   点击转账数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「随机范围」**&#x9009;项，输入金额范围，所有地址将接收到指定范围内数额。

<figure><img src="../../../.gitbook/assets/image (727).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (728).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 转账时间

可自由设置各地址转账执行间隔时间。

<figure><img src="../../../.gitbook/assets/image (729).png" alt=""><figcaption></figcaption></figure>

1. **固定时间**\
   设置为 0 时，所有转账立即提交广播，快速分发资金。
2. **随机时间**\
   转账将会在指定的时间范围内随机提交，模拟真实转账行为，但需要保持页面以持续执行。
{% endstep %}

{% step %}
### 发送形式

系统将根据收款地址数量自动分组，每组最多 5 个收款地址。

<figure><img src="../../../.gitbook/assets/image (730).png" alt=""><figcaption></figcaption></figure>

1. **RPC 发送**\
   通过 RPC 节点统一广播转账交易，无需支付 Jito 小费，各笔交易不保证按提交顺序执行。
2. **Jito Bundle**\
   每包最多 25 个收款地址（5 组），通过 Jito 小费提升上链优先级并按顺序执行。
{% endstep %}

{% step %}
### 核实信息

点&#x51FB;**「下一步」**&#x8FDB;入确认页面，核对收款地址及数量、转账总额和预估费用，确认无误后再提交转账。

<figure><img src="../../../.gitbook/assets/image (731).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下方「**确认并发送**」按钮，您可以实时查看转账程序完成情况，并等待转账程序完成，。

<figure><img src="../../../.gitbook/assets/image (732).png" alt=""><figcaption></figcaption></figure>
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

可以。你可以为每个地址设置不同的转账数量，也可以设置统一的金额和随机金额区间分发给所有目标地址。

</details>

<details>

<summary><strong>操作是否安全？</strong></summary>

平台采用纯前端签名机制，您的私钥绝不会被上传或储存在任何服务器上，所有交易均在本地浏览器完成签名，从技术层面确保平台无法访问您的私钥。

</details>

<details>

<summary><strong>一次可以发送到多少个地址？</strong></summary>

没有数量限制。

</details>

<details>

<summary><strong>可以同时转多种代币吗？</strong></summary>

当前版本支持选择单一 SPL 代币或 SOL 进行批量转账；如需多种资产分发，可多次执行操作。

</details>

***

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
