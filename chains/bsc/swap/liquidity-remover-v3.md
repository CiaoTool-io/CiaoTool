---
description: >-
  CiaoTool 提供免代码的 PancakeSwap 移除 V3 流动性池基础组件。一键精准撤回 BSC
  链上指定价格区间的集中流动性与手续费收益。纯前端本地签名，助您安全高效地完成 Web3 做市策略调整与资金回笼。
metaLinks:
  alternates:
    - https://app.gitbook.com/s/b56FKZGe1viFi67H1pPQ/swap/remove-liquidity-v3
---

# BSC - 移除 V3 流动性教程

{% hint style="info" %}
当前&#x662F;**「PancakeSwap 移除 V3 流动性」**&#x6559;程页面，以移除 V3 流动性，回收资金。

想移除的 V2 流动性资金，请查阅[**「PancakeSwap 移除 V2 流动性」**](liquidity-remover-v2.md)**。**
{% endhint %}

## PancakeSwap 移除 V3 流动性池是什么？

<figure><img src="../../../.gitbook/assets/image (592).png" alt="CiaoTool BSC链 移除 PancakeSwap V3 流动性 功能页面"><figcaption></figcaption></figure>

PancakeSwap 移除 V3 流动性池 是指做市商或项目方从其部署的特定 V3 流动性中，按比例撤回底层资金并提取累积手续费收益的链上操作。

与 V2 的全区间同质化代币不同，V3 采用的是集中流动性（CLMM）机制，每个流动性都对应着一个包含特定价格区间的非同质化 LP 凭证。移除 V3 流动性，意味着您在精确缩减该特定价格区间内的盘面承载力，并进行资产结算。

核心适用场景：

* 做市利润结算与资金回笼： 项目阶段性目标达成后，安全撤回初始注入的底层做市资金（如 BNB）及交易产生的手续费收益。
* 动态做市策略调整： 当代币市场价格跌出或涨出原先设定的 V3 价格区间时，资金将处于闲置状态。此时需移除旧流动性，并在新的市场价格区间内重新建立池子。
* 应对极端市场行情： 在面临不可控的市场剧烈波动时，紧急撤回流动性以保护核心做市资产的安全。

立即在 BSC 上，用 CiaoTool​ 移除流动性功能进行一键回收资金操作：

{% embed url="https://bsc.ciaotool.io/zh-Hans/swap/v3/remove-liquidity-v3" %}

***

## 为什么选择 CiaoTool 移除 V3 流动性？

对于需要严密掌控筹码分布的专业团队，CiaoTool 构筑了极致安全与高效的基础设施：

* **零代码极速撤池：**\
  &#x20;将复杂的 LP 授权与销毁指令转化为直观的 Web 端可视化操作，无需编写底层调用脚本，任何人都能安全、精准地完成资金撤回。
* **纯前端私钥隔离：**\
  平台严格采用客户端本地处理机制。您的钱包私钥仅在本地浏览器中用于交易签名，绝不上传、存储或传输至任何云端服务器，从技术底层切断资金风险。
* **端到端的生态闭环：**\
  CiaoTool 定位为全栈式代币生命周期管理平台。资金撤回后，您可以立即联动「批量转账」进行分红发放，或利用「多对一转账」进行资产归集，实现资金调度无缝衔接。

***

## **图文指南 |** PancakeSwap 移除 V3 流动性

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 BSC 链的钱包

<figure><img src="../../../.gitbook/assets/image (446).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入移除流动性钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

当&#x524D;**「移除流动性」**&#x529F;能仅支持 私钥导入以进行回收操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

该钱包地址将用于支付工具手续费，并需确保该地址拥有池子权限。

<figure><img src="../../../.gitbook/assets/image (652).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择移除的币对

&#x20;现在拥有权限的币对，准备移除流动性。

<figure><img src="../../../.gitbook/assets/image (593).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 设置移除比例

自由设置移除比例，回收资金。

{% hint style="info" %}
**关于比例：**&#x5047;设池子都是您一个人加的， 那么这个百分比=池子的百分比。如果池子是多个人加的，就需要另外算的。比如，您本身占有池子份额的20%。那么您即便选择100%，整个池子也只是锁了20%的流动性。如果您选择20%，那么整个池子也就是锁了4%的流动性。
{% endhint %}
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下&#x65B9;**「开始交易」**&#x6309;钮，并等待移除程序完成。
{% endstep %}
{% endstepper %}

***

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
