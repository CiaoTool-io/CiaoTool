---
description: >-
  专为 Meteora 平台提供的防夹交易执行工具。在同一区块内完成买卖闭环，有效降低 MEV
  机器人交易干扰并降低资金磨损。稳步提升代币交易量，全面优化盘口数据的自然度。
---

# Meteora - 防夹交易量机器人指南

{% hint style="info" %}
**CiaoTool Meteora 多地址捆绑买入**现已全面支持 **DBC、DLMM、DAMM V2** 全部的流动性池类型
{% endhint %}

## 功能介绍

**CiaoTool Meteora 防夹交易量机器人**是一款面向 Meteora 的自动化交易工具。用户可自定义交易金额、执行频率和参与钱包，由系统持续执行多地址买卖操作，提升代币交易量与链上活跃度。

该功能采用同区块聚合机制，将关联的买入与卖出交易组成 Bundle，并按预设顺序连续执行，减少交易间隙被 MEV 机器人插入的风险，降低高频交易过程中的滑点与资金损耗。

立即在 Meteora 上，用 CiaoTool 进行防夹交易量机器人操作：

{% embed url="https://ciaotool.io/zh-Hans/meteora/anti-mev" %}

***

## 核心优势

* **降低夹击风险：** 买入与卖出交易在同一区块内连续执行，减少被其他交易插入的机会
* **控制交易损耗：** 缩短买卖间隔，降低价格波动、滑点及 MEV 干扰带来的损耗
* **提升交易数据：** 通过多地址持续交互，增加交易量、活跃度及独立交易地址数
* **参数灵活：** 支持自定义交易金额、执行间隔、运行次数和参与钱包
* **自动循环：** 一键启动买卖任务，减少重复手动操作
* **本地签名：** 私钥仅在浏览器本地用于交易授权，无需上传

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

<figure><img src="../../../.gitbook/assets/image (924).png" alt=""><figcaption></figcaption></figure>
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

<figure><img src="../../../.gitbook/assets/image (861).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x6BCF;行仅输入一个钱包私钥，可在私钥后追加数量。

```
privateKey, 300
```

<figure><img src="../../../.gitbook/assets/image (737).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (864).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 下载 CiaoTool 模板文件，并将信息导入到文件内。

<figure><img src="../../../.gitbook/assets/image (862).png" alt=""><figcaption></figcaption></figure>

2. 点击![](<../../../.gitbook/assets/image (848).png>)**「导入文件」**&#x6309;钮，弹出文件上传窗口。
3. 点&#x51FB;**「确定导入」**，将所有地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (863).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入交易金额

支&#x6301;**「逐一输入」「输入金额」「随机范围」**&#x548C;**「全部」四**种转账金额类型。

<figure><img src="../../../.gitbook/assets/image (865).png" alt=""><figcaption></figcaption></figure>

1. **逐一输入**\
   在输入框中，逐一输入交易金额数量。
2. **统一金额**\
   点击交易数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「输入金额」**&#x9009;项，所有地址将统一兑换数量。

<figure><img src="../../../.gitbook/assets/image (866).png" alt=""><figcaption></figcaption></figure>

3. **随机范围**\
   点击交易数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「随机范围」**&#x9009;项，输入金额范围，所有地址将兑换指定范围内数额。
4. **全部**\
   点击转账数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「全部」**&#x9009;项，所有钱包将所选代币全部兑换为指定代币。
{% endstep %}

{% step %}
### 交易参数设置

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

* [x] 当前执行钱包及交易数量
* [x] 费用预览

交易费用将由各钱包独立承担。
{% endstep %}

{% step %}
### 启动交易

{% hint style="danger" %}
关闭 / 刷新页面，机器人策略亦会**立即停止**。请保持策略执行期间，将网页持续处于后台并运行状态。为保证策略执行之必要，**该功能不推荐于**「**移动电子设备**」**使用。**
{% endhint %}

确认信息无误后，点击下方「**确认并开始执行**」按钮，即可开启批量兑换程序。
{% endstep %}
{% endstepper %}

## **常见失败案例**

* 捆绑包未成功打包，导致交易被拆分执行
* 流动性不足，买卖过程中滑点过大
* 小费不足，被优先级更高的交易抢占

***

## **常见问题**

<details>

<summary><strong>什么是 Meteora 防夹交易量机器人？</strong></summary>

该功能用于 Meteora 同一区块内执行买卖交易，形成交易闭环，从而降低交易路径暴露与外部干扰，提升执行稳定性与交易效率。

</details>

<details>

<summary><strong>什么是 MEV 机器人？</strong></summary>

MEV 机器人是区块链上的一种自动化套利程序。它们会实时监控网络中尚未确认的待处理交易。当发现有利可图的交易时，MEV 机器人会通过支付更高的网络费用（Gas）来操纵区块内的交易顺序，故意在普通用户的交易前后插入自己的买入和卖出订单，以此毫无风险地赚取差价利润，这种行为被称为“夹击攻击”。

</details>

<details>

<summary><strong>为什么需要防夹交易量机器人？普通工具有什么痛点？</strong></summary>

在使用普通的交易量机器人优化盘口活跃度时，买入和卖出指令通常是分离执行的。这极易成为 MEV 机器人的攻击目标：在您的程序执行买入前，MEV 机器人会抢先买入，导致您被迫以被推高的价格成交；而在您的程序执行卖出前，MEV 机器人又会抢先抛售。这种恶意的夹击拦截，会导致在正常的交易量优化过程中产生严重的滑点与巨额的交易磨损。防夹机器人的出现正是为了解决这一致命痛点。

</details>

<details>

<summary><strong>Jito 技术在防夹刷中起什么作用？</strong></summary>

Jito 可将关键交易打包发送至优先池，提高链上排序优先级，防止中间被插队。

</details>

<details>

<summary><strong>如何实现“防夹”并降低交易损耗的？</strong></summary>

该工具采用了底层的“同区块聚合执行”技术。系统会将您的买入指令与卖出指令在底层打包，确保这两笔双向交互在同一个区块内瞬间、连续地完成。由于两笔操作之间没有任何时间差，MEV 机器人无法在其中插入任何恶意订单，从而从根本上阻断了夹击行为，将交易量优化的资金磨损降至最低。

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
