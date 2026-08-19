---
description: >-
  通过自动化 Uniswap V2 和 V3 交易提升代币在 Robinhood Chain
  上的链上活跃度。利用多钱包执行、灵活的交易间隔和智能停止条件，持续保持市场活跃与项目曝光。
---

# Robinhood - 市值管理教程

{% hint style="info" %}
**CiaoTool Uniswap 市值管理**现已全面支持 **V2 / V3** 全部的流动性池类型，请先切换到指定池子功能页面进行市值管理操作，满足不同场景下的快捷做市服务。
{% endhint %}

## CiaoTool Robinhood 市值管理是什么？

<figure><picture><source srcset="../../../.gitbook/assets/ScreenShot_2026-07-22_173414_953.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (655).png" alt="CiaoTool Robinhood链 Uniswap V2 市值管理页面"></picture><figcaption></figcaption></figure>

CiaoTool Robinhood Chain 市值管理是一款面向 Uniswap V2 和 V3 流动性池的自动化交易工具。

用户可以导入多个由自己控制的交易钱包，并根据预先设置的交易金额、执行间隔、交易优先级和停止条件，自动执行买入或卖出交易。

相比逐个切换钱包、输入金额并确认交易，CiaoTool 可以通过一个页面统一配置、执行和管理多钱包交易任务，减少重复操作，让自动化策略更容易设置、监控和停止。

在本教程中，“市值管理”指按照用户设置执行自动化交易，并不代表 CiaoTool 代替用户托管资金、直接提供流动性，或保证价格稳定、交易量和投资收益。

### 常见用例

<table data-view="cards"><thead><tr><th></th><th></th></tr></thead><tbody><tr><td><strong>维持市场活跃度</strong></td><td>通过多个钱包持续循环执行买入和卖出，让代币在一段时间内保持稳定的链上交易活跃度。</td></tr><tr><td><strong>增强买盘活跃度</strong></td><td>根据设定的金额、钱包和执行频率运行买入策略，增加买盘参与度并支持积极的市场动能。</td></tr><tr><td><strong>平滑卖盘执行</strong></td><td>将卖出交易分散到不同时间和钱包执行，降低集中卖出可能产生的市场冲击。</td></tr><tr><td><strong>提升代币市场可见度</strong></td><td>通过持续、稳定的交易活动增强代币的链上表现，提高项目在市场参与者中的可见度。</td></tr><tr><td><strong>自动化策略控制</strong></td><td>统一管理交易金额、执行频率、交易速度和买卖方向，并通过执行次数或价格范围条件自动停止策略。</td></tr></tbody></table>

### 快速使用

立即在 Robinhood 链上，用 CiaoTool 进行市值管理操作：

{% embed url="https://robinhood.ciaotool.io/zh-Hans/swap/v2/market-making-manage-v2" %}

{% embed url="https://robinhood.ciaotool.io/zh-Hans/swap/v3/market-making-manage-v3" %}

***

## 为什么选择 CiaoTool Robinhood 市值管理？

CiaoTool 通过持续、灵活配置的买卖策略，帮助项目团队提升代币在 Robinhood Chain 上的链上活跃度和市场可见度，支持 Uniswap V2 和 V3 流动性池。

用户无需频繁切换钱包并手动提交每一笔交易，即可通过一个页面管理最多 20 个交易钱包。任务开始前，可以统一配置交易金额、执行间隔、交易优先设置和停止条件。

凭借多钱包自动化、本地浏览器安全签名、灵活的交易金额模式、随机执行间隔和自动停止控制，CiaoTool 让持续做市策略的配置、执行和管理更加高效、安全且可控。

***

## **视频教程**

{% embed url="https://www.youtube.com/watch?t=4s&v=iM4stNNHWro" %}

***

## **分步式教程**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 Robinhood 链的钱包

<figure><img src="../../../.gitbook/assets/image (656).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入做市代币地址

{% hint style="info" %}
V2 / V3 功能页面略有不同，点击下方按钮切换并显示 V2 / V3 教程。
{% endhint %}

{% tabs %}
{% tab title="V2" %}
可以选择输入代币地址，也可以选择当前钱包拥有的代币进行买入操作。\
点击中间箭头可快速切换兑换目标。

<figure><img src="../../../.gitbook/assets/image (657).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="V3" %}
不同于 V2 流动性池，每个不同币对和税费的 V3 流动性池有专属的币对地址，请输入正确的币对地址以选择兑换币对。

点击中间箭头可快速切换兑换目标。

<figure><img src="../../../.gitbook/assets/image (658).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入支付钱包私钥

将用于支付市值操作手续费的钱包私钥导入。

<figure><img src="../../../.gitbook/assets/image (551).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入交易钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

**「批量交易」**&#x529F;能多地址导入仅支持 私钥导入以进行兑换操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入交易地址私钥的类型。最多支持 20 个地址。

1. 点&#x51FB;**「导入私钥」**&#x6309;钮，弹出输入框。

<figure><img src="../../../.gitbook/assets/image (659).png" alt=""><figcaption></figcaption></figure>

2. 手动输入或导入私钥文件，确认框中显示私钥后点击确认。

<figure><img src="../../../.gitbook/assets/image (660).png" alt=""><figcaption></figcaption></figure>

使用 CiaoTool 模板文件导入，并保存确定导入并显示在输入框内。\
点击下载并查看模板：

{% file src="../../../.gitbook/assets/EVM_privateKey_demo.xlsx" %}
{% endstep %}

{% step %}
### 输入买入金额

支&#x6301;**「固定数量」「固定留存」「全部数量」三**种交易金额类型。

<figure><img src="../../../.gitbook/assets/image (661).png" alt=""><figcaption></figcaption></figure>

1. **固定数量**\
   所有钱包根据同一数量将代币全部兑换为指定代币。
2. **固定留存**\
   所有钱包留存指定数量代币，其余全部兑换为指定代币。
3. **全部数量**\
   所有钱包将把价值代币全部兑换为指定代币。
{% endstep %}

{% step %}
### 交易参数设置

{% hint style="danger" %}
关闭 / 刷新页面，机器人策略亦会**立即停止**。请保持策略执行期间，将网页持续处于后台并运行状态。为保证策略执行之必要，**该功能不推荐于**「**移动电子设备**」**使用。**
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (662).png" alt=""><figcaption></figcaption></figure>

**停止方式：**

* **运行次数：**&#x5F53;导入钱包执行循环到指定阈值时，市值管理机器人随即停止。
* 价格范围：当做市代币价格超出指定范围时，市值管理机器人随即停止。

**交易间隔：**&#x6307;各钱包买入 / 卖出的执行间隔，通过随机时间范围，模拟真实交易。
{% endstep %}

{% step %}
### 确认交易

提交任务前，请仔细核对所有参数。页面会在执行前显示所有适用费用。

确认信息无误后，点击下&#x65B9;**「开始交易」**&#x6309;钮，并等交易程序完成。

<figure><img src="../../../.gitbook/assets/image (663).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>CiaoTool 支持 Robinhood Chain 上的哪些 Uniswap 池子？</strong></summary>

CiaoTool 支持 Robinhood Chain 上符合条件的 Uniswap V2 和 V3 流动性池。V2 和 V3 的池子选择方式不同，请在开始任务前选择与目标池子相对应的页面。

</details>

<details>

<summary><strong>V2 和 V3 市值管理工具有什么区别？</strong></summary>

在 V2 页面中，用户通常需要选择交易代币以及对应的 V2 交易对。

在 V3 页面中，用户需要输入准确的币对地址。因为同一个代币交易对可能存在多个不同手续费等级的 V3 池子，每个 V3 池子都有独立的合约地址。

</details>

<details>

<summary><strong>如何查找正确的 Uniswap V3 币对地址？</strong></summary>

可以通过 Uniswap 官方页面或 Robinhood Chain 区块浏览器查找对应的 V3 池子。

继续操作前，请核对两个代币的合约地址、池子手续费等级，以及 CiaoTool 页面显示的币对地址。

</details>

<details>

<summary><strong>最多可以导入多少个交易钱包？</strong></summary>

CiaoTool 目前支持在单个任务中通过手动输入或兼容的私钥文件导入最多 20 个交易钱包。

</details>

<details>

<summary><strong>为什么需要付款钱包和交易钱包？</strong></summary>

付款钱包用于支付适用的 CiaoTool 服务费。

交易钱包用于执行交易。每个交易钱包需要持有相应的交易资产，并保留足够的 ETH 用于支付 Robinhood Chain 网络 Gas 费用。

</details>

<details>

<summary><strong>操作是否安全？</strong></summary>

平台采用纯前端签名机制，您的私钥绝不会被上传或储存在任何服务器上，所有交易均在本地浏览器完成签名，从技术层面确保平台无法访问您的私钥。

</details>

<details>

<summary><strong>关闭或刷新页面后会发生什么？</strong></summary>

自动化任务运行在当前浏览器页面中。关闭或刷新页面后，CiaoTool 将停止安排新的交易。

但是，已经提交到 Robinhood Chain 的交易仍可能继续确认。关闭页面不会撤销已确认的交易，也不能保证取消处于待交易状态的交易。

</details>

<details>

<summary><strong>自动停止条件如何工作？</strong></summary>

CiaoTool 支持根据指定执行次数或价格范围停止新的任务执行。

检测到停止条件后，机器人将不再安排新的交易，但不会撤销已经提交或确认的交易。

</details>

***

## **联系我们**

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
