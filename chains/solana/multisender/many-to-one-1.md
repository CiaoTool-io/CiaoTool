---
description: 方便快捷地将分散在多个账户中的 SOL 或 SPL 代币统一归集到一个主账户，提高资金管理的效率，同时减少交易成本和时间。
hidden: true
---

# Solana - 批量转账 | 多对一转账教程

{% hint style="info" %}
当前&#x662F;**「Solana 多对一转账」**&#x6559;程页面，点击[**「EVM - 多对一转账」**](../../../tools/multisender/multi-to-one/many-to-one.md)以查看 BSC、opBNB、Base、X Layer、IoTeX、BOT、Robinhood Chain 等 EVM 网络多对一转账教程
{% endhint %}

## CiaoTool Solana 多对一转账是什么？ <a href="#definition" id="definition"></a>

<figure><picture><source srcset="../../../.gitbook/assets/屏幕截图 2026-09-04 170749.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (733).png" alt="CiaoTool Solana 批量转账 多对一转账页面"></picture><figcaption></figcaption></figure>

**CiaoTool  Solana 多对一转账**是一款高效链上资产回笼与多钱包资金管理工具。它允许用户在单次可视化操作中，将分散在成百上千个子钱包中的 **SOL（原生代币）**&#x6216;**任何 SPL 代币**，全自动地集中汇聚至一个主地址中。

相较于「逐笔复制地址、手动签名转账」的传统模式，该功能的核心机制在于「底层批量指令聚合」。系统会将海量的独立转账指令通过智能合约整合为一个不可分割的数据包提交至链上。这种机制不仅将原本需要耗费数小时的机械性工作缩短至一键秒级完成，更通过合并同类项大幅平摊了整体的网络费。

立即在 Solana 上，用 CiaoTool​ 批量转账功能进行多对一转账操作：

{% embed url="https://ciaotool.io/zh-Hans/transfer/many-to-one" %}

***

## 为什么选择 CiaoTool 多对一转账？ <a href="#advantage" id="advantage"></a>

CiaoTool 为 Solana 网络上的海量资产调拨提供了一种兼顾绝对安全与极简操作的专业解决方案。对于需要高频、大批量分发代币或基础燃料的用户而言，该工具构建了高效且稳健的执行防线： ​ ​

**百倍提升效率：**\
彻底免去人工频繁切换账号、复制粘贴地址与重复授权签名的繁琐流程，支持一键并发执行成百上千笔转账，实现链上资产的极速归集。 ​

**灵活的矩阵配置：**\
支持通过 Excel 电子表格文件一键批量导入目标地址列表与对应的分发额度。支持自定义等额、定额或随机金额分配，完美适配复杂多变的空投策略与持币分布需求。 ​

**本地安全环境：**\
采用纯前端本地执行机制，私钥仅在本地环境中用于交易签名，在极速提升交易效率的同时，全方位保障多钱包资产的绝对安全。

***

## **图文指南**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角【连接钱包】按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (712).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择转账代币

可以选择 SOL，也可以选择当前钱包拥有的代币进行转账。

<figure><img src="../../../.gitbook/assets/image (735).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择转账钱包

{% hint style="danger" %}
使用其他私钥钱包模式时，请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (715).png" alt=""><figcaption></figcaption></figure>

**当前连接钱包：**&#x76F4;接使用当前钱包直接进行转账操作，无需使用私钥，资金更安全。

**其他私钥钱包：**&#x4F7F;用私钥的形式进行转账操作，无需切换当前钱包快速调用备用钱包。
{% endstep %}

{% step %}
### 导入来源钱包私钥

{% hint style="danger" %}
**「多对一转账」**&#x529F;能仅支持私钥导入以进行转账操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

导入钱包数量没有限制，支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入来源地址的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「批量输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (736).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x6BCF;行仅输入一个钱包私钥，可在私钥后追加数量。

```
privateKey, 300
```

<figure><img src="../../../.gitbook/assets/image (737).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (738).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 下载 CiaoTool 模板文件，并将信息导入到文件内。

<figure><img src="../../../.gitbook/assets/image (739).png" alt=""><figcaption></figcaption></figure>

2. 点&#x51FB;**「导入文件」**&#x6309;钮，弹出文件上传窗口。

<figure><img src="../../../.gitbook/assets/image (740).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (738).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入转账金额

支&#x6301;**「逐一输入」「全部」「输入金额」**&#x548C;**「保留金额」**&#x56DB;种转账金额类型。

<figure><img src="../../../.gitbook/assets/image (741).png" alt=""><figcaption></figcaption></figure>

1. **逐一输入**\
   在输入框中，逐一输入转账金额数量。
2. **全部**\
   点击转账数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「全部」**&#x9009;项，目标代币将全部转账到归集地址。

<figure><img src="../../../.gitbook/assets/image (742).png" alt=""><figcaption></figcaption></figure>

3. **输入金额**\
   点击转账数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**」**&#x9879;，输入金额范围，所有地址将接收到指定范围内数额。
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

系统将根据收款地址数量自动分组，每组最多 5 个收款地址。

<figure><img src="../../../.gitbook/assets/image (730).png" alt=""><figcaption></figcaption></figure>

1. **RPC 发送**\
   通过 RPC 节点统一广播转账交易，无需支付 Jito 小费，各笔交易不保证按提交顺序执行。
2. **Jito Bundle**\
   每包最多 25 个收款地址（5 组），通过 Jito 小费提升上链优先级并按顺序执行。
{% endstep %}

{% step %}
### 核实信息

点&#x51FB;**「下一步」**&#x8FDB;入确认页面，核对收款地址及数量、转账总额和预估费用，确认无误后再提交转账。

<figure><img src="../../../.gitbook/assets/image (731).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下方「**确认并发送**」按钮，您可以实时查看转账程序完成情况，并等待转账程序完成，。

<figure><img src="../../../.gitbook/assets/image (732).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (256).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择转账代币

可以选择 SOL，也可以选择当前钱包拥有的代币进行转账。

<figure><img src="../../../.gitbook/assets/image (258).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入转账钱包私钥

{% hint style="danger" %}
**「多对一转账」**&#x529F;能仅支持私钥导入以进行转账操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入转账地址私钥的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「手动输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (260).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (320).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包私钥，**&#x4E00;行仅输入一个私钥，按回车键换行

<figure><img src="../../../.gitbook/assets/image (263).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (264).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 点&#x51FB;**「上传文件」**&#x6309;钮，弹出文件上传窗口。

<figure><img src="../../../.gitbook/assets/image (262).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (251).png" alt=""><figcaption></figcaption></figure>

2. 导入钱包私钥信息文件，显示私钥信息。\
   请通过 CiaoTool 模板文件导入，以确保私钥准确导入。

{% file src="../../../.gitbook/assets/Solana_privateKey_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (247).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (264).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入转账金额

点击归集数量上方&#x7684;**「设置」**&#x6309;&#x94AE;**，**&#x652F;&#x6301;**「全部」「归集数量」**&#x548C;**「保留数量」**&#x4E09;种转账金额类型。

1. **全部**\
   无需额外操作，方便快捷将钱包所有该代币归集到同一地址
2. **归集数量**\
   统一全部待归集钱包的转账金额数量
3. **保留数量**\
   确保每个钱包有固定留存，以便后续继续使用
{% endstep %}

{% step %}
### 输入支付钱包私钥

导入私钥，该次使用功能的手续费将由该钱包支付。

<figure><img src="../../../.gitbook/assets/image (265).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入接收钱包地址

指定归集接收地址，输入钱包地址或选定当前绑定钱包

<figure><img src="../../../.gitbook/assets/image (266).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下方「**确认转账**」按钮，并等待转账程序完成。
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>什么是多对一批量转账？</strong></summary>

多对一批量归集指将多个钱包地址中持有的代币统一转入一个主地址，**便于集中管理资产、统一调配资金**。

</details>

<details>

<summary><strong>如何导入接收地址？</strong></summary>

你可以手动输入地址，也可以上传 CSV 文件导入目标地址列表，系统会自动识别并展示预览。

</details>

<details>

<summary><strong>操作是否安全？</strong></summary>

平台采用纯前端签名机制，您的私钥绝不会被上传或储存在任何服务器上，所有交易均在本地浏览器完成签名，从技术层面确保平台无法访问您的私钥。

</details>

<details>

<summary><strong>一次可以多少个地址转账？</strong></summary>

得益于私钥导入的模式，多对一转账功能免除了逐一钱包签署的繁复工作，发送地址没有任何数量限制。

</details>

<details>

<summary><strong>可以同时转多种代币吗？</strong></summary>

当前版本支持选择单一 SPL 代币或 SOL 进行批量转账；如需多种资产归集，可多次执行操作。

</details>

**💬 如遇到问题？加入社群实时咨询**：[https://t.me/ciaotool](https://t.me/ciaotool)

* **Email**：[support@ciaotool.io](mailto:support@ciaotool.io)
* **官网**：[https://ciaotool.io](https://ciaotool.io/)
* **X（Twitter）**：[https://x.com/CiaoTool](https://x.com/CiaoTool)
* **Medium**： [https://medium.com/@ciaotool](https://medium.com/@ciaotool)
* **Blog**：[https://www.ciaoailiquidity.com/zh/blog](https://www.ciaoailiquidity.com/zh/blog)
* **YouTube**：[https://www.youtube.com/@CiaoTool](https://www.youtube.com/@CiaoTool)
* **WhatsApp**：[https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J](https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J)

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
