---
description: >-
  专为 Pump.fun
  平台已发行的代币打造的狙击工具。支持在代币发行后的任意阶段，将“多钱包买满内盘联合曲线”与“流动性迁移外盘时的首笔狙击”聚合在同一区块内执行，实现内盘毕业到外盘开盘的无缝筹码锁定。
---

# PumpFun - 捆绑并迁移买入教程

{% hint style="info" %}
**CiaoTool PumpFun 捆绑并迁移买入**现已全面支持官方 **SOL** 和 **USDC** 全部的价值代币
{% endhint %}

## 功能介绍

CiaoTool PumpFun 捆绑并迁移买入是一款面向**已在 Pump.fun 上线、尚未完成迁移**的代币自动化工具，无需重新创建代币。

系统计算 Bonding Curve 的剩余进度，并将以下操作按顺序组成 Bundle：

1. **内盘捆绑买入：** 由多个钱包买入剩余额度，推动代币达到平台迁移条件。
2. **迁移与外盘买入：** 完成流动性迁移后，由指定钱包在 PumpSwap 执行买入。

正常执行时，Bundle 内的交易将在同一区块按预设顺序完成；任一关键交易失败，整个 Bundle 不执行。

立即在 PumpFun 上，用 CiaoTool​ 捆绑并迁移买入功能进行一键开盘操作：

{% embed url="https://ciaotool.io/zh-Hans/pump/bundled-graduate" %}

***

## 核心优势

* **支持已上线代币：** 适用于尚处于 Bonding Curve 阶段的兼容代币
* **自动计算额度：** 根据实时链上状态估算达到迁移条件所需的买入金额
* **多钱包执行：** 支持配置多个内盘买入钱包及对应金额
* **迁移流程衔接：** 将内盘买入、流动性迁移与外盘买入按顺序打包
* **提升上链机会：** 通过 Jito 小费提高 Bundle 的上链优先级
* **本地签名：** 交易在浏览器本地完成签名，私钥无需上传

***

## **技术实现示意**

### 传统发射代币

{% columns %}
{% column %}
多地址买入、迁移至 DEX 以及迁移后的买入交易分别广播、独立上链，无法保证执行顺序或进入相邻区块。

执行期间若有其他交易插入，可能改变代币价格，导致后续钱包的买入成本和实际获得数量发生变化。

在迁移时，极容易被机器人狙击抢跑，实际获得的代币数量减少，造成损失。
{% endcolumn %}

{% column %}
<figure><img src="../../../.gitbook/assets/Frame 1321314910.png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}
{% endcolumns %}

### 捆绑发射代币

{% columns %}
{% column %}
整体流程分为两个捆绑执行：

* **发射阶段**：将 8 个钱包的买入交易打包，按预设顺序在同一区块内连续执行，直接打满联合曲线，使代币进入迁移程序。
* **迁移阶段**：将迁移至 DEX 与指定钱包的买入交易再次打包，按预设顺序在同一区块内执行。

完美减少交易间隙及迁移过程中被其他交易插入的风险，提升发射与买入的执行一致性及上链优先级，提升利润空间。
{% endcolumn %}

{% column %}
<figure><img src="../../../.gitbook/assets/Frame 1321314911.png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}
{% endcolumns %}

***

***

## **图文指南**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角【连接钱包】按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (748).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 内盘钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入接收地址的类型，选择以查看详细教程。最多支持 **8 个地址**在联合曲线阶段捆绑买入。

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

<figure><img src="../../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 下载 CiaoTool 模板文件，并将信息导入到文件内。

<figure><img src="../../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

2. 点击![](<../../../.gitbook/assets/image (848).png>)**「导入文件」**&#x6309;钮，弹出文件上传窗口。
3. 点&#x51FB;**「确定导入」**，将所有地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入交易金额

支&#x6301;**「逐一输入」「输入金额」**&#x4E24;种交易金额类型。系统会实时获取当前联合曲线状态并计算打满所需数量，开发者钱包买入 + 捆绑钱包买入代币数量必须超过显示数。

<figure><img src="../../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

1. **逐一输入**\
   在输入框中，逐一输入交易金额数量。
2. **统一金额**\
   点击交易数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「输入金额」**&#x9009;项，所有地址将统一交易数量。
{% endstep %}

{% step %}
### 迁移狙击钱包

当代币迁移至外盘 PumpSwap 时，同步狙击的钱包私钥，获得底部筹码的同时活跃代币。

外盘买入数量没有限制。

<figure><img src="../../../.gitbook/assets/image (932).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Jito 小费设置

{% hint style="danger" %}
此功能实现依赖于 Jito 的捆绑功能。由于网络环境、Jito节点、RPC节点和区块处理引擎的复杂影响，该功能可能面临较高的失败率。

若操作失败，不会开盘成功也不会产生任何费用，请尝试更换RPC节点，区块处理引擎，增加Jito的小费(建议0.01SOL)，并考虑在链上活跃度较低的时段再次尝试。
{% endhint %}

通过 Jito 小费，将创建代币+多地址交易打包为一个捆绑包，确保交易不被狙击，并提升上链优先级，但需要消耗更多费用。

<figure><img src="../../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下&#x65B9;**「创建并买入」**&#x6309;钮，并等待开盘完成。
{% endstep %}
{% endstepper %}

## **常见失败案例**

* 若因 Jito 小费低于市场均值或遭机器人抢跑导致失败，请适当提高 Jito 小费并重试。
* 若因 RPC 节点或区块引擎响应延迟导致错失打包时机，请切换至其他更稳定的节点。
* 若因主钱包余额不足以支付建币费与租金等隐藏消耗，请确保额外预留至少 0.05 SOL 的缓冲资金。
* 若遇 Solana 链上极度壅塞引发底层随机丢包，请直接避开交易尖峰时段，稍后再试。

***

## **常见问题**

<details>

<summary><strong>“捆绑并迁移买入”与“创建并迁移买入”有什么本质区别？</strong></summary>

“创建并迁移买入”包含了代币的初始链上部署；而“捆绑并迁移买入”不包含发币操作，它专门服务于已经上线内盘且正在交易中的代币，允许项目方在开盘后的任意窗口期介入，为其提供后续的打满内盘与跨盘狙击服务。

</details>

<details>

<summary><strong>如果我的 Pump 代币不是通过 CiaoTool 发射的，还能使用这个功能吗？</strong></summary>

可以。只要目标代币当前仍处于 Pump.fun 的内盘流转阶段，无论其最初通过何种平台或代码部署，您都可以随时调用该功能执行同区块的捆绑买入与外盘狙击操作。

</details>

<details>

<summary><strong>打满内盘所需的资金是如何计算和分配的？</strong></summary>

系统会实时读取当前代币联合曲线的剩余进度。确保您导入的多捆绑买入钱包只需确保拥有充足的 SOL 余额（涵盖购买本金、预估滑点），以完成内盘捆绑买入指令。

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
