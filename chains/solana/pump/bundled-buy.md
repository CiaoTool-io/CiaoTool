---
description: >-
  专为 Pump.fun 和 PumpSwap
  打造的高效批量买入工具，通过在同一区块内同步执行多钱包买入操作，帮助您安全优化持币分布，提升多钱包资产配置效率，是专业流动性管理的进阶利器。
---

# Pump - 多地址捆绑买入教程

{% hint style="info" %}
**CiaoTool Pump 多地址捆绑买入**现已全面支持官方 **SOL** 和 **USDC** 全部的价值代币，输入代币地址将自动切换池子适配和价值代币。
{% endhint %}

## CiaoTool Pump 多地址捆绑买入是什么？

<figure><picture><source srcset="../../../.gitbook/assets/屏幕截图 2026-09-08 175501.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (901).png" alt="CiaoTool Solana Chain Pump 多地址捆绑买入页面"></picture><figcaption></figcaption></figure>

**CiaoTool Pump 多地址捆绑买入**是一款专注于交易执行优化与链上流动性管理的高阶工具。它允许您通过底层智能聚合技术，在同一个区块内，自动让多个独立钱包同步完成 **Pump.fun** 和 **PumpSwap 平台**上的代币批量买入操作。

相较于传统的分批手动交易，多地址捆绑买入的核心优势在于有效防止 MEV 机器人的干扰与资金损耗。系统将多笔交易聚合于同一区块执行，最大程度减少交易“被夹”的风险，保障交易的成本效益。这不仅能显著提升批量买入的执行效率，更能帮助团队安全、稳健地优化代币的持币者分布，是执行进阶做市与流动性策略的关键利器。

此工具尤其适用于：

* 专业做市的初期建仓与流动性布局
* 降低多钱包批量买入时的滑点与 MEV 夹击风险
* 安全、稳健地促进代币地址的健康分布
* 提升多地址链上资产配置与资金调拨的整体效率

立即在 Pump.fun 和 PumpSwap 平台上，用 CiaoTool 进行多地址捆绑买入操作：

{% embed url="https://ciaotool.io/zh-Hans/pump/multi-address-buy" %}

***

## 为什么选择 CiaoTool Pump 多地址捆绑买入？

**CiaoTool** 为 **Pump.fun** 和 **PumpSwap 平台**上的资产建仓与流动性管理提供了一种兼顾效率与成本保护的专业方案。无论您是执行专业做市的初期建仓、规避 MEV 夹击的批量买入交易，还是稳健地促进代币持币者分布，其多地址捆绑买入功能都能通过同区块智能聚合技术，免去您在繁琐流程中频繁更换钱包地址的操作麻烦，成倍节省宝贵的运营时间，全方位保障交易的成本效益与执行安全。\
​\
专为 Pump.fun 和 PumpSwap 交易环境打造，它能最大程度降低滑点损耗与链上机器人的干扰。结合自动化批处理引擎，它在免除人工换号操作的同时，极大提升了多钱包资产配置与建仓的效率，是 Web3 项目方和专业团队不可或缺的流动性管理利器。

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
### 选择交易代币

可以选择输入代币地址，也可以选择当前钱包拥有的代币进行交易。系统将自动识别锚定价值代币并匹配所在池位置。

<figure><img src="../../../.gitbook/assets/image (896).png" alt=""><figcaption></figcaption></figure>
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

<figure><img src="../../../.gitbook/assets/image (902).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 启动交易

{% hint style="info" %}
<mark style="color:$primary;">**捆绑包设置**</mark>

服务费均由每组第一个地址支付，Jito 小费由导入的最后一个地址支付，调整导入的第一个和最后一个地址中有足够余额。
{% endhint %}

确认信息无误后，点击下方「**确认并开始捆绑买入**」按钮，即可买入程序。

<figure><img src="../../../.gitbook/assets/image (892).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

***

## **常见问题**

<details>

<summary><strong>什么是 Pump 多地址捆绑买入功能？</strong></summary>

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
