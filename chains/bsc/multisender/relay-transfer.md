---
description: >-
  中转转账功能旨在为用户提供一种更隐蔽和安全的转账方式。通过独立中间地址处理 BNB 和 BEP-20 / ERC-20
  的资金转移，有效打断资金关联，从而提高资金转账的隐私性和安全性。
metaLinks:
  alternates:
    - https://app.gitbook.com/s/b56FKZGe1viFi67H1pPQ/transfer/relay-transfer
---

# BSC - 批量转账 | 中转转账教程

{% hint style="info" %}
当前&#x662F;**「BSC - 中转转账」**&#x6559;程页面，点击[**「Solana - 中转转账」**](../../solana/multisender/sol-relay-transfer.md)查看 Solana 网络中转转账教程。
{% endhint %}

## CiaoTool BSC 中转转账是什么？ <a href="#definition" id="definition"></a>

<figure><img src="../../../.gitbook/assets/image (513).png" alt="CiaoTool BSC 中转转账页面"><figcaption></figcaption></figure>

**CiaoTool BSC 中转转账**是一款专为 BSC (BNB Smart Chain) 打造的高阶资产隐匿与防追踪流转工具。它允许用户在发送方（源钱包）与接收方（目标钱包）之间自动插入一层全新的“隔离中间钱包”，从而将原本在公开账本上一览无余的转账动作，拆分为「源地址 → 中转地址 → 目标地址」的断层式路径。

相比传统直接转账模式，中转转账无需用户手动创建和管理临时钱包。系统将自动完成中转地址生成、资金划转以及流程执行，大幅降低复杂资金迁移的操作门槛。

该功能适用于资产迁移、筹码重组、多钱包换仓、地址分散管理以及需要优化链上资金流向结构的场景，帮助用户更高效地完成多钱包资产调度。

立即在 BSC 网络上，用 CiaoTool​ 批量转账功能进行多对多转账操作：

{% embed url="https://bsc.ciaotool.io/zh-Hans/transfer/relay-transfer" %}

***

## 为什么选择 CiaoTool BSC 中转转账转账？ <a href="#advantage" id="advantage"></a>

在完全透明的区块链账本上处理核心筹码的位移，通常伴随着极高的被标记与关联风险。CiaoTool 为 BSC 链上的隐私资金调拨构建了兼顾极简交互与绝对隐匿的执行防线：

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

## **视频教程 | BSC 批量转账 - 中转转账** <a href="#solana-one-to-multi-guide" id="solana-one-to-multi-guide"></a>

{% embed url="https://www.youtube.com/watch?v=PfN-Fr84MvU" %}

***

## **图文指南 | BSC 批量转账 - 中转转账**  <a href="#solana-one-to-multi-guide" id="solana-one-to-multi-guide"></a>

{% stepper %}
{% step %}
### **切换公链并绑定钱包**

点击右上角按钮，绑定支持 EVM 网络的钱包

<figure><img src="../../../.gitbook/assets/image (475).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择转账代币

选择代币或直接输入代币地址。

<figure><img src="../../../.gitbook/assets/image (479).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入发送钱包私钥

{% hint style="danger" %}
**「多对多转账」**&#x529F;能支持使用私钥导入以进行转账操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

{% hint style="info" %}
发送钱包数量需要和接收钱包数量保持一致
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入发送钱包私钥的类型，选择以查看详细教程。

{% tabs %}
{% tab title="手动输入" %}
直接在输入框中，输入 / 粘贴发送钱包私钥。每行仅输入一个地址

<figure><img src="../../../.gitbook/assets/image (505).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 点&#x51FB;**「上传文件」**&#x6309;钮，弹出文件上传窗口导入发送钱包私钥。

<figure><img src="../../../.gitbook/assets/image (506).png" alt=""><figcaption></figcaption></figure>

2. 使用 CiaoTool 模板文件导入，并保存确定导入并显示在输入框内。\
   点击下载并查看模板：

{% file src="../../../.gitbook/assets/EVM_privateKey_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (507).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 导入接收钱包地址

{% hint style="info" %}
发送钱包数量需要和接收钱包数量保持一致
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入接收地址的类型，选择以查看详细教程。

{% tabs %}
{% tab title="手动输入" %}
直接在输入框中，输入 / 粘贴接收钱包地址。每行仅输入一个地址

<figure><img src="../../../.gitbook/assets/image (511).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 点&#x51FB;**「上传文件」**&#x6309;钮，弹出文件上传窗口导入接收钱包地址。

<figure><img src="../../../.gitbook/assets/image (512).png" alt=""><figcaption></figcaption></figure>

2. 使用 CiaoTool 模板文件导入，并保存确定导入并显示在输入框内。\
   点击下载并查看模板：

{% file src="../../../.gitbook/assets/EVM_address_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (509).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入转账金额

支&#x6301;**「自定义」「全部数量」「固定数量」「固定留存」**&#x56DB;种转账金额类型。

<figure><img src="../../../.gitbook/assets/image (502).png" alt=""><figcaption></figcaption></figure>

1.
   1. **自定义输入**\
      在输入框中，逐一输入转账金额数量
   * 若填写数量，则按照填写的数量进行转账。
   * 若未填写数量，则按照发送数量中     设置的数量进行转账。
   2. **全部数量**\
      所有钱包将余额内指定的代币全部发送到接收地址。
   3. **固定数量**\
      所有钱包根据同一数量将指定代币全部发送到接收地址。
   4. **固定留存**\
      所有钱包留存指定数量代币，其余全部数量发送到接收地址。
{% endstep %}

{% step %}
### 核对

点击下一步，核对发送信息，并查看状态栏。

<figure><img src="../../../.gitbook/assets/image (503).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下&#x65B9;**「发送」**&#x6309;钮，并等待转账程序完成。
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>什么是中转转账？</strong></summary>

BSC 中转转账是一款专注于链上隐私保护的可视化操作工具。它通过自动生成中间钱包作为“跳板”，将资金从发送方先转入中转地址，再由中转地址自动转入最终的接收钱包。这种机制能在区块链浏览器上有效切断发送方与接收方之间的直接交易记录。

</details>

<details>

<summary><strong>如何导入地址？</strong></summary>

你可以手动输入地址，也可以上传 Excel 文件导入目标地址列表，系统会自动识别并展示预览。

</details>

<details>

<summary><strong>是否支持不同地址转不同数量？</strong></summary>

可以。你可以为每个地址设置不同的转账数量，也可以设置统一的金额和制定金额分发给所有目标地址。

</details>

<details>

<summary><strong>操作是否安全？</strong></summary>

平台采用纯前端签名机制，您的私钥绝不会被上传或储存在任何服务器上，所有交易均在本地浏览器完成签名，从技术层面确保平台无法访问您的私钥。

</details>

<details>

<summary><strong>一次可以发送到多少个地址？</strong></summary>

得益于私钥导入的模式，多对多转账功能免除了逐一钱包签署的繁复工作，发送地址没有任何数量限制。

</details>

<details>

<summary><strong>可以同时转多种代币吗？</strong></summary>

当前版本支持选择单一代币进行批量转账；如需多种资产分发，可多次执行操作。

</details>

***

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
