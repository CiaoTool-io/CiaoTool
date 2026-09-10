---
description: 快速将少量地址中的代币分散至多个全新地址，降低前排持有量，优化链上分布结构，提升图表自然度和项目可信度。
---

# Solana - 冷换仓教程

{% hint style="info" %}
当前&#x662F;**「Solana - 冷换仓」**&#x6559;程页面以查看 Solana 网络冷换仓教程。

点击[**「EVM - 冷换仓」**](../../../tools/multisender/leng-huan-cang/fragmentation.md)以查看 **BSC、Base、X Layer、IoTeX、Robinhood Chain** 等 EVM 网络教程。
{% endhint %}

## 功能介绍 <a href="#definition" id="definition"></a>

CiaoTool Solana 冷换仓是一款批量代币分仓工具，可将集中在一个或多个钱包中的代币，按固定金额、设定比例或随机金额，分配至多个新建或已有的 Solana 钱包。

系统可自动生成接收钱包、计算分配金额、构建转账任务并分组执行，无需通过中心化交易平台或 DEX 完成买卖，适用于项目资产配置与多钱包持仓管理。

**适用场景：**

* **项目资产分仓：** 将代币分配至金库、运营及不同业务钱包
* **团队与社区分配：** 按既定规则向贡献者或成员发放代币
* **风险隔离：** 减少资产集中存放带来的单点管理风险
* **运营账户准备：** 为后续测试、流动性管理等授权用途配置钱包

立即在 Solana 网络上，用 CiaoTool​ 冷换仓功能进行持仓打散与碎片化资产迁移操作：

{% embed url="https://ciaotool.io/zh-Hans/asset-migration/fragmentation" %}

***

## 核心优势 <a href="#advantage" id="advantage"></a>

* **自动创建钱包：** 批量生成接收地址并整理对应钱包信息
* **灵活分配：** 支持固定、比例或随机金额等分仓方式
* **自动分组：** 根据任务数量构建并提交多笔转账交易
* **结果可追踪：** 展示每条任务的转账金额、交易 Hash 和执行状态
* **本地签名：** 私钥仅在本地用于交易授权，无需上传至服务器

***

## **图文指南** <a href="#solana-one-to-multi-guide" id="solana-one-to-multi-guide"></a>

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角【连接钱包】按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (748).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择转账代币

可以选择 SOL，也可以选择当前钱包拥有的代币进行转账。

<figure><img src="../../../.gitbook/assets/image (781).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入发送钱包私钥

{% hint style="danger" %}
**「冷换仓」**&#x529F;能仅支持私钥导入以进行转账操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

导入钱包数量没有限制，支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入来源地址的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「批量输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (782).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x6BCF;行仅输入一个钱包私钥，可在私钥后追加数量。

```
privateKey, 300
```

<figure><img src="../../../.gitbook/assets/image (737).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (787).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 下载 CiaoTool 模板文件，并将信息导入到文件内。

<figure><img src="../../../.gitbook/assets/image (783).png" alt=""><figcaption></figcaption></figure>

2. 点击![「导入文件」](<../../../.gitbook/assets/image (784).png>)按钮，弹出文件上传窗口。
3. 点&#x51FB;**「确定导入」**，将所有地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (786).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入转账金额

支&#x6301;**「逐一输入」「输入金额」「随机范围」「保留金额」「百分比金额」**&#x548C;**「全部」**&#x516D;种转账金额类型。

<figure><img src="../../../.gitbook/assets/image (788).png" alt=""><figcaption></figcaption></figure>

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
### 生成换仓钱包

可自由设置各换仓任务转账的新钱包的数量。

提高冷钱包数量可以将目标代币分散至更多地址，但也会产生更多损耗和 ATA 租金费用。

<figure><img src="../../../.gitbook/assets/image (789).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 发送形式

<figure><img src="../../../.gitbook/assets/image (730).png" alt=""><figcaption></figcaption></figure>

1. **RPC 发送**\
   通过 RPC 节点统一广播转账交易，无需支付 Jito 小费。
2. **Jito Bundle**\
   通过 Jito 小费提升上链优先级并按顺序执行。
{% endstep %}

{% step %}
### 核实信息

确认页面并核对：

* [x] 来源钱包及分仓钱包数量
* [x] 转账数量、转账总额、新地址 ATA 租金
* [x] 本次转账预估费用

<figure><img src="../../../.gitbook/assets/image (790).png" alt=""><figcaption></figcaption></figure>
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

<summary><strong>冷换仓的作用是什么？</strong></summary>

冷换仓可将代币从当前地址分散转移至大量新地址，降低单一地址持仓比例，优化链上分布结构，增强项目安全性和隐蔽性。

</details>

<details>

<summary><strong>为什么换仓后要使用新生成的钱包地址？</strong></summary>

新地址无历史交易记录，可避免被链上工具标记为“关联钱包”，更适合用于策略重建和分散操作。

</details>

<details>

<summary><strong>操作是否安全？</strong></summary>

平台采用纯前端签名机制，您的私钥绝不会被上传或储存在任何服务器上，所有交易均在本地浏览器完成签名，从技术层面确保平台无法访问您的私钥。

</details>

<details>

<summary><strong>可以同时换仓多种代币吗？</strong></summary>

当前版本支持选择单一代币进行碎片化换仓；如需多种资产分发，可多次执行操作。

</details>

***

## **寻求支持**

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
