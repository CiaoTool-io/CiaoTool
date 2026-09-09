---
description: >-
  专为 Bonk.fun 打造的高效批量卖出工具，通过同区块聚合执行多地址卖出，有效降低 MEV
  夹击风险与资金损耗，优化团队资产出仓效率，是保障交易成本效益的专业利器。
---

# Bonk - 多地址捆绑卖出教程

{% hint style="info" %}
**CiaoTool Bonk 多地址捆绑卖出**现已全面支持官方 **SOL** 和 **USD1** 全部的价值代币，输入代币地址并切换价值代币。
{% endhint %}

## 功能介绍

**CiaoTool Bonk 多地址捆绑卖出**是一款面向 B的n多钱包批量卖出工具。用户可配置多个卖出钱包及代币数量，系统自动构建交易并通过 Bundle 按预设顺序提交。

正常执行时，包内卖出交易将在同一区块连续完成，减少多笔交易之间被其他交易插入的风险，提升批量卖出的执行一致性与管理效率。

**适用场景：**

* 多钱包批量减仓或退出
* 项目金库及运营资金回收
* 做市与流动性仓位调整
* 多账户资产归集前的统一卖出
* 自动化交易与执行测试

立即在 Bonk.fun 上，用 CiaoTool 进行多地址捆绑卖出操作：

{% embed url="https://ciaotool.io/zh-Hans/bonk/multi-address-sell" %}

***

## 为什么选择 CiaoTool Bonk 多地址捆绑卖出？

**CiaoTool** 为 **Bonk** 上的资产管理与流动性调整提供了一种兼顾效率与成本保护的专业方案。无论您是执行专业做市的资产变现、规避 MEV 夹击的批量卖出交易，还是稳健地管理代币的链上流动性，其多地址捆绑卖出功能都能通过同区块智能聚合技术，免去您在繁琐流程中频繁更换钱包地址的操作麻烦，成倍节省宝贵的运营时间，全方位保障交易的成本效益与执行安全。\
​\
专为 **BONKfun** 交易环境打造，它能最大程度降低滑点损耗与链上机器人的干扰。结合自动化批处理引擎，它在免除人工换号操作的同时，极大提升了多钱包资产变现的效率，是 Web3 项目方和专业团队不可或缺的流动性管理利器。

***

## **技术实现示意**

### 传统交易

多个钱包的交易将分别广播并独立上链，无法保证执行顺序或进入同一区块。若其他交易抢先交易，币对价格可能提前下跌，导致后续钱包的成交价格降低、实际收到的资产减少。

<figure><img src="../../../.gitbook/assets/Frame 1321314899.png" alt=""><figcaption></figcaption></figure>

### 捆绑交易

将多达 20 个钱包中的指定代币归集至 1 个钱包，并由该钱包统一卖出。将代币转账与卖出交易打包在一个捆绑包内按预设顺序执行，减少交易间隙被其他交易插入的风险，提升批量买入的执行一致性，并提升交易优先级。

<figure><img src="../../../.gitbook/assets/Frame 1321314903.png" alt=""><figcaption></figcaption></figure>

***

## **图文指南**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角【连接钱包】按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (748).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择交易对

可以选择输入代币地址，也可以选择当前钱包拥有的代币进行交易操作。

* **价值代币：**&#x6267;行交易操作时，用以支付币对价格的代币地址
* **做市代币：**&#x6267;行交易操作时，用以实现市值管理策略目标的代币地址

<figure><img src="../../../.gitbook/assets/image (918).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入钱包私钥

{% hint style="danger" %}
请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

{% hint style="info" %}
<mark style="color:$primary;">**操作钱包设置**</mark>

导入钱包没有数量限制。服务费均由第一个地址支付，Jito 小费由每组导入的最后一个地址支付，调整导入的第一个和最后一个地址中有足够余额。
{% endhint %}

导入钱包数量没有限制，系统会根据钱包数量自动分组。支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入来源地址的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「批量输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (1) (1) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x6BCF;行仅输入一个钱包私钥，可在私钥后追加数量。

```
privateKey, 300
```

<figure><img src="../../../.gitbook/assets/image (737).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (4) (1) (1).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 下载 CiaoTool 模板文件，并将信息导入到文件内。

<figure><img src="../../../.gitbook/assets/image (2) (1) (1) (1).png" alt=""><figcaption></figcaption></figure>

2. 点击![](<../../../.gitbook/assets/image (848).png>)**「导入文件」**&#x6309;钮，弹出文件上传窗口。
3. 点&#x51FB;**「确定导入」**，将所有地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (3) (1) (1).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 发送设置

* **RPC 发送**\
  RPC 发送策略是尽力而为，无需支付 Jito 小费。通过统一交易广播交易，但不保证在同一区块内，可能会被机器人狙击造成损失。
* **Jito Bundle**\
  通过 Jito 小费，将交易打包为一个捆绑包，确保交易不被狙击，并提升上链优先级，但需要消耗更多费用。

<figure><img src="../../../.gitbook/assets/image (857).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 启动交易

{% hint style="info" %}
<mark style="color:$primary;">**捆绑包设置**</mark>

服务费均由第一个地址支付，Jito 小费由导入的每组最后一个地址支付，调整导入的第一个和最后一个地址中有足够余额。
{% endhint %}

确认信息无误后，点击下方「**捆绑卖出**」按钮，即可启动程序。

<figure><img src="../../../.gitbook/assets/image (5) (1).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

***

## **常见问题**

<details>

<summary><strong>什么是 Bonk 多地址捆绑卖出功能？</strong></summary>

多地址捆绑卖出是指通过多个钱包在同一区块内同步执行卖出操作。通过将多笔交易打包执行，可以减少时间差带来的价格波动，从而降低滑点并提升整体执行效率，适用于退出、止盈等关键交易阶段。

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
