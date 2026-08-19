---
description: >-
  CiaoTool 提供免代码的 PancakeSwap V2 创建流动性池基础组件。在 BSC 链上一键 AMM
  资金池部署。纯前端本地处理机制，助您安全、低成本启动 Web3 代币交易生态。
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/b56FKZGe1viFi67H1pPQ/swap/create-add-liquidity-v2
---

# BSC - 创建 V2 流动性教程

{% hint style="info" %}
当前&#x662F;**「PancakeSwap 创建 V2 流动性池」**&#x6559;程页面，以创建「易用、全区间覆盖」的 V2 流动性池。

想创建具有「集中流动性、自定义流动区间」的 V3 流动性池，请查阅[**「PancakeSwap 创建 V3 流动性池」**](create-liquidity-v3.md)**。**
{% endhint %}

## PancakeSwap 创建 V2 流动性池是什么？

<figure><img src="../../../.gitbook/assets/image (580).png" alt="CiaoTool BSC链 PancakeSwap 创建 V2 流动性池 功能页面"><figcaption></figcaption></figure>

**PancakeSwap V2 流动性池** 是基于 BNB 链（BSC）上最经典的 AMM 机制的去中心化交易基础。它通过 `x * y = k` 的恒定乘积公式，为代币提供初始的交易定价与买卖深度。

对于任何新发行的代币而言，创建 V2 流动性池是代币转变为“可流通资产”的必经之路。通过注入一定比例的基础资产（如 BNB 或 USDT）与项目代币，项目方可为资产锚定初始价格，并搭建起无需许可的买卖市场。

核心适用场景：

* 资产首发与初始定价：刚完成部署的新代币需要通过建立 V2 流动性池来设定开盘价，并向全网开放交易权限。
* 建立底层基础流动性： 作为基石流动性，为后续的链上做市、借贷协议整合或跨链桥搭建提供基础深度。

立即在 BSC 上，用 CiaoTool​ 创建流动性池功能进行一键开盘操作：

{% embed url="https://bsc.ciaotool.io/zh-Hans/swap/v2/create-liquidity-v2" %}

***

## 如何选择 V2 / V3 流动性池？

| 对比维度    | V3 流动性池                                          | V2 流动性池                    |
| ------- | ------------------------------------------------ | -------------------------- |
| 流动性分布   | 集中流动性 (自定义价格区间)                                  | 全区间覆盖                      |
| 资金利用率   | 极高。相比 V2，资金效率最高可提升 4000 倍。                       | 较低。大量资金闲置在极端价格，未被有效利用。     |
| 操作门槛    | 较高。需自行设定和调整流动性的价格上限和下限。                          | 极低。只需输入代币数量和 BNB 比例即可一键建池。 |
| 手续费机制   | 提供多个费率级别（如 0.01%, 0.05%, 0.25%, 1%），可根据资产波动性自定义。 | 固定收取 0.25% 交易手续费。          |
| 无常损失风险  | 较高风险。由于资金集中，若价格跌出你设定的区间，价格将瞬间击穿。                 | 标准风险。资产价格变动带来的损失相对可预测。     |
| 滑点表现    | 在设定的流动性区间内，滑点极低，交易体验极佳。                          | 在大额交易时，容易产生较大滑点。           |
| 代币经济学兼容 | 部分具有复杂机制的代币在 V3 部署时可能出现兼容性问题。                    | 完美兼容所有类型的代币。               |

更详细对比 V2 / V3 流动性池定义以及适用场景，欢迎查阅：

{% content-ref url="../../../start/liquidity-configuration.md" %}
[liquidity-configuration.md](../../../start/liquidity-configuration.md)
{% endcontent-ref %}

***

## 为什么选择 CiaoTool 创建 V2 流动性池？

对于需要严密掌控筹码分布的专业团队，CiaoTool 构筑了极致安全与高效的基础设施：

* **零代码高效部署：**\
  将复杂的 AMM 合约交互转化为直观的 Web 端可视化操作，无需编写底层调用脚本，任何人都能安全、精准地完成资金池初始化。
* **纯前端私钥隔离：**\
  平台严格采用客户端本地处理机制。您的钱包私钥仅在本地浏览器中用于交易签名，绝不上传、存储或传输至任何云端服务器，从技术底层切断资金风险。
* **端到端的生态闭环：**\
  CiaoTool 定位为全栈式代币生命周期管理平台。开盘建仓完成后，您可以无缝联动「市值管理」、「批量交易」等工具，一站式打造繁荣的链上数据表现。

***

## **图文指南 |** PancakeSwap 创建 V2 流动性池

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 BSC 链的钱包

<figure><img src="../../../.gitbook/assets/image (446).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入创建流动性池钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

当&#x524D;**「创建流动性池」**&#x529F;能仅支持 私钥导入以进行开盘操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
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

<figure><img src="../../../.gitbook/assets/image (581).png" alt=""><figcaption></figcaption></figure>

分别输入两个加池代币放入流动性资金池的代币数量，请自行计算合适的比例后并确定初始币对价格后再创建流动性。

初始币对价格：`项目代币 / 计价代币 = 初始价格`
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
