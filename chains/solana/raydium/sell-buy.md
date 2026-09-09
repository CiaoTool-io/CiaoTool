---
description: >-
  专为 Raydium 打造的高效交易换仓工具，通过同区块聚合执行卖出与多钱包买入，模拟真实盘口交易形式让换仓行为更自然。在有效降低 MEV
  夹击风险与资金损耗的同时，安全优化链上资产轨迹。
---

# Solana - 卖出并多地址捆绑买入教程

{% hint style="info" %}
**CiaoTool Raydium 卖出并多地址捆绑买入**现已全面支持 **AMM V4、CLMM、CPMM** 全部的流动性池类型，请先切换到指定池子功能页面进行多地址捆绑买卖操作，满足不同场景下的快捷交易服务。
{% endhint %}

## CiaoTool Solana 卖出并多地址捆绑买入是什么？

<figure><picture><source srcset="../../../.gitbook/assets/屏幕截图 2026-09-08 153455.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (6) (1).png" alt="CiaoTool Solana Chain Raydium 卖出并捆绑买入页面"></picture><figcaption></figcaption></figure>

**CiaoTool Solana 卖出并多地址捆绑买入**是一款专注于交易连贯性与链上流动性管理的高阶工具。它允许您通过底层智能聚合技术，在同一个区块内，自动让指定钱包完成 Raydium 上的代币卖出操作，并同步触发多个独立钱包的批量买入行为。

相较于传统的分步手动交易或直接批量转账，该功能的核心优势在于以真实的盘口交易形式让换仓行为更自然。系统将买卖双向交易聚合于同一区块执行，不仅最大程度减少了交易被 MEV 机器人“夹击”的风险与资金磨损，更免去了您在繁琐流程中频繁切换钱包地址的操作麻烦。这能在成倍节省运营时间的同时，帮助团队安全、稳健地优化代币的持币者分布，是执行进阶做市与流动性平移策略的关键利器。

此工具尤其适用于：

* 专业做市的流动性平移与资产安全重组
* 以真实盘口买卖取代直接转账，让筹码转移轨迹更符合市场自然逻辑
* 降低买卖双向交易时的滑点损耗与 MEV 夹击风险
* 免除频繁切换钱包的繁琐操作，大幅节省团队运营时间
* 安全、稳健地促进代币地址的健康分布与链上数据优化

立即在 Solana 上，用 CiaoTool 通过卖出并多地址捆绑买入进行交易换仓操作：

{% embed url="https://ciaotool.io/zh-Hans/raydium/sell-buy" %}

***

## 为什么选择 CiaoTool Solana 卖出并捆绑买入？

CiaoTool 为 Solana 链上的资产调拨与流动性重组提供了一种兼顾安全与低损耗的专业“交易换仓”方案。相较于容易被追踪的直接批量转账，该功能通过同区块智能聚合技术，将筹码转移巧妙转化为真实的盘口买卖，让多钱包的换仓行为更自然、更符合市场逻辑，有效优化链上数据的聚类呈现。\
​\
买卖双向交易的无缝衔接，不仅大幅降低了 Solana 网络中的滑点损耗与 MEV 机器人的夹击风险，更免去了您在繁琐流程中频繁切换钱包地址的操作麻烦。在成倍节省运营时间的同时，为 Web3 项目方与专业团队构建了一道坚实的流动性安全防线。

***

## **技术实现示意**

### 传统交易

多个钱包的交易将分别广播并独立上链，无法保证执行顺序或进入同一区块。若其他交易抢先交易，币对价格可能波动，导致后续买入钱包的成本上升、实际获得的代币数量减少。

<figure><img src="../../../.gitbook/assets/Frame 1321314904.png" alt=""><figcaption></figcaption></figure>

### 捆绑交易

将卖出钱包钱包和多地址买入钱包的交易将按预设顺序打包到一个 Bundle 捆绑包内提交，并在同一区块内连续执行，减少交易间隙被其他交易插入的风险，提升批量买入的执行一致性，并提升交易优先级。

<figure><img src="../../../.gitbook/assets/Frame 1321314905 (1).png" alt=""><figcaption></figcaption></figure>

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
### 卖出钱包

{% hint style="danger" %}
请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

输入卖出钱包的私钥地址，及卖出目标代币数量。
{% endstep %}

{% step %}
### 买入钱包

{% hint style="danger" %}
请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

{% hint style="info" %}
<mark style="color:$primary;">**操作钱包设置**</mark>

**Raydium 卖出并捆绑买入**导入钱包没有数量限制。服务费均由第一个地址支付，Jito 小费由每组导入的最后一个地址支付，调整导入的第一个和最后一个地址中有足够余额。
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
### 发送设置

* **RPC 发送**\
  RPC 只能保证首笔卖出与第一个买入同笔原子，无需支付 Jito 小费。通过统一交易广播交易，但不保证在同一区块内，可能会被机器人狙击造成损失。
* **Jito Bundle**\
  通过 Jito 小费，将交易打包为一个捆绑包，确保交易不被狙击，并提升上链优先级，但需要消耗更多费用。

<figure><img src="../../../.gitbook/assets/image (857).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 核实信息

程序自动运行，查看确认页面并核对：

* [x] 买入钱包数量、买入本金、预计买回
* [x] 卖出本金、卖出到账

<figure><img src="../../../.gitbook/assets/image (907).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 启动交易

{% hint style="info" %}
<mark style="color:$primary;">**捆绑包设置**</mark>

服务费均由第一个地址支付，Jito 小费由导入的每组最后一个地址支付，调整导入的第一个和最后一个地址中有足够余额。
{% endhint %}

确认信息无误后，点击下&#x65B9;**「卖出并捆绑买入」**&#x6309;钮，即可启动程序。

<figure><img src="/broken/files/MWjoASSIXidRqCTkvVAD" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

***

## **常见问题**

<details>

<summary><strong>什么是 Solana 卖出并捆绑买入功能？</strong></summary>

这是 CiaoTool 专为 Raydium 平台打造的高阶「交易换仓」工具。它允许用户在同一个区块内，无缝衔接指定钱包的代币卖出操作与多个子钱包的批量买入行为。透过同区块智能聚合技术，将资产的跨钱包平移巧妙转化为真实的盘口买卖交互。

</details>

<details>

<summary><strong>该功能与「冷换仓」有什么区别？</strong></summary>

两者的核心区别在于资产迁移的链上行为形式不同，分别适用于不同的营运场景：

**冷换仓**（纯转帐形式）：纯粹透过链上转帐将代币从源钱包打散分发到多个新地址，绝不涉及任何盘口交易。其优点是完全不影响市场价格，适合悄无声息地隐匿分仓。

**卖出并捆绑买入**（交易换仓形式）：筹码转移不通过直接转帐，而是通过盘口卖出 & 多钱包同步买入的真实交易来完成。它会在链上留下正常的市场买卖轨迹，让多钱包的换仓行为显得更加真实自然，完美切断了钱包之间的直接转帐关联。

</details>

<details>

<summary><strong>交易换仓会对代币的市场数据产生什么影响？</strong></summary>

由于整个换仓过程是通过在 Raydium 盘口进行真实的买卖交互完成的，因此它在自然完成资产平移的同时，还会为代币贡献真实的交易笔数与盘口活跃度，并安全、稳健地优化代币的持币者分布与独立交易地址结构。

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
