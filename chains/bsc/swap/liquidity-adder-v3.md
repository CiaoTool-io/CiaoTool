---
description: >-
  CiaoTool 提供免代码的 PancakeSwap V3
  添加流动性池工具。深度适配集中流动性（CLMM）机制，支持智能判定并增加单边流动性。纯前端本地处理机制，助您高效管理 BSC 链上做市资金。
---

# BSC - 添加 V3 流动性教程

{% hint style="info" %}
当前&#x662F;**「PancakeSwap 添加 V3 流动性」**&#x6559;程页面，以添加「集中流动性、自定义流动区间」的 V3 流动性池，增加池子深度。

想添加具有「易用、全区间覆盖」的 V2 流动性池，请查阅[**「PancakeSwap 添加 V2 流动性」**](liquidity-adder-v2.md)**。**
{% endhint %}

## PancakeSwap 添加 V3 流动性是什么？

<figure><img src="../../../.gitbook/assets/image (583).png" alt=""><figcaption></figcaption></figure>

**PancakeSwap V3 添加流动性**是指在已部署的 V3 资金池中追加做市资金的操作。V3 协议采用了“集中流动性”机制，要求做市商在添加资金时设定特定的价格区间。

核心适用场景：

* 动态市值维护： 随着代币价格的波动，项目方需要不断调整并追加流动性，以确保当前市场价格附近有足够的交易深度。
* 单边做市与托盘： 当项目方希望在特定低价区建立极强的防守买盘，或在高价区布置压制卖盘时，可利用 V3 的单边特性进行精准资金投放。

立即在 BSC 上，用 CiaoTool​ 添加流动性池功能进行增加池子深度操作：

{% embed url="https://bsc.ciaotool.io/zh-Hans/swap/v3/add-liquidity-v3" %}

***

## 为什么选择 CiaoTool 添加 V3 流动性？

对于需要严密掌控筹码分布的专业团队，CiaoTool 构筑了极致安全与高效的基础设施：

* **零代码高效部署：**\
  将复杂的 V3 价格区间计算与合约交互，转化为直观的 Web 端可视化操作，任何人都能无门槛使用。
* **纯前端私钥隔离：**\
  平台严格采用客户端本地处理机制。您的钱包私钥仅在本地浏览器中用于交易签名，绝不上传、存储或传输至任何云端服务器，从技术底层切断资金风险。
* **端到端的生态闭环：**\
  CiaoTool 定位为全栈式代币生命周期管理平台。开盘建仓完成后，您可以无缝联动「市值管理」、「批量交易」等工具，一站式打造繁荣的链上数据表现。

***

## **图文指南 |** PancakeSwap 创建 V3 流动性

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 BSC 链的钱包

<figure><img src="../../../.gitbook/assets/image (446).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入添加流动性钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

当&#x524D;**「添加流动性」**&#x529F;能仅支持 私钥导入以进行加池操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

该钱包地址将用于支付工具手续费，并拥有池子权限。

<figure><img src="../../../.gitbook/assets/image (569).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入币对地址

每个不同币对 / 不同税率的 V3 流动性池都有独立的币对地址。将币对地址输入到框内，系统将自动显示币对信息。

<figure><img src="../../../.gitbook/assets/image (584).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 设置流动性价格区间

<figure><img src="../../../.gitbook/assets/image (585).png" alt=""><figcaption></figcaption></figure>

1. 区间大小決定收益高低 (LP 手续费收益、CAKE 收益皆适用)

* 越窄收益越高，无常损失越大；
* 越宽收益越低，无常损失越小；
* 全区间设置则类似于 V2 运作，收益将非常少。

2. 超出区间时

* V3 池无收益；
* 流动性仓位将变为单币；
* 可以移除流动性并重新添加，或是等待价格重新回到区间内。
* 可以添加 V2 流动性池，确保 V3 区间外基础流动性。

3. 单边添加

* 对 Uniswap / Pancake V3 来说，纯单边只在“当前价格落在所设价格区间外”时成立；
* 当前价低于最低价时只能单边添加 WBNB，当前价高于最高价时只能单边添加 USDT。全区间模式下，当前价天然在区间内，所以纯单边不成立。
{% endstep %}

{% step %}
### 输入加池代币数量

<figure><img src="../../../.gitbook/assets/image (586).png" alt=""><figcaption></figcaption></figure>

系统将根据当前币对价格，以及添加流动性的价格范围，自动计算出 价值代币 / 项目代币的加池数量。

您可以自由输入加池代币数量，以显示加池币对数量情况。
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下&#x65B9;**「开始交易」**&#x6309;钮，并等待开盘完成。
{% endstep %}
{% endstepper %}

***

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
