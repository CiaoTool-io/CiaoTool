---
description: 使用 CiaoTool 交易量机器人，在币安 Alpha 上持续执行代币买卖。集中配置参与钱包和金额，轻松管理代币的链上交易活动。
---

# 币安 Alpha - 交易量机器人指南

## 功能介绍

**CiaoTool 币安 Alpha 交易量机器人**是一款面向 币安 Alpha 的免代码交易工具。当你需要持续执行代币买卖时，可以提前选好交易对、配置参与钱包并设定交易金额。启动后，机器人会按任务设置提交 Swap，省去反复切换钱包、填写金额和逐笔提交的操作。随着买卖陆续成交，代币的链上交易活跃度随之提升，成交量也会在目标池中逐步累积。

{% embed url="https://bsc.ciaotool.io/zh-Hans/bscalpha/volume-trading-alpha" %}

***

## **图文指南**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 BSC 链的钱包

<figure><img src="../../../.gitbook/assets/image (467).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入做市代币地址

{% hint style="info" %}
V2 / V3 功能页面略有不同，点击下方按钮切换并显示 V2 / V3 教程。
{% endhint %}

选择输入支付/交易资产地址，自动检测并匹配当前币对价格。

<figure><img src="../../../.gitbook/assets/image (27).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 买卖参数设置

支&#x6301;**「固定数量」「随机范围」「余额比例」「固定留存」「全部数量」**&#x4E94;种交易金额类型。

买入时使用支付资产，卖出时使用交易资产。

<figure><img src="../../../.gitbook/assets/image (23).png" alt=""><figcaption></figcaption></figure>

1. **固定数量**\
   所有钱包每次按照固定设定值 买 / 卖 资产。
2. **随机范围**\
   所有钱包每次按照指定范围区间 买 / 卖 资产。
3. **余额比例**\
   所有钱包每次按照实时余额比例 买 / 卖 资产。
4. **固定留存**\
   所有钱包每次将留存固定值在钱包余额内，其余全部用于 买 / 卖 资产。
5. **全部数量**\
   所有钱包将每次将全部余额用于 买 / 卖 资产。
{% endstep %}

{% step %}
### 执行参数

#### 买卖顺序

决定每个钱包每次交易的买卖顺序，依次执行完成买卖两笔。

#### 钱包顺序

```
轮询：A → B → C → A → B → C → A → B → C
随机：C → A → B → B → C → A → A → C → B（示例）
连续：A → A → A → B → B → B → C → C → C
```

* **轮序：**&#x6309;照导入钱包的顺序，依次循环地完成买卖操作。
* **随机：**&#x968F;机钱包顺序，依次循环地完成买卖操作。
* **连续：**&#x6309;照导入钱包的顺序，依次批量完成买卖操作。

#### 并发数

同时执行交易组合的数量，默认 1 组买卖，最多支持 5 个买卖同时并发。

选择「连续」顺序，仅支持并发 1。

#### 交易间隔

通过指定区间，随机交易间隔，有效模拟真实链上交易。

#### 停止条件

* 循环次数：完成买卖循环次数的数量，达到指定次数后自动停止。
* 价格范围：设定支付资产的价格范围，超出范围自动停止。选择「连续」顺序，仅支持循环次数。

#### 滑点与交易有效期

滑点限制可接受的成交价格偏差，交易有效期限制单笔交易的执行时限；交易失败或处于待确认状态时，机器人暂停后续执行。

#### Gas 价格与Swap Gas Limit

Gas 价格是每单位 Gas 的费用；

Swap Gas Limit 是每笔兑换的 Gas 用量上限，实际网络费按实际消耗的 Gas × Gas 价格计算。

#### 服务费支付钱包

将用于支付交易量机器人服务费的钱包私钥导入。
{% endstep %}

{% step %}
### 导入交易钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

多地址导入仅支持 私钥导入以进行兑换操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入交易地址私钥的类型。最多支持 20 个地址。

1. 点&#x51FB;**「导入私钥」**&#x6309;钮，弹出输入框。

<figure><img src="../../../.gitbook/assets/image (553).png" alt=""><figcaption></figcaption></figure>

2. 手动输入或导入私钥文件，确认框中显示私钥后点击确认。

<figure><img src="../../../.gitbook/assets/image (474).png" alt=""><figcaption></figcaption></figure>

使用 CiaoTool 模板文件导入，并保存确定导入并显示在输入框内。\
点击下载并查看模板：

{% file src="../../../.gitbook/assets/EVM_Demo.xlsx" %}
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下&#x65B9;**「开始执行」**&#x6309;钮，并等交易程序完成。
{% endstep %}
{% endstepper %}

***

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
