---
description: 批量处理多个钱包地址 SOL 或 SPL 代币的资金转账，模拟真实转账，有效打乱地址关联，优化气泡图检测，提升多地址资金管理效率，丰富您的资产管理策略。
---

# Solana - 批量转账 | 多对多转账教程

{% hint style="info" %}
当前&#x662F;**「Solana 多对多转账」**&#x6559;程页面，点击[**「EVM - 多对多转账」**](../../../tools/multisender/multi-to-multi/many-to-many.md)以查看 BSC、opBNB、Base、X Layer、IoTeX、BOT 等 EVM 网络多对多转账教程
{% endhint %}

## CiaoTool Solana 多对多转账是什么？

**CiaoTool Solana 多对多转账**是一款专为 Web3 高效资产管理打造的高阶工具。它允许您在一次操作中，自动从多个发送钱包将 SOL 或任意 SPL 代币批量转入多个接收钱包。

相较于传统的单地址发币，多对多转账的核心优势在于完全模拟真实用户的独立转账行为。系统会自动拆分并执行点对点的独立交易，有效打乱资金的流转路径，切断链上追踪工具的关联分析。这不仅能大幅节省批量操作的时间、降低手动执行的错误率，还能有效防止钱包地址被追踪。

此工具尤其适用于：

* 防追踪的代币空投及分发
* 隐匿的链上资金调拨与分散换仓
* 高效的社区多地址批量付款
* Web3 增长活动的复杂资金管理

立即在 Solana 上，用 CiaoTool​ 批量转账功能进行多对多转账操作：

{% embed url="https://ciaotool.io/zh-CN/transfer/many-to-many" %}

***

## 为什么选择 CiaoTool 多对多转账？

**CiaoTool** 提供了一种在 Solana 上高效、隐秘管理链上资产的顶级方案。无论您是需要进行高隐匿性的代币分发、做市筹码的安全换仓，还是执行复杂的节点资金调拨，其多对多转账功能都能通过模拟真实的独立交易，确保操作的准确性并完美切断链上关联。

全面支持 SOL 和各类 SPL 代币，结合一键文件导入与智能自动批处理引擎，它不仅极大解放了运营双手，更是任何在 Solana 上深耕的 Web3 项目和专业团队不可或缺的增长与资管利器。

***

## **图文指南 | Solana 批量转账 - 多对多转账**&#x20;

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
**「多对多转账」**&#x529F;能仅支持私钥导入以进行转账操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

{% hint style="info" %}
转出钱包数量需要和接收钱包数量保持一致
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入转账地址私钥的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「手动输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (267).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (310).png" alt=""><figcaption></figcaption></figure>

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

<figure><img src="../../../.gitbook/assets/image (247).png" alt=""><figcaption></figcaption></figure>

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
1. 点&#x51FB;**「上传文件」**&#x6309;钮，弹出文件上传窗口。

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
### 确认交易

确认信息无误后，点击下方「**确认转账**」按钮，并等待转账程序完成。
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

你可以手动输入地址，也可以上传 CSV 文件导入目标地址列表（支持地址+金额格式），系统会自动识别并展示预览。

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
