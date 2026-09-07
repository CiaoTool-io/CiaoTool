---
description: 通过独立中间地址处理 SOL 的资金转移，切断首尾直接联系，有效打断资金关联，优化气泡图呈现，提升多钱包资金调拨安全性，打造深度隐匿的资产管理策略。
---

# Solana - 批量转账 | 中转转账教程

{% hint style="info" %}
当前&#x662F;**「Solana 中转转账」**&#x6559;程页面，点击[**「BSC - 中转转账」**](../../bsc/multisender/relay-transfer.md)以查看 BSC 网络多对多转账教程。
{% endhint %}

## CiaoTool Solana 中转转账是什么？

<figure><img src="../../../.gitbook/assets/image (764).png" alt="CiaoTool Solana 中转转账页面"><figcaption></figcaption></figure>

**CiaoTool Solana 中转转账**是一款专注于链上隐私保护与资金隐匿的高阶工具。它允许您在转账过程中自动引入独立的中间钱包节点，将 SOL（原生代币） 智能中转并批量分发至目标钱包。

相较于普通的直接转账，中转转账的核心优势在于切断发送端与接收端之间的直接链上联系。系统通过中间地址自动处理资金流转，完美模拟真实独立交互行为，有效打乱资金流转路径，优化气泡图等链上工具的聚类分析与追踪显示。这不仅能隐藏资金的动向，保护主钱包安全隐私，保障多钱包交互的安全流转。

此工具尤其适用于： ​ ​

* 隐私保护下的 SOL 资金调拨与分仓策略
* 优化链上气泡图与聚类分析显示
* 安全的多地址资产分布管理

立即在 Solana 上，用 CiaoTool​ 批量转账功能进行中转转账操作：

{% embed url="https://ciaotool.io/zh-Hans/transfer/relay-transfer" %}

***

## 为什么选择 CiaoTool 中转转账？

在完全透明的区块链账本上处理核心筹码的位移，通常伴随着极高的被标记与关联风险。CiaoTool 为 Solana 链上的隐私资金调拨构建了兼顾极简交互与绝对隐匿的执行防线：

**智能中转隔离机制**\
系统自动在发送地址与接收地址之间创建独立中转钱包，将单一路径转账拆分为多段执行流程，优化链上资金流向结构与地址关联关系。

**全自动中转钱包生成**\
无需手动创建临时钱包或管理复杂地址矩阵。系统根据任务需求自动生成对应数量的中转钱包，并完成全部转账流程，大幅降低操作复杂度。

**批量中转高效执行**\
支持多个钱包同时执行中转任务，无需频繁切换账户与重复签名。通过批量化执行机制，大幅提升大规模资产迁移效率。

**优化资金分布结构**\
支持结合多地址迁移与中转机制进行资产重组，使资金流转路径更加灵活，满足筹码分散、仓位调整与多钱包管理等复杂场景需求。​

**本地安全环境**\
采用纯前端本地执行机制，私钥仅在本地环境中用于交易签名，在极速提升交易效率的同时，全方位保障多钱包资产的绝对安全。

***

## **技术实现示意**

中转转账采用“两阶段路由”机制，在源钱包与目标钱包之间创建临时中转钱包，将一次直接转账拆分为两笔独立的链上交易：

**「源钱包 → 中转钱包 → 目标钱包」**

<figure><img src="../../../.gitbook/assets/Frame 1321314893.png" alt=""><figcaption></figcaption></figure>

***

## **图文指南**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角【连接钱包】按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (748).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入发送钱包私钥

{% hint style="danger" %}
**「中转转账」**&#x529F;能仅支持私钥导入以进行转账操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

{% hint style="info" %}
发送钱包数量需要和接收钱包数量保持一致
{% endhint %}

导入钱包数量没有限制，支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入来源地址的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「批量输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (765).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x6BCF;行仅输入一个钱包私钥，可在私钥后追加数量。

```
privateKey, 300
```

<figure><img src="../../../.gitbook/assets/image (737).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (769).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 下载 CiaoTool 模板文件，并将信息导入到文件内。

<figure><img src="../../../.gitbook/assets/image (766).png" alt=""><figcaption></figcaption></figure>

2. 点&#x51FB;**「导入文件」**&#x6309;钮，弹出文件上传窗口。

<figure><img src="../../../.gitbook/assets/image (767).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (768).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入转账金额

支&#x6301;**「逐一输入」「输入金额」「随机范围」「保留金额」「百分比金额」**&#x548C;**「全部」**&#x516D;种转账金额类型。

<figure><img src="../../../.gitbook/assets/image (770).png" alt=""><figcaption></figcaption></figure>

1. **逐一输入**\
   在输入框中，逐一输入转账金额数量。

<figure><img src="../../../.gitbook/assets/image (771).png" alt=""><figcaption></figcaption></figure>

2. **统一金额**\
   点击转账数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「输入金额」**&#x9009;项，所有地址将统一转账数量。
3. **随机范围**\
   点击转账数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「随机范围」**&#x9009;项，输入金额范围，所有地址将转账指定范围内数额。
4. **保留金额**\
   点击转账数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「保留金额」**&#x9009;项，所有发送钱包保留指定数量的目标代币，并将剩余代币全部转账到收款地址。
5. **保留金额**\
   点击转账数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「百分比金额」**&#x9009;项，所有发送钱包保留指定百分比的目标代币，并将剩余代币全部转账到收款地址。
6. **全部**\
   点击转账数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「全部」**&#x9009;项，所有发送钱包将目标代币全部转账到收款地址。
{% endstep %}

{% step %}
### 导入收款地址

{% hint style="info" %}
转出钱包数量需要和接收钱包数量保持一致
{% endhint %}

收款钱包数量没有限制，支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入接收地址的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「批量输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (772).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x6BCF;行仅输入一个钱包地址。

```
address
```

<figure><img src="../../../.gitbook/assets/image (719).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (776).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 下载 CiaoTool 模板文件，并将信息导入到文件内。

<figure><img src="../../../.gitbook/assets/image (773).png" alt=""><figcaption></figcaption></figure>

2. 点&#x51FB;**「导入文件」**&#x6309;钮，弹出文件上传窗口。

<figure><img src="../../../.gitbook/assets/image (774).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (775).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 中继钱包

可自由设置各地址转账到目标钱包的中继钱包数量。

提高中继钱包数量可以提升来源钱包私密性，但费用和损耗会随之上升。

<figure><img src="../../../.gitbook/assets/image (777).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 发送形式

系统将根据收款地址数量自动分组，每组最多 4 个收发地址。

<figure><img src="../../../.gitbook/assets/image (730).png" alt=""><figcaption></figcaption></figure>

1. **RPC 发送**\
   通过 RPC 节点统一广播转账交易，无需支付 Jito 小费，各笔交易不保证按提交顺序执行。
2. **Jito Bundle**\
   每个捆绑包最多 20 个转账地址（5 组），通过 Jito 小费提升上链优先级并按顺序执行。
{% endstep %}

{% step %}
### 核实信息

点&#x51FB;**「下一步」**&#x8FDB;入确认页面并核对：

* [x] 每个中转任务的收发地址
* [x] 转账数量、转账总额，预计转入数量
* [x] 本次转账预估服务费用

<figure><img src="../../../.gitbook/assets/image (778).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下方「**确认并发送**」按钮，您可以实时查看转账程序完成情况，并等待转账程序完成。

<figure><img src="../../../.gitbook/assets/image (732).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

***

## **常见问题**

<details>

<summary><strong>什么是中转转账？</strong></summary>

Solana 中转转账是一款专注于链上隐私保护的可视化操作工具。它通过自动生成中间钱包作为“跳板”，将资金从发送方先转入中转地址，再由中转地址自动转入最终的接收钱包。这种机制能在区块链浏览器上有效切断发送方与接收方之间的直接交易记录。

</details>

<details>

<summary><strong>如何导入地址？</strong></summary>

你可以手动输入地址，也可以上传 CSV 文件导入目标地址列表（支持地址+金额格式），系统会自动识别并展示预览。

</details>

<details>

<summary><strong>操作是否安全？</strong></summary>

平台采用纯前端签名机制，您的私钥绝不会被上传或储存在任何服务器上，所有交易均在本地浏览器完成签名，从技术层面确保平台无法访问您的私钥。

</details>

<details>

<summary><strong>一次可以发送到多少个地址？</strong></summary>

得益于私钥导入的模式，中转转账功能免除了逐一钱包签署的繁复工作，发送地址没有任何数量限制。

</details>

<details>

<summary><strong>可以同时转多种代币吗？</strong></summary>

当前版本仅支持选择 SOL 进行批量转账。

</details>

***

## **寻求支持**

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
