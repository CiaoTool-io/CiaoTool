---
description: 方便快捷地将分散在多个账户中的 SOL 或 SPL 代币统一归集到一个主账户，提高资金管理的效率，同时减少交易成本和时间。
---

# Solana - 批量转账 | 多对一转账教程

{% hint style="info" %}
当前&#x662F;**「Solana 多对一转账」**&#x6559;程页面，点击[**「EVM - 多对一转账」**](../../../tools/multisender/multi-to-one/many-to-one.md)以查看 BSC、opBNB、Base、X Layer、IoTeX、BOT、Robinhood Chain 等 EVM 网络多对一转账教程
{% endhint %}

## CiaoTool Solana 多对一转账是什么？ <a href="#definition" id="definition"></a>

<figure><picture><source srcset="../../../.gitbook/assets/屏幕截图 2026-09-04 170749.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (733).png" alt="CiaoTool Solana 批量转账 多对一转账页面"></picture><figcaption></figcaption></figure>

**CiaoTool  Solana 多对一转账**是一款高效链上资产回笼与多钱包资金管理工具。它允许用户在单次可视化操作中，将分散在成百上千个子钱包中的 **SOL（原生代币）**&#x6216;**任何 SPL 代币**，全自动地集中汇聚至一个主地址中。

相较于「逐笔复制地址、手动签名转账」的传统模式，该功能的核心机制在于「底层批量指令聚合」。系统会将海量的独立转账指令通过智能合约整合为一个不可分割的数据包提交至链上。这种机制不仅将原本需要耗费数小时的机械性工作缩短至一键秒级完成，更通过合并同类项大幅平摊了整体的网络费。

立即在 Solana 上，用 CiaoTool​ 批量转账功能进行多对一转账操作：

{% embed url="https://ciaotool.io/zh-Hans/transfer/many-to-one" %}

***

## 为什么选择 CiaoTool 多对一转账？ <a href="#advantage" id="advantage"></a>

CiaoTool 为 Solana 网络上的海量资产调拨提供了一种兼顾绝对安全与极简操作的专业解决方案。对于需要高频、大批量分发代币或基础燃料的用户而言，该工具构建了高效且稳健的执行防线： ​ ​

**百倍提升效率：**\
彻底免去人工频繁切换账号、复制粘贴地址与重复授权签名的繁琐流程，支持一键并发执行成百上千笔转账，实现链上资产的极速归集。 ​

**灵活的矩阵配置：**\
支持通过 Excel 电子表格文件一键批量导入目标地址列表与对应的分发额度。支持自定义等额、定额或随机金额分配，完美适配复杂多变的空投策略与持币分布需求。 ​

**本地安全环境：**\
采用纯前端本地执行机制，私钥仅在本地环境中用于交易签名，在极速提升交易效率的同时，全方位保障多钱包资产的绝对安全。

***

## **图文指南**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角【连接钱包】按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (748).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择转账代币

可以选择 SOL，也可以选择当前钱包拥有的代币进行转账。

<figure><img src="../../../.gitbook/assets/image (735).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入来源钱包私钥

{% hint style="danger" %}
**「多对一转账」**&#x529F;能仅支持私钥导入以进行转账操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

导入钱包数量没有限制，支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入来源地址的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「批量输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (736).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x6BCF;行仅输入一个钱包私钥，可在私钥后追加数量。

```
privateKey, 300
```

<figure><img src="../../../.gitbook/assets/image (737).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (738).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 下载 CiaoTool 模板文件，并将信息导入到文件内。

<figure><img src="../../../.gitbook/assets/image (739).png" alt=""><figcaption></figcaption></figure>

2. 点&#x51FB;**「导入文件」**&#x6309;钮，弹出文件上传窗口。

<figure><img src="../../../.gitbook/assets/image (740).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (738).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入转账金额

支&#x6301;**「逐一输入」「全部」「输入金额」**&#x548C;**「保留金额」**&#x56DB;种转账金额类型。

<figure><img src="../../../.gitbook/assets/image (741).png" alt=""><figcaption></figcaption></figure>

1. **逐一输入**\
   在输入框中，逐一输入转账金额数量。
2. **全部**\
   点击转账数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「全部」**&#x9009;项，所有来源钱包将目标代币全部转账到接收地址。

<figure><img src="../../../.gitbook/assets/image (742).png" alt=""><figcaption></figcaption></figure>

3. **输入金额**\
   点击转账数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「输入金额」**&#x9009;项，所有来源钱包将根据指定数量将目标代币转账到接收地址。
4. **保留金额**\
   点击转账数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「保留金额」**&#x9009;项，所有来源钱包保留指定数量的目标代币，并将剩余代币全部转账到接收地址。
{% endstep %}

{% step %}
### 独立手续费钱包

{% hint style="danger" %}
请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

独立手续费钱包统一支付网络费、平台服务费、Jito 小费和接收 ATA 租金。

<figure><img src="../../../.gitbook/assets/image (743).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 接收地址

输入接收地址，以接收来源钱包转账的指定代币。可以直接点击「当前钱包」快速使用当前连接钱包地址。

<figure><img src="../../../.gitbook/assets/image (744).png" alt=""><figcaption></figcaption></figure>
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

系统将根据收款地址数量自动分组，每组最多 5 个转账地址。

<figure><img src="../../../.gitbook/assets/image (730).png" alt=""><figcaption></figcaption></figure>

1. **RPC 发送**\
   通过 RPC 节点统一广播转账交易，无需支付 Jito 小费，各笔交易不保证按提交顺序执行。
2. **Jito Bundle**\
   每个捆绑包最多 25 个转账地址（5 组），通过 Jito 小费提升上链优先级并按顺序执行。
{% endstep %}

{% step %}
### 核实信息

点&#x51FB;**「下一步」**&#x8FDB;入确认页面并核对：

* [x] 费用钱包地址
* [x] 归集地址及数量、转账总额
* [x] 本次转账预估费用

<figure><img src="../../../.gitbook/assets/image (746).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下方「**确认并发送**」按钮，您可以实时查看转账程序完成情况，并等待转账程序完成。

<figure><img src="../../../.gitbook/assets/image (732).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>什么是多对一批量转账？</strong></summary>

多对一批量归集指将多个钱包地址中持有的代币统一转入一个主地址，**便于集中管理资产、统一调配资金**。

</details>

<details>

<summary><strong>如何导入接收地址？</strong></summary>

你可以手动输入地址，也可以上传 CSV 文件导入目标地址列表，系统会自动识别并展示预览。

</details>

<details>

<summary><strong>操作是否安全？</strong></summary>

平台采用纯前端签名机制，您的私钥绝不会被上传或储存在任何服务器上，所有交易均在本地浏览器完成签名，从技术层面确保平台无法访问您的私钥。

</details>

<details>

<summary><strong>一次可以多少个地址转账？</strong></summary>

得益于私钥导入的模式，多对一转账功能免除了逐一钱包签署的繁复工作，发送地址没有任何数量限制。

</details>

<details>

<summary><strong>可以同时转多种代币吗？</strong></summary>

当前版本支持选择单一 SPL 代币或 SOL 进行批量转账；如需多种资产归集，可多次执行操作。

</details>

***

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
