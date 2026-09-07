---
description: 批量处理多个钱包地址 SOL 或 SPL 代币的资金转账，模拟真实转账，有效打乱地址关联，优化气泡图检测，提升多地址资金管理效率，丰富您的资产管理策略。
---

# Solana - 批量转账 | 多对多转账教程

{% hint style="info" %}
当前&#x662F;**「Solana 多对多转账」**&#x6559;程页面，点击[**「EVM - 多对多转账」**](../../../tools/multisender/multi-to-multi/many-to-many.md)以查看 BSC、opBNB、Base、X Layer、IoTeX、BOT、Robinhood Chain 等 EVM 网络多对多转账教程
{% endhint %}

## CiaoTool Solana 多对多转账是什么？

<figure><picture><source srcset="../../../.gitbook/assets/屏幕截图 2026-09-04 180127.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (750).png" alt="CiaoTool Solana 批量转账 多对多转账页面"></picture><figcaption></figcaption></figure>

**CiaoTool Solana 多对多转账**是一款高阶并行资产流转与财务分发工具。它允许用户在单次操作中，将多个独立源钱包（发送方）中的 **SOL（原生代币）**&#x6216;**任何 SPL 代币**，交叉且批量地发送至多个目标接收钱包。

相较于传统单向的「一转多」或「多转一」模式，该功能的核心机制在于「全方位交叉矩阵流转」。系统打破了地址映射的单一性限制，在底层自动建立多源头到多目标的交叉网状关系。这意味着：源地址 A 与源地址 B 可以同时向目标地址 A 打款；同理，源地址 A 与源地址 B 也可同时向目标地址 B 分发。此功能完美适配项目方在进行复杂的社区定向交叉奖励分发、多地址矩阵资金重组、防追踪深度混淆链上资金轨迹，或大规模测试账户退款等高度复杂的账本处理场景。

立即在 Solana 上，用 CiaoTool​ 批量转账功能进行多对多转账操作：

{% embed url="https://ciaotool.io/zh-Hans/transfer/many-to-many" %}

***

## 为什么选择 CiaoTool 多对多转账？

处理跨越几十甚至上百个独立源地址到多目标地址的资金交叉分发，通常伴随着极高的操作失误率与私钥管理风险。CiaoTool 为 Solana 链上的复杂矩阵调拨构建了兼顾极简交互与绝对安全的执行防线：

**复杂矩阵一键执行**\
支持多个发送地址与多个接收地址同时参与转账，无需逐个钱包重复操作。一次配置即可批量完成复杂资金调拨，大幅提升多账户协同管理效率。

**百倍提升效率：**\
彻底免去人工频繁切换账号、复制粘贴地址与重复授权签名的繁琐流程，支持一键并发执行成百上千笔转账，实现链上资产的极速归集。 ​

**优化资金分布结构**\
通过多地址交叉转账与随机金额分配机制，有效打散单一路径的大额资金流向，使整体资金迁移更加自然，帮助优化链上地址之间的关联结构。

**灵活的矩阵配置：**\
支持通过 Excel 电子表格文件一键批量导入目标地址列表与对应的分发额度。支持自定义等额、定额或随机金额分配，完美适配复杂多变的空投策略与持币分布需求。 ​

**本地安全环境：**\
采用纯前端本地执行机制，私钥仅在本地环境中用于交易签名，在极速提升交易效率的同时，全方位保障多钱包资产的绝对安全。

***

## **技术实现示意**

多对多转账以「转出地址—收款地址—金额」为基本任务单元，通过建立多源地址与多目标地址之间的映射关系。有效分散资金来源，模拟真实转账行为。

{% columns %}
{% column %}
<table><thead><tr><th width="76">发送地址</th><th width="76">收款地址</th><th>转账金额</th></tr></thead><tbody><tr><td>A</td><td>1</td><td>A→1 配置金额</td></tr><tr><td>A</td><td>2</td><td>A→2 配置金额</td></tr><tr><td>A</td><td>3</td><td>A→3 配置金额</td></tr><tr><td>B</td><td>1</td><td>B→1 配置金额</td></tr><tr><td>B</td><td>2</td><td>B→2 配置金额</td></tr><tr><td>B</td><td>3</td><td>B→3 配置金额</td></tr></tbody></table>


{% endcolumn %}

{% column %}
<figure><img src="../../../.gitbook/assets/Section 2.png" alt=""><figcaption></figcaption></figure>


{% endcolumn %}
{% endcolumns %}

***

## **图文指南**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角【连接钱包】按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (748).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择转账代币

可以选择 SOL，也可以选择当前钱包拥有的代币进行转账。

<figure><img src="../../../.gitbook/assets/image (751).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入发送钱包私钥

{% hint style="danger" %}
**「多对多转账」**&#x529F;能仅支持私钥导入以进行转账操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

{% hint style="info" %}
转出钱包数量需要和接收钱包数量保持一致
{% endhint %}

导入钱包数量没有限制，支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入来源地址的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「批量输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (752).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x6BCF;行仅输入一个钱包私钥，可在私钥后追加数量。

```
privateKey, 300
```

<figure><img src="../../../.gitbook/assets/image (737).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (753).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 下载 CiaoTool 模板文件，并将信息导入到文件内。

<figure><img src="../../../.gitbook/assets/image (754).png" alt=""><figcaption></figcaption></figure>

2. 点&#x51FB;**「导入文件」**&#x6309;钮，弹出文件上传窗口。

<figure><img src="../../../.gitbook/assets/image (755).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (738).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入转账金额

支&#x6301;**「逐一输入」「输入金额」「随机范围」「保留金额」「百分比金额」**&#x548C;**「全部」**&#x516D;种转账金额类型。

<figure><img src="../../../.gitbook/assets/image (756).png" alt=""><figcaption></figcaption></figure>

1. **逐一输入**\
   在输入框中，逐一输入转账金额数量。

<figure><img src="../../../.gitbook/assets/image (757).png" alt=""><figcaption></figcaption></figure>

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

<figure><img src="../../../.gitbook/assets/image (758).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x6BCF;行仅输入一个钱包地址。

```
address
```

<figure><img src="../../../.gitbook/assets/image (719).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (720).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 下载 CiaoTool 模板文件，并将信息导入到文件内。

<figure><img src="../../../.gitbook/assets/image (759).png" alt=""><figcaption></figcaption></figure>

2. 点&#x51FB;**「导入文件」**&#x6309;钮，弹出文件上传窗口。

<figure><img src="../../../.gitbook/assets/image (761).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (760).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 转账时间

可自由设置各地址转账执行间隔时间。

<figure><img src="../../../.gitbook/assets/image (729).png" alt=""><figcaption></figcaption></figure>

1. **固定时间**\
   设置为 0 时，所有转账立即提交广播，快速分发资金。
2. **随机时间**\
   转账将会在指定的时间范围内随机提交，模拟真实转账行为，但需要保持页面以持续执行。
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

* [x] 费用钱包地址及余额
* [x] 收发地址及数量、转账总额
* [x] 本次转账预估费用

<figure><img src="../../../.gitbook/assets/image (746).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下方「**确认并发送**」按钮，您可以实时查看转账程序完成情况，并等待转账程序完成。

<figure><img src="../../../.gitbook/assets/image (732).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>什么是多对多批量转账？</strong></summary>

Solana 多对多批量转账工具是一款可视化服务工具。无需代码即可允许您同时从多个发送钱包向多个目标地址并发分发代币。通过网状交叉的转账模式，它能打破单一的资金轨迹，比手动操作更精准、更具隐蔽性。

</details>

<details>

<summary><strong>如何导入地址？</strong></summary>

你可以手动输入地址，也可以上传 Excel 文件导入目标地址列表（支持地址+金额格式），系统会自动识别并展示预览。

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

当前版本支持选择单一 SPL 代币或 SOL 进行批量转账；如需多种资产归集，可多次执行操作。

</details>

***

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
