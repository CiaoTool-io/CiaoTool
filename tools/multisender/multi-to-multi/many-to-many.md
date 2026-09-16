---
description: 批量将多个钱包中的原生代币或 ERC-20 项目代币转入对应接收地址，支持灵活金额设置、固定或随机发送间隔，让多钱包资产调拨更加便捷。
metaLinks:
  alternates:
    - https://app.gitbook.com/s/b56FKZGe1viFi67H1pPQ/transfer/many-to-many
---

# EVM - 批量转账 | 多对多转账教程

{% hint style="info" %}
当前&#x662F;**「EVM - 多对多转账」**&#x6559;程页面以查看 **BSC、opBNB、Base、X Layer、IoTeX、Robinhood Chain** 等 EVM 网络教程。

本教程演示基于 BSC（BNB Chain）功能页面，本功能 EVM 网络 CiaoTool 全链通用，请切换至对应公链进行一对多转账操作。

点击[**「Solana - 多对多转账」**](../../../chains/solana/multisender/many-to-many-old.md)查看 Solana 网络多对多转账教程。
{% endhint %}

## CiaoTool EVM 多对多转账是什么？ <a href="#definition" id="definition"></a>

<figure><img src="../../../.gitbook/assets/image (504).png" alt="CiaoTool EVM 多对多转账页面"><figcaption></figcaption></figure>

**CiaoTool EVM 多对多转账**是一款免代码批量转账工具，支持从多个发送钱包向各自对应的接收地址发送原生代币（例如 BNB）或受支持的 ERC-20 / BEP-20 代币。

通过批量导入钱包、设置转账金额及发送参数，即可统一完成多组转账。系统自动进行交易分组和浏览器本地签名，并提供费用复核、实时进度及失败原因查看，减少重复切换钱包和逐笔操作。

**适用场景：**

* **资产迁移：**&#x5C06;多个旧钱包的资产转入对应的新钱包。
* **运营资金调拨：**&#x6309;计划向对应运营账户分配资金。
* **团队与合作方结算：**&#x4ECE;不同付款钱包向指定收款方批量付款。
* **测试账户管理：**&#x6279;量完成测试钱包注资、退款或余额转移。
* **多账户资金整理：**&#x7ED3;合保留金额、百分比等设置，调整各钱包的资产配置。

立即在 EVM 网络上，用 CiaoTool​ 批量转账功能进行多对多转账操作：

<table data-view="cards"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/BSC.png" alt="" data-size="line">BSC (BNB Chain)</td><td><a href="https://bsc.ciaotool.io/zh-Hans/transfer/many-to-many">https://bsc.ciaotool.io/zh-Hans/transfer/many-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/BSC.png" alt="" data-size="line">opBNB Chain</td><td><a href="https://opbnb.ciaotool.io/zh-Hans/transfer/many-to-many">https://opbnb.ciaotool.io/zh-Hans/transfer/many-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/Base3.png" alt="" data-size="line">Base Chain</td><td><a href="https://base.ciaotool.io/zh-Hans/transfer/many-to-many">https://base.ciaotool.io/zh-Hans/transfer/many-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/3 (1).png" alt="" data-size="line">X Layer</td><td><a href="https://xlayer.ciaotool.io/zh-Hans/transfer/many-to-many">https://xlayer.ciaotool.io/zh-Hans/transfer/many-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/IoTex.png" alt="" data-size="line">IoTeX Chain</td><td><a href="https://iotex.ciaotool.io/zh-Hans/transfer/many-to-many">https://iotex.ciaotool.io/zh-Hans/transfer/many-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/BOT-2.png" alt="" data-size="line"> BOT Chain</td><td><a href="https://bot.ciaotool.io/zh-Hans/transfer/many-to-many">https://bot.ciaotool.io/zh-Hans/transfer/many-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/Group 1261152954.png" alt="" data-size="line"> Robinhood Chain</td><td><a href="https://r.ciaotool.io/zh-Hans/transfer/many-to-many">https://r.ciaotool.io/zh-Hans/transfer/many-to-many</a></td></tr></tbody></table>

***

## 核心优势

* **批量操作：**&#x4E00;次导入多组钱包，减少重复录入与钱包切换。
* **金额灵活：**&#x652F;持逐一输入、统一金额、随机范围、保留金额、百分比及全部余额。
* **发送节奏可控：**&#x652F;持固定间隔和随机延时。
* **新手友好：**&#x901A;过可视化步骤完成操作，无需编程。
* **非托管：**&#x7528;户保留钱包控制权，私钥用于浏览器本地签名，不上传或存储到 CiaoTool 服务器。

***

## **图文指南** <a href="#solana-one-to-multi-guide" id="solana-one-to-multi-guide"></a>

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

1. **自定义输入**\
   在输入框中，逐一输入转账金额数量

* 若填写数量，则按照填写的数量进行转账。
* 若未填写数量，则按照发送数量中  设置的数量进行转账。

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

<summary><strong>什么是多对多批量转账？</strong></summary>

它是一款多钱包批量转账工具，可以将多个发送钱包中的 SOL 或受支持代币，分别转入对应接收地址，并统一完成配置、费用复核和进度跟踪。

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
