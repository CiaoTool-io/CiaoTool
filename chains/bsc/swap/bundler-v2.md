---
description: 在 BSC 链上实现同一区块内的自动建池与极速建仓，彻底规避 MEV 夹子攻击。纯前端本地签名，助您安全、高效启动 Web3 代币交易生态。
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/b56FKZGe1viFi67H1pPQ/swap/create-liquidity-and-buy-v2
---

# BSC - 创建 V2 流动性池并捆绑买入教程

{% hint style="info" %}
当前&#x662F;**「PancakeSwap 创建 V2 流动性池并捆绑买入」**&#x6559;程页面，以创建「易用、全区间覆盖」的 V2 流动性池。

想创建具有「集中流动性、自定义流动区间」的流动性池，请查阅[**「PancakeSwap 创建 V3 流动性池并捆绑买入」**](bundler-v3.md)**。**
{% endhint %}

## PancakeSwap 创建 V2 流动性池并捆绑买入是什么？

<figure><img src="../../../.gitbook/assets/image (568).png" alt="CiaoTool BSC链 创建 V2 流动性资金池并捆绑买入 页面"><figcaption></figcaption></figure>

**PancakeSwap V2 流动性池** 是基于 BNB 链（BSC）上最经典的 AMM 机制的去中心化交易基础。它通过 `x * y = k` 的恒定乘积公式，为代币提供初始的交易定价与买卖深度。

**创建流动性池并捆绑买入**则是 CiaoTool 为项目量身打造的高阶开盘策略。在传统的开盘流程中，项目方手动添加流动性后，极易被埋伏在链上的 MEV 机器人在同一区块内抢先买入（俗称“抢首矿”或“夹子攻击”），导致项目方或真实用户被迫在高位接盘。CiaoTool 通过底层智能合约聚合指令，将「创建 V2 流动性池」与「初始资金买入建仓」打包在同一个区块链交易中执行。

**核心适用场景：**

* 代币安全首发： 确保项目团队或早期核心支持者能够以绝对的初始底价获取筹码，建立安全的底部共识。
* Meme 币冷启动： 针对极易引发机器人抢跑的 Meme 币，提供最高级别的防夹保护。
* 流动性极速部署： 缩短开盘繁琐步骤，提升资产在去中心化交易所的上线效率。

立即在 BSC 上，用 CiaoTool​ 创建并买入功能进行一键开盘操作：

{% embed url="https://bsc.ciaotool.io/zh-Hans/swap/v2/create-liquidity-and-buy-v2" %}

***

## 如何选择 V2 / V3 流动性池？

| 对比维度    | V2 流动性池                    | V3 流动性池                                          |
| ------- | -------------------------- | ------------------------------------------------ |
| 流动性分布   | 全区间覆盖                      | 集中流动性 (自定义价格区间)                                  |
| 资金利用率   | 较低。大量资金闲置在极端价格，未被有效利用。     | 极高。相比 V2，资金效率最高可提升 4000 倍。                       |
| 操作门槛    | 极低。只需输入代币数量和 BNB 比例即可一键建池。 | 较高。需自行设定和调整流动性的价格上限和下限。                          |
| 手续费机制   | 固定收取 0.25% 交易手续费。          | 提供多个费率级别（如 0.01%, 0.05%, 0.25%, 1%），可根据资产波动性自定义。 |
| 无常损失风险  | 标准风险。资产价格变动带来的损失相对可预测。     | 较高风险。由于资金集中，若价格跌出你设定的区间，价格将瞬间击穿。                 |
| 滑点表现    | 在大额交易时，容易产生较大滑点。           | 在设定的流动性区间内，滑点极低，交易体验极佳。                          |
| 代币经济学兼容 | 完美兼容所有类型的代币。               | 部分具有复杂机制的代币在 V3 部署时可能出现兼容性问题。                    |

更详细对比 V2 / V3 流动性池定义以及适用场景，欢迎查阅：

{% content-ref url="../../../start/liquidity-configuration.md" %}
[liquidity-configuration.md](../../../start/liquidity-configuration.md)
{% endcontent-ref %}

***

## 为什么选择 CiaoTool 创建 V2 流动性池并捆绑买入？

对于需要严密掌控筹码分布的专业团队，CiaoTool 构筑了极致安全与高效的基础设施：

* **零代码安全防御：**\
  将复杂的底层防夹量化脚本，转化为直观的 Web 端可视化操作，任何人都能无门槛使用。
* **纯前端私钥隔离：**\
  平台严格采用客户端本地处理机制。您的钱包私钥仅在本地浏览器中用于交易签名，绝不上传、存储或传输至任何云端服务器，从技术底层切断资金风险。
* **端到端的生态闭环：**\
  CiaoTool 定位为全栈式代币生命周期管理平台。开盘建仓完成后，您可以无缝联动「市值管理」、「批量交易」等工具，一站式打造繁荣的链上数据表现。

***

## **图文指南 |** PancakeSwap 创建 V2 流动性池并捆绑买入

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 BSC 链的钱包

<figure><img src="../../../.gitbook/assets/image (446).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入创建流动性钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

当&#x524D;**「创建并买入」**&#x529F;能仅支持 私钥导入以进行开盘操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

该钱包地址将用于支付工具手续费，并拥有池子所有权。

<figure><img src="../../../.gitbook/assets/image (569).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入加池代币地址

将代币地址输入到框内，作为计价代币和项目代币，没有填写顺序。

<figure><img src="../../../.gitbook/assets/image (570).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入加池代币数量

分别输入两个加池代币放入流动性资金池的代币数量，请自行计算合适的比例后并确定初始币对价格后再创建流动性。

初始币对价格：`项目代币 / 计价代币 = 初始价格`

<figure><img src="../../../.gitbook/assets/image (571).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入捆绑买入私钥地址

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

当&#x524D;**「创建并买入」**&#x529F;能仅支持 私钥导入以进行多地址交易操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

1. 点&#x51FB;**「导入私钥」**&#x6309;钮，弹出上传弹窗。

<figure><img src="../../../.gitbook/assets/image (572).png" alt=""><figcaption></figcaption></figure>

2. 支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入钱包私钥的类型，最多支持 **20 个地址**捆绑买入。

<figure><img src="../../../.gitbook/assets/image (453).png" alt=""><figcaption></figcaption></figure>

使用 CiaoTool 模板文件导入，并保存确定导入并显示在输入框内。\
点击下载并查看模板：

{% file src="../../../.gitbook/assets/EVM_privateKey_demo.xlsx" %}

3. 系统将自动读取每个私钥的 **BNB 余额**

<figure><img src="../../../.gitbook/assets/image (574).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入买入金额

为每个地址设置「买入金额」 ，单个地址无上限买入金额，刷新余额查看即可。

{% hint style="danger" %}
买入地址的 BNB 余额必须大于 0.0008，以预留支付 Gas 等网络费用；

当选择 MAX 时，系统将自动预留 0.001 BNB 左右的余额于钱包内，您可手动调整范围。
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (455).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下&#x65B9;**「创建并买入」**&#x6309;钮，并等待开盘完成。
{% endstep %}
{% endstepper %}

***

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
