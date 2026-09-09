---
description: 批量处理多个钱包地址 SOL 或 SPL 代币的资金转账，模拟真实转账，有效打乱地址关联，优化气泡图检测，提升多地址资金管理效率，丰富您的资产管理策略。
---

# Solana - 批量转账 | 多对多转账教程

{% hint style="info" %}
当前&#x662F;**「Solana 多对多转账」**&#x6559;程页面，点击[**「EVM - 多对多转账」**](../../../tools/multisender/multi-to-multi/many-to-many.md)以查看 BSC、opBNB、Base、X Layer、IoTeX、BOT、Robinhood Chain 等 EVM 网络多对多转账教程
{% endhint %}

## 功能介绍

CiaoTool Solana 多对多转账是一款批量资产调度工具，支持多个转出钱包向多个收款地址发送 SOL 或支持的 SPL 代币。

用户可分别配置每条“转出地址—收款地址—金额”关系；同一钱包能够向多个地址转账，同一地址也能接收多个钱包的资金。系统会将地址映射转换为转账任务，并根据数量自动分组执行。

**适用场景：**

* 社区奖励与多钱包批量付款
* 团队、合作方及用户资金结算
* 多账户资产迁移与结构调整
* DApp 测试账户充值或退款

立即在 Solana 上，用 CiaoTool​ 批量转账功能进行多对多转账操作：

{% embed url="https://ciaotool.io/zh-Hans/transfer/many-to-many" %}

***

## 核心优势

* **灵活映射：** 支持多个转出地址与多个收款地址自由组合
* **批量执行：** 系统自动生成、分组并提交转账任务，减少重复操作
* **便捷导入：** 支持通过 Excel 批量导入地址、金额及对应关系
* **金额可配：** 支持等额、定额或我等金额分配方式，满足不同资金调度需求
* **发送方式可选：** 支持 RPC 统一广播或 Jito 打包发送
* **过程可核对：** 提交前可确认转账关系、总金额及预估费用
* **本地签名：** 私钥仅在本地用于交易签名，无需上传至服务器

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

<figure><img src="../../../.gitbook/assets/image (779).png" alt=""><figcaption></figcaption></figure>
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

## **寻求支持**

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
