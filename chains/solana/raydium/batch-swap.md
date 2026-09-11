---
description: >-
  专为 Raydium
  平台提供的多地址批量兑换与交易执行工具。支持快速将多个地址内的代币同步兑换为指定代币，大幅提升交易效率与时效性，特别适用于需要快速执行大量交易的场景。
---

# Solana - 批量交易教程

{% hint style="info" %}
**CiaoTool Raydium 批量交易**现已全面支持 **AMM V4、CLMM、CPMM** 全部的流动性池类型
{% endhint %}

## 功能介绍

**CiaoTool Solana 批量交易**是一款面向 Raydium 的多钱包自动化交易工具。用户可批量导入或选择多个钱包，分别设置交易方向和金额，一次执行指定代币的买入或卖出操作。

系统将配置转换为独立的交易任务，并通过多地址并发提交，减少逐个切换钱包、填写参数和重复签名的操作，提升大规模资产兑换与资金调度效率。

{% embed url="https://ciaotool.io/zh-Hans/raydium/batch-swap" %}

***

## 核心优势

* **批量执行：** 一次启动多个钱包的买入或卖出任务
* **并发提交：** 多笔交易在较短时间内广播，提升整体执行效率
* **灵活配置：** 支持为不同钱包分别设置交易方向及金额
* **统一管理：** 集中查看各钱包余额、交易状态及执行结果
* **快速兑换：** 支持将多个钱包中的资产批量兑换为目标资产
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

<figure><img src="../../../.gitbook/assets/image (845).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入钱包私钥

{% hint style="danger" %}
请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

{% hint style="info" %}
<mark style="color:$primary;">**操作钱包设置**</mark>

**Raydium 批量交易**导入钱包没有数量限制。交易手续费由每个钱包独立支付。
{% endhint %}

导入钱包数量没有限制，支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入来源地址的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「批量输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (861).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x6BCF;行仅输入一个钱包私钥

```
privateKey
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

* 滑点设置过低，币对价格超出额定范围
* 流动性不足，价格波动剧烈
* Jito 小费设置过低，被 MEV 机器人抢跑

***

## **常见问题 FAQ**

<details>

<summary><strong>什么是 Solana 批量交易？</strong></summary>

批量交易是指通过多地址自动执行买入或卖出操作，在设定的滑点范围内完成代币交换。该功能主要用于大规模资金的快速换仓或资产转换，在保证成交效率的同时尽量降低因滑点带来的损耗。

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
