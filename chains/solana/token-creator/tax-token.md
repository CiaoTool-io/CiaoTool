---
description: >-
  Solana 一键发币工具，快速创建具有税费功能的 Token-2022 代币，通过纯前端安全处理，助力 Web3
  开发者与链上运营者以极低成本快速发行代币，并无缝衔接后续的流动性管理与多地址资产调度。
---

# Solana - 税费代币创建教程

{% hint style="info" %}
当前&#x662F;**「Solana - 税费代币创建」**&#x6559;程页面，点击[**「Solana - 标准代币创建」**](standard-token.md)以查看标准代币创建教程。
{% endhint %}

## CiaoTool Solana 税费代币创建是什么？

<figure><img src="../../../.gitbook/assets/image (647).png" alt="CiaoTool Solana网络 创建税费代币 功能页面"><figcaption></figcaption></figure>

传统 Solana 标准代币（SPL Token）主要用于基础的转账与流通，而 Solana 税费代币创建 则是基于 Solana 官方最新的 Token-2022 扩展协议 实现的高阶资产发行功能。

通过 CiaoTool 的一键创建工具，项目方可以在无需编写任何智能合约代码的情况下，直接在底层协议级别为代币设定“转账/交易税率”以及“单笔最高税费上限”。这意味着代币在每一次链上流转时，都会自动扣除一定比例的费用并存入项目方指定的“收税钱包”中，并可设置或放弃代币权限（如增发、冻结）。发行方可以一键生成具备 Solana 极高并发处理能力与极低网络手续费特性的专属代币。

**适用场景：**

* 社区金库与生态建设基金 \
  将收取到的代币税费自动流入项目多签金库，用于长期的研发、市场营销与生态贡献者奖励，确保项目拥有持续的造血能力。
* 构建通缩经济模型：\
  项目方可通过定期销毁收取的税费代币，实现流通量的持续减少，从而优化代币的稀缺性与长期价值支撑。
* 项目专属机制创新：\
  支持设置复杂的授权机制，包括权限委托与利息设定等高级配置，为 SocialFi 或特定实用型代币提供更灵活的机制与市场策略。

立即在 Solana 网络上，用 CiaoTool​ 创建税费代币：

{% embed url="https://ciaotool.io/zh-CN/token/tax-token" %}

***

## 为什么选择 CiaoTool Solana 税费代币创建？

在快节奏的 Solana 生态中，效率与后续配套设施决定了项目的起跑线。CiaoTool 为发行方构筑了极具竞争力的基础设施：

* **极高安全性：** \
  CiaoTool 采用纯前端本地执行，私钥不触网，合约代码开源透明，保障创建者的绝对控制权。
* **零代码极速创建：**\
  彻底免去编写与调试复杂智能合约的繁琐流程，全前端表单化操作，一键支付 Gas 费即可实现链上资产的极速诞生，将技术门槛降至为零。
* **极致的前端安全隔离：** \
  采用前端本地化处理机制，确保发币过程中的权限控制与私钥安全，从技术底层杜绝中心化存储带来的资产风险。
* **全矩阵生态闭环：**\
  完美衔接 CiaoTool 强大的市值管理（MM）与流动性管理工具，帮助项目从“创建”平稳过渡到“运营”，完美适配从资产生成到生态繁荣的全生命周期战略。

***

## **视频教程 | Solana 税费代币创建**

{% hint style="info" %}
如果你更偏好视频形式的学习，该功能页面与 税费代币 页面结构类似，参考并观看本教程
{% endhint %}

{% embed url="https://www.youtube.com/watch?v=FtfJagh1u2s" %}

***

## **图文指南 | Solana 税费代币创建**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 Solana 网络的钱包

<figure><img src="../../../.gitbook/assets/image (622).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 填写代币基础信息

<figure><img src="../../../.gitbook/assets/image (643).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**克隆：** 点击克隆按钮，克隆其他代币的信息。
{% endhint %}

* **代币名称：**&#x60A8;希望展示在钱包或区块浏览器中的完整代币名称（_例如：MyFirstToken_）。
* **代币简称：**&#x4EE3;币的缩写，通常为 3\~6 个大写字母（_例如：MYT_）。
* **精度：**&#x6307;的是一种代币最小可以分割到的小数位数。简单来说，它决定了你可以将一枚代币分成多小的单位。常见为 18 位。
* **总供应量：**&#x53D1;行的代币总量。
* **LOGO：**&#x4E0A;传项目或代币的标志图像，建议尺寸 1000\*1000 像素。
* **描述：** 简要介绍代币用途、故事或 Meme 背景（选填）。
* **添加社交链接**：虽然为可选项，但强烈建议填写，**官网、X / Twitter、Telegram。**
{% endstep %}

{% step %}
### 税费设置

<figure><img src="../../../.gitbook/assets/image (648).png" alt=""><figcaption></figcaption></figure>

* **费率：**&#x6BCF;次交易或转账所需的手续费率，单位为百分比。
* **最高费用：**&#x5355;笔转账或交易时的最大手续费用上限。
* **权限钱包地址：**&#x9ED8;认为当前连接的钱包地址，控制此代币的所有权限。
* **提现钱包地址：**&#x4EE3;币所产生的手续费，有权限进行提现的地址，默认为当前连接的钱包地址。
{% endstep %}

{% step %}
### 设置权限

**元数据修改权**：“放弃元数据修改权”，意味着您将无法修改令牌元数据，让投资者感到更安全确实很有用。

**冻结权**：“放弃冻结权”，意味着您无法限制特定帐户执行发送交易等操作，CiaoTool 支持未放弃此权限的代币创建市场。

**铸币权**：“放弃铸币权”对于让投资者感到更加安全和作为代币的成功是必要的。如果您放弃铸币权，则意味着您将无法铸造更多代币供应。

<figure><img src="../../../.gitbook/assets/image (645).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下&#x65B9;**「创建代币」**&#x6309;钮，并等待合约创建完成。

<figure><img src="../../../.gitbook/assets/image (646).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 创建流动性池

代币创建完成后，还不具有交易属性，只能进行转账操作。添加流动性资金池，让代币在去中心化平台自由兑换。

点击前往 Raydium 创建流动性资金池：

{% embed url="https://raydium.io/liquidity-pools/" %}
{% endstep %}
{% endstepper %}

***

## **更多快捷工具 & 指南**

{% columns %}
{% column %}
{% content-ref url="tax-fee-claim.md" %}
[tax-fee-claim.md](tax-fee-claim.md)
{% endcontent-ref %}
{% endcolumn %}

{% column %}
{% content-ref url="../multisender/one-to-many-old.md" %}
[one-to-many-old.md](../multisender/one-to-many-old.md)
{% endcontent-ref %}
{% endcolumn %}
{% endcolumns %}

## **常见问题 FAQ**

<details>

<summary><strong>手续费是交易的时候出，还是转账的时候出？</strong></summary>

转账和交易，都会产生手续费，且无法更改。Solana不像BSC那样，可以设置某些场景。

</details>

<details>

<summary><strong>手续费可以是 USDT 或者 SOL 吗？</strong></summary>

不行，Token-2022 标准的手续费，只能是项目代币（您创建的代币）。

</details>

<details>

<summary><strong>创建代币的地址是白名单吗？转账或交易没有税费吗？</strong></summary>

Solana 代币没有白名单功能，所有地址转账与交易都会产生手续费，权限地址也不例外。

</details>

<details>

<summary><strong>手续费是发起转账的地址出，还是接收地址出？</strong></summary>

用户发起转账1000枚代币，假设10%的税率，接受者到账是900枚。

</details>

<details>

<summary><strong>发币后还能修改参数吗？</strong></summary>

没有放弃元数据修改权前，您可以自由地修改代币参数。若放弃元数据修改权限，不能再修改数据，您必须重新创建代币。

</details>

<details>

<summary><strong>代币名称和代币简称能使用中文吗？</strong></summary>

可以，现在 Solana 链全面支持中文、英文以及中英混合文字。

</details>

<details>

<summary><strong>操作是否安全？</strong></summary>

平台采用纯前端签名机制，您的私钥绝不会被上传或储存在任何服务器上，所有交易均在本地浏览器完成签名，从技术层面确保平台无法访问您的私钥。

</details>

***

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
