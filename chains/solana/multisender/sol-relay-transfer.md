---
description: 通过独立中间地址处理 SOL 的资金转移，切断首尾直接联系，有效打断资金关联，优化气泡图呈现，提升多钱包资金调拨安全性，打造深度隐匿的资产管理策略。
---

# Solana - 批量转账 | 中转转账教程

{% hint style="info" %}
当前&#x662F;**「Solana 中转转账」**&#x6559;程页面，点击[**「BSC - 中转转账」**](../../bsc/multisender/relay-transfer.md)以查看 BSC 网络多对多转账教程。
{% endhint %}

## CiaoTool Solana 中转转账是什么？

**CiaoTool Solana 中转转账**是一款专注于链上隐私保护与资金隐匿的高阶工具。它允许您在转账过程中自动引入独立的中间钱包节点，将 SOL（原生代币） 智能中转并批量分发至目标钱包。\
​\
相较于普通的直接转账，中转转账的核心优势在于切断发送端与接收端之间的直接链上联系。系统通过中间地址自动处理资金流转，完美模拟真实独立交互行为，有效打乱资金流转路径，优化气泡图等链上工具的聚类分析与追踪显示。这不仅能隐藏资金的动向，保护主钱包安全隐私，保障多钱包交互的安全流转。

此工具尤其适用于： ​ ​

* 隐私保护下的 SOL 资金调拨与分仓策略
* 优化链上气泡图与聚类分析显示
* 安全的多地址资产分布管理

立即在 Solana 上，用 CiaoTool​ 批量转账功能进行中转转账操作：

{% embed url="https://ciaotool.io/zh-CN/transfer/relay-transfer" %}

***

## 为什么选择 CiaoTool 中转转账？

**CiaoTool** 提供了一种在 Solana 上高效、安全管理链上资产的专业方案。无论您是需要进行注重隐私的 SOL 资金分发、多钱包的安全换仓，还是执行复杂的节点资金调拨，其中转转账功能都能通过引入中间节点并模拟真实的独立交易，确保操作的准确性，有效分散资金流转路径并优化链上关联显示。

专为 **SOL** 资产流转打造，结合一键文件导入与批量处理，它不仅极大解放了运营双手，更是任何在 Solana 上深耕的 Web3 项目和专业团队不可或缺的安全资管利器。

***

## **图文指南 | Solana 批量转账 - 中转转账**&#x20;

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (256).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择转账代币

可以选择 SOL，也可以选择当前钱包拥有的代币进行转账。

<figure><img src="../../../.gitbook/assets/image (243).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入转账钱包私钥

{% hint style="danger" %}
**「中转转账」**&#x529F;能仅支持私钥导入以进行转账操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

{% hint style="info" %}
转出钱包数量需要和接收钱包数量保持一致
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入转账地址私钥的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「手动输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (267).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (245).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包私钥，**&#x4E00;行仅输入一个私钥，按回车键换行

<figure><img src="../../../.gitbook/assets/image (263).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (270).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 点&#x51FB;**「上传文件」**&#x6309;钮，弹出文件上传窗口。

<figure><img src="../../../.gitbook/assets/image (268).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (251).png" alt=""><figcaption></figcaption></figure>

2. 导入钱包私钥信息文件，显示私钥信息\
   请通过 CiaoTool 模板文件导入，以确保私钥准确导入。

{% file src="../../../.gitbook/assets/Solana_privateKey_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (318).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (269).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入转账金额

点击转账数量上方&#x7684;**「统一输入」**&#x6309;&#x94AE;**，**&#x652F;&#x6301;**「金额」「百分比」「保留数量」**&#x548C;**「全部」四**种转账金额类型。

1. **金额**\
   统一所有钱包指定金额进行转账
2. **百分比**\
   统一设定余额百分比，每个钱包根据百分比数量进行转账
3. **保留数量**\
   确保每个钱包有固定留存，以便后续继续使用，其余金额转入接收钱包地址
4. **全部**\
   无需额外操作，方便快捷将钱包所有该代币转账到接收地址
{% endstep %}

{% step %}
### 导入接收钱包地址

{% hint style="info" %}
接收钱包数量需要和转出钱包数量保持一致
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入接收地址的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「手动输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (312).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (245).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x4E00;行仅输入一个地址，按回车键换行

<figure><img src="../../../.gitbook/assets/image (247).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (313).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
* 点&#x51FB;**「上传文件」**&#x6309;钮，弹出文件上传窗口。

<figure><img src="../../../.gitbook/assets/image (314).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (251).png" alt=""><figcaption></figcaption></figure>

2. 导入钱包地址信息文件，显示地址信息\
   请通过 CiaoTool 模板文件导入，以确保钱包地址准确导入。

{% file src="../../../.gitbook/assets/Solana_address_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (247).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (313).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 设置中转数量

自定义中转地址数量，所有转账均会经过数个地址到达指定接收钱包
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下方「**确认转账**」按钮，并等待转账程序完成。
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

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
