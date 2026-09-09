---
description: >-
  专为 Bonk.fun
  打造的高效批量买入工具，通过在同一区块内同步执行多钱包买入操作，帮助您安全优化持币分布，提升多钱包资产配置效率，是专业流动性管理的进阶利器。
---

# Bonk - 多地址捆绑买入教程

{% hint style="info" %}
**CiaoTool Bonk 多地址捆绑买入**现已全面支持官方 **SOL** 和 **USD1** 全部的价值代币，输入代币地址并切换价值代币。
{% endhint %}

## CiaoTool Bonk 多地址捆绑买入是什么？

## 功能介绍

CiaoTool Bonk 多地址捆绑买入是一款面向 Bonk.fun 的多钱包交易工具。用户可配置多个钱包及买入金额，系统自动构建交易并通过 Bundle 按预设顺序提交。

正常执行时，包内交易将在同一区块连续完成，减少多笔交易之间被其他交易插入的风险，提升批量买入的执行一致性。

**适用场景：**

* 多钱包批量买入与资产配置
* 项目金库及运营钱包建仓
* 自动化交易与流动性策略执行

立即在 Bonk 上，用 CiaoTool 进行多地址捆绑买入操作：

{% embed url="https://ciaotool.io/zh-Hans/bonk/multi-address-buy" %}

***

## 核心优势

* **多钱包配置：** 支持分别设置买入钱包及交易金额
* **同区块执行：** Bundle 上链后，包内交易按预设顺序连续执行
* **减少交易间隙：** 降低批量操作期间被其他交易插入的风险
* **自动分组：** 根据交易数量自动构建并提交 Bundle
* **提升上链机会：** 通过 Jito 小费提高 Bundle 的上链优先级
* **本地签名：** 交易在浏览器本地完成签名，私钥无需上传

***

## **技术实现示意**

### 传统交易

多个钱包的交易将分别广播并独立上链，无法保证执行顺序或进入同一区块。期间若有其他交易抢先成交，池内价格可能发生变化，导致后续钱包的买入成本上升、实际获得的代币数量减少，造成损失。

<figure><img src="../../../.gitbook/assets/Frame 1321314899.png" alt=""><figcaption></figcaption></figure>

### 捆绑交易

将 10 个钱包的交易将按预设顺序打包到一个 Bundle 捆绑包内提交，并在同一区块内连续执行，减少交易间隙被其他交易插入的风险，提升批量买入的执行一致性，并提升交易优先级。

<figure><img src="../../../.gitbook/assets/Frame 1321314903 (1).png" alt=""><figcaption></figcaption></figure>

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

导入钱包没有数量限制。服务费均由每组第一个地址支付，Jito 小费由导入的最后一个地址支付，调整导入的第一个和最后一个地址中有足够余额。
{% endhint %}

导入钱包数量没有限制，系统会根据钱包数量自动分组。支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入来源地址的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「批量输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (887).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x6BCF;行仅输入一个钱包私钥，可在私钥后追加数量。

```
privateKey, 300
```

<figure><img src="../../../.gitbook/assets/image (737).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (890).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 下载 CiaoTool 模板文件，并将信息导入到文件内。

<figure><img src="../../../.gitbook/assets/image (888).png" alt=""><figcaption></figcaption></figure>

2. 点击![](<../../../.gitbook/assets/image (848).png>)**「导入文件」**&#x6309;钮，弹出文件上传窗口。
3. 点&#x51FB;**「确定导入」**，将所有地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (889).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入交易金额

支&#x6301;**「逐一输入」「输入金额」「随机范围」「保留金额」「百分比金额」**&#x548C;**「全部」**&#x516D;种交易金额类型。

<figure><img src="../../../.gitbook/assets/image (893).png" alt=""><figcaption></figcaption></figure>

1. **逐一输入**\
   在输入框中，逐一输入交易金额数量。

<figure><img src="../../../.gitbook/assets/image (894).png" alt=""><figcaption></figcaption></figure>

2. **统一金额**\
   点击交易数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「输入金额」**&#x9009;项，所有地址将统一交易数量。
3. **随机范围**\
   点击交易数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「随机范围」**&#x9009;项，输入金额范围，所有地址将交易指定范围内数额。
4. **保留金额**\
   点击交易数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「保留金额」**&#x9009;项，所有钱包保留指定数量的目标代币，并将剩余代币全部交易。
5. **保留金额**\
   点击交易数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「百分比金额」**&#x9009;项，所有钱包保留指定百分比的目标代币，并将剩余代币全部交易。
6. **全部**\
   点击交易数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「全部」**&#x9009;项，所有钱包将目标代币全部交易。
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
### 核实信息

程序自动运行，查看确认页面并核对：

* [x] 交易钱包数量
* [x] 协议费消耗
* [x] 交易本金

<figure><img src="../../../.gitbook/assets/image (3) (1).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 启动交易

{% hint style="info" %}
<mark style="color:$primary;">**捆绑包设置**</mark>

服务费均由每组第一个地址支付，Jito 小费由导入的最后一个地址支付，调整导入的第一个和最后一个地址中有足够余额。
{% endhint %}

确认信息无误后，点击下方「**开始 BonkFun 捆绑买入**」按钮，即可买入程序。

<figure><img src="../../../.gitbook/assets/image (892).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>什么是 Bonk 多地址捆绑买入功能？</strong></summary>

多地址捆绑买入是指通过多个钱包在同一区块内同步执行买入操作。通过将多笔交易打包执行，可以减少时间差带来的价格波动，从而降低滑点并提升整体执行效率，适用于开盘、建仓等关键交易阶段。

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
