---
description: >-
  专为 Solana 生态提供的 SOL 与 WSOL 双向互换工具。支持一键将原生 SOL 包装为 WSOL，或将 WSOL 快速解包还原为
  SOL，大幅提升多钱包做市与自动化交易的前置准备效率。
---

# Solana - WSOL 转换器

## CiaoTool WSOL 转换器是什么？ <a href="#what-is-coinfactory-solana-multisender" id="what-is-coinfactory-solana-multisender"></a>

**CiaoTool WSOL 转换器**是一款专为 Solana 生态用户及项目团队打造的基础资产互换工具。它旨在解决 Solana 链上原生代币 SOL 与包装代币 WSOL（Wrapped SOL）之间频繁转换的效率痛点。

在 Solana 网络中，原生的 SOL 属于公链底层燃料，并不直接兼容 SPL 标准代币协议。因此，在进行多钱包批量买卖、自动化做市以及与各类 DEX 的智能合约进行底层交互时，通常强制要求使用符合 SPL 标准的 WSOL。该转换器的核心机制在于提供一个可视化的极速双向通道：用户可以一键将多个钱包中的 SOL 转换为 WSOL，也可以随时将归集回来的 WSOL 解包还原为原生 SOL，确保资金在不同交易场景下的无缝流转。

立即在 Solana 上，用 CiaoTool 进行 WSOL 转换兑换操作：

{% embed url="https://ciaotool.io/zh-Hans/wallet/solana-wrapper" %}

***

## **图文指南**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (747).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择包装 / 解包

点击箭头切换包装 SOL / 解包 WSOL 的功能。

* 由于底层代码限制，SOL 包装成 WSOL 可以自定义输入指定包装数量。
* WSOL 解包为 SOL 时，只能全部解包为 WSOL，不能输入指定数量兑换。

<figure><img src="../../../.gitbook/assets/image (804).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择转换钱包

<figure><img src="../../../.gitbook/assets/image (805).png" alt=""><figcaption></figcaption></figure>

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

进行私钥导入操作时，请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入转账地址私钥的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「批量输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (807).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x6BCF;行仅输入一个钱包私钥，可在私钥后追加数量。

```
privateKey, 300
```

<figure><img src="../../../.gitbook/assets/image (737).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (808).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 下载 CiaoTool 模板文件，并将信息导入到文件内。

<figure><img src="../../../.gitbook/assets/image (810).png" alt=""><figcaption></figcaption></figure>

2. 点击![](<../../../.gitbook/assets/image (811).png>)**「导入文件」**&#x6309;钮，弹出文件上传窗口。
3. 点&#x51FB;**「确定导入」**，将所有地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (808).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入转账金额

支&#x6301;**「逐一输入」「输入金额」「随机范围」「保留金额」「百分比金额」**&#x548C;**「全部」**&#x516D;种转账金额类型。

<figure><img src="../../../.gitbook/assets/image (809).png" alt=""><figcaption></figcaption></figure>

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
### 发送形式

系统将根据收款地址数量自动分组，每组最多 1 个钱包。

<figure><img src="../../../.gitbook/assets/image (730).png" alt=""><figcaption></figcaption></figure>

1. **RPC 发送**\
   通过 RPC 节点统一广播转账交易，无需支付 Jito 小费。
2. **Jito Bundle**\
   将 5 组交易打包为一个捆绑包，通过 Jito 小费提升上链优先级并按顺序执行。
{% endstep %}

{% step %}
### 核实信息

确认页面并核对：

* [x] 转换钱包及转换代币数量
* [x] 新地址 ATA 租金
* [x] 本次预估费用

<figure><img src="../../../.gitbook/assets/image (812).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下&#x65B9;**「开始」**&#x6309;钮，并等待程序执行完成。
{% endstep %}
{% endstepper %}

***

## **寻求支持**

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
