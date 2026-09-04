---
description: 一对多转账是一种高效便捷的代币分发工具，支持将同一钱包中的 SOL 或 SPL 代币批量发送至无限个接收地址，适用于空投、奖励发放和批量结算等场景。
hidden: true
---

# Solana - 批量转账 | 一对多转账教程

{% hint style="info" %}
当前&#x662F;**「Solana - 一对多转账」**&#x6559;程页面，点击[**「EVM - 一对多转账」**](../../../tools/multisender/one-to-multi/one-to-many.md)以查看 BSC、opBNB、Base、X Layer、IoTeX、BOT、Robinhood Chain 等 EVM 网络一对多转账教程
{% endhint %}

## CiaoTool Solana 一对多转账是什么？ <a href="#definition" id="definition"></a>

<figure><picture><source srcset="../../../.gitbook/assets/屏幕截图 2026-09-04 142205.png" media="(prefers-color-scheme: dark)"><img src="../../../.gitbook/assets/image (711).png" alt="CiaoTool BSC 批量转账 一对多转账页面"></picture><figcaption></figcaption></figure>

**CiaoTool Solana 一对多转账**是一款高效链上资产分发工具。它允许用户突破传统单笔转账的限制，全自动调度将单个主钱包中的 **SOL（原生代币）**&#x6216;**任何 SPL 代币**，在同一次操作中批量发送至数百个不同的接收地址。

相较于「逐笔复制地址、手动签名转账」的传统模式，该功能的核心机制在于「底层批量指令聚合」。系统会将海量的独立转账指令通过智能合约整合为一个不可分割的数据包提交至链上。这种机制不仅将原本需要耗费数小时的机械性工作缩短至一键秒级完成，更通过合并同类项大幅平摊了整体的网络矿工费，是项目方进行空投分发、团队结算或做市前置分仓的核心基建。

此工具尤其适用于：

* 空投和代币分发
* DAO收益和奖励
* 向用户批量付款
* 营销活动和Web3增长策略

立即在 Solana 上，用 CiaoTool​ 批量转账功能进行一对多转账操作：

{% embed url="https://ciaotool.io/zh-hans/transfer/one-to-many" %}

***

## 为什么选择 CiaoTool 代币空投（一对多转账）？ <a href="#advantage" id="advantage"></a>



**百倍提升效率：** 彻底免去人工频繁切换账号、复制粘贴地址与重复授权签名的繁琐流程，支持一键并发执行成百上千笔转账，实现链上资产的极速流转。 ​

**极致削减成本：** 通过底层智能合约的多重调用与批量打包技术，将多笔转账聚合为单次链上交互，最大程度摊薄网络费用，显著降低大规模分发的资金损耗。 ​

**灵活的矩阵配置：** 支持通过 Excel 电子表格文件一键批量导入目标地址列表与对应的分发额度。支持自定义等额、定额或随机金额分配，完美适配复杂多变的空投策略与持币分布需求。 ​

**本地安全环境：** 采用纯前端本地执行机制，私钥仅在本地环境中用于交易签名，在极速提升交易效率的同时，全方位保障多钱包资产的绝对安全。

**CiaoTool** 提供了一种在 Solana 上分发代币最快捷、最可靠的方式。无论您是发行新代币、进行空投还是管理支付，其批量转账功能都能确保准确性、可扩展性和流畅的用户体验。

它支持 **SOL 和 SPL 代币**、文件导入和自动批处理，是任何在 Solana 上运行的 Web3 项目必不可少的工具。

***

## 视频教程 | Solana 批量转账 - 一对多转账 <a href="#video-guide" id="video-guide"></a>

{% embed url="https://www.youtube.com/watch?v=vD431lBM3cU" %}

***

## **图文指南 | Solana 批量转账 - 一对多转账**  <a href="#solana-one-to-multi-guide" id="solana-one-to-multi-guide"></a>

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (240).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入转账钱包私钥

{% hint style="danger" %}
当&#x524D;**「一对多转账」**&#x529F;能仅支持 私钥导入以进行转账操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

导入私钥，系统自动刷新 SOL 余额与 Token 余额，请保证钱包中有充足的 SOL。

<figure><img src="../../../.gitbook/assets/image (242).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择转账代币

可以选择 SOL，也可以选择当前钱包拥有的代币进行转账。

<figure><img src="../../../.gitbook/assets/image (243).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入接收地址

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入接收地址的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「手动输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (244).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (245).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x4E00;行仅输入一个地址，按回车键换行

<figure><img src="../../../.gitbook/assets/image (247).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (248).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 点&#x51FB;**「上传文件」**&#x6309;钮，弹出文件上传窗口。

<figure><img src="../../../.gitbook/assets/image (250).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (251).png" alt=""><figcaption></figcaption></figure>

2. 使用 CiaoTool 模板文件导入，并保存确定导入并显示在输入框内。\
   点击下载并查看模板：

{% file src="../../../.gitbook/assets/Solana_address_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (247).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (249).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入转账金额

支&#x6301;**「逐一输入」「统一金额」**&#x548C;**「随机范围」**&#x4E09;种转账金额类型。

1. **逐一输入**\
   在输入框中，逐一输入转账金额数量

<figure><img src="../../../.gitbook/assets/image (252).png" alt=""><figcaption></figcaption></figure>

2. **统一金额**\
   点击转账数量上方&#x7684;**「统一输入」**&#x6309;&#x94AE;**，**&#x9009;&#x62E9;**「金额」**&#x9009;项，输入金额数量，所有地址将统一转账数量

<figure><img src="../../../.gitbook/assets/image (253).png" alt=""><figcaption></figcaption></figure>

3. **随机范围**\
   点击转账数量上方&#x7684;**「统一输入」**&#x6309;&#x94AE;**，**&#x9009;&#x62E9;**「随机范围」**&#x9009;项，输入金额范围，所有地址将接收到指定范围内数额。

<figure><img src="../../../.gitbook/assets/image (259).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 慢速转账设置

{% hint style="warning" %}
&#x4EC5;**「慢速一转多功能」**&#x9002;配，可设置任务执行间隔时间
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (255).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下方「**确认转账**」按钮，并等待转账程序完成。
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>什么是一对多批量转账？</strong></summary>

一对多批量转账是指从一个钱包地址，向多个目标地址**同时发送代币**的操作，常用于空投、奖励发放、资产分发等场景。

</details>

<details>

<summary><strong>如何导入接收地址？</strong></summary>

你可以手动输入地址，也可以上传 CSV 文件导入目标地址列表（支持地址+金额格式），系统会自动识别并展示预览。

</details>

<details>

<summary><strong>是否支持不同地址转不同数量？</strong></summary>

可以。你可以为每个地址设置不同的转账数量，也可以设置统一的金额和随机金额区间分发给所有目标地址。

</details>

<details>

<summary><strong>操作是否安全？</strong></summary>

平台采用纯前端签名机制，您的私钥绝不会被上传或储存在任何服务器上，所有交易均在本地浏览器完成签名，从技术层面确保平台无法访问您的私钥。

</details>

<details>

<summary><strong>一次可以发送到多少个地址？</strong></summary>

得益于私钥导入的模式，一对多转账功能免除了逐一钱包签署的繁复工作，接收地址没有任何数量限制。

</details>

<details>

<summary><strong>可以同时转多种代币吗？</strong></summary>

当前版本支持选择单一 SPL 代币或 SOL 进行批量转账；如需多种资产分发，可多次执行操作。

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
