---
description: >-
  在 BSC 链上实现同一区块内的集中流动性（CLMM）部署与极速建仓，彻底规避 MEV 夹子攻击。纯前端本地签名，助您安全、高效启动 Web3
  代币交易生态。
metaLinks:
  alternates:
    - >-
      https://app.gitbook.com/s/b56FKZGe1viFi67H1pPQ/swap/create-liquidity-and-buy-v3
---

# BSC - 创建 V3 流动性池并捆绑买入教程

{% hint style="info" %}
当前&#x662F;**「PancakeSwap 创建 V3 流动性池并捆绑买入」**&#x6559;程页面，以创建「集中流动性、自定义流动区间」的 V3 流动性池。

想创建具有「易用、全区间覆盖」的 V2 流动性池，请查阅[**「PancakeSwap 创建 V2 流动性池并捆绑买入」**](bundler-v2.md)**。**
{% endhint %}

## PancakeSwap 创建 V3 流动性池并捆绑买入是什么？

<figure><img src="../../../.gitbook/assets/image (575).png" alt="CiaoTool BSC链 创建 V3 流动性池并捆绑买入 页面"><figcaption></figcaption></figure>

**PancakeSwap V3 流动性池** 是 BNB 链（BSC）上最新一代的去中心化交易基础设施。与 V2 的全区间流动性不同，V3 引入了「集中流动性」机制，允许项目方在自定义的价格区间内提供流动性，从而以更少的初始资金实现成倍的交易深度与资金利用率。

**创建流动性池并捆绑买入**则是 CiaoTool 为项目量身打造的高阶开盘策略。在传统的开盘流程中，项目方手动添加流动性后，极易被埋伏在链上的 MEV 机器人在同一区块内抢先买入（俗称“抢首矿”或“夹子攻击”），导致项目方或真实用户被迫在高位接盘。CiaoTool 通过底层智能合约聚合指令，将「创建 V3 流动性池」与「初始资金买入建仓」打包在同一个区块链交易中执行。

**核心适用场景：**

* 精细化市值开盘： 适合资金量有限但需要极深交易盘面的项目方，利用 V3 特性集中资金，结合捆绑买入确保团队以绝对底价获取筹码。
* Meme 币冷启动： 针对极易引发机器人抢跑的 Meme 币，提供最高级别的防夹保护。
* 流动性极速部署： 缩短开盘繁琐步骤，提升资产在去中心化交易所的上线效率。

立即在 BSC 上，用 CiaoTool​ 创建并买入功能进行一键开盘操作：

{% embed url="https://bsc.ciaotool.io/zh-Hans/swap/v3/create-liquidity-and-buy-v3" %}

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

## 为什么选择 CiaoTool 创建 V3 流动性池并捆绑买入？

对于需要严密掌控筹码分布的专业团队，CiaoTool 构筑了极致安全与高效的基础设施：

* **零代码安全防御：**\
  将复杂的 V3 价格区间计算与底层防夹量化脚本，转化为直观的 Web 端可视化操作，任何人都能无门槛使用。
* **纯前端私钥隔离：**\
  平台严格采用客户端本地处理机制。您的钱包私钥仅在本地浏览器中用于交易签名，绝不上传、存储或传输至任何云端服务器，从技术底层切断资金风险。
* **端到端的生态闭环：**\
  CiaoTool 定位为全栈式代币生命周期管理平台。开盘建仓完成后，您可以无缝联动「市值管理」、「批量交易」等工具，一站式打造繁荣的链上数据表现。

***

## **图文指南 |** PancakeSwap 创建 V3 流动性池并捆绑买入

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
### 设置手续费级别

<figure><img src="../../../.gitbook/assets/image (576).png" alt=""><figcaption></figcaption></figure>

交易费用不同：V3 有四种不同的交易费等级，最多可比 V2 降低 25 倍交易费用；V2 每一笔交易将支付 0.25% 手续费。您也可以选择 1% 以获得更高的 LP 收益。
{% endstep %}

{% step %}
### 设置初始价格与价格区间

<figure><img src="../../../.gitbook/assets/image (577).png" alt=""><figcaption></figcaption></figure>

1. 区间大小決定收益高低 (LP 手续费收益、CAKE 收益皆适用)

* 越窄收益越高，无常损失越大；
* 越宽收益越低，无常损失越小；
* 全区间设置则类似于 V2 运作，收益将非常少。

2. 超出区间时

* V3 池无收益；
* 流动性仓位将变为单币；
* 可以移除流动性并重新添加，或是等待价格重新回到区间内。
* 可以添加 V2 流动性池，确保 V3 区间外基础流动性。
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

{% hint style="danger" %}
每个不同币对 / 不同税率的 V3 流动性池，有不同的币对地址，请务必保存币对合约地址信息，并将 LP 凭证保存至您的 Web3 钱包中。
{% endhint %}
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>为什么创建流动性并捆绑买入会失败？</strong></summary>

请确认钱包内 BNB / WBNB 余额是否充足，以覆盖加池，捆绑买入所需资金及 Gas 费用。

</details>

<details>

<summary><strong>为什么要将“创建”和“买入”捆绑在一起执行？</strong></summary>

如果先创建池子再手动买入，中间产生的时间差极易被链上狙击机器人监控并抢先买入，导致您被迫以数倍的高价接盘。捆绑执行消除了时间差，彻底阻断了恶意抢跑，保护了初始建仓的资金成本。

</details>

<details>

<summary><strong>这项功能可以用来优化代币早期的持币结构吗？</strong></summary>

可以。由于该功能支持批量导入多个钱包地址同步执行买入，这些买入会在代币创建的瞬间独立完成。这能让代币在刚发布时就展现出健康、分散的持币者分布数据，避免筹码过于集中在单一地址中。

</details>

<details>

<summary><strong>操作是否安全？</strong></summary>

平台采用纯前端签名机制，您的私钥绝不会被上传或储存在任何服务器上，所有交易均在本地浏览器完成签名，从技术层面确保平台无法访问您的私钥。

</details>

***

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
