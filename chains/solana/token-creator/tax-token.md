---
description: >-
  Solana 一键发币工具，快速创建具有税费功能的 Token-2022 代币，通过纯前端安全处理，助力 Web3
  开发者与链上运营者以极低成本快速发行代币，并无缝衔接后续的流动性管理与多地址资产调度。
---

# Solana - 税费代币创建教程

{% hint style="info" %}
当前&#x662F;**「Solana - 税费代币创建」**&#x6559;程页面，点击[**「Solana - 标准代币创建」**](standard-token.md)以查看标准代币创建教程。
{% endhint %}

## 功能介绍

CiaoTool 提供基于 Solana Token-2022 协议的零代码税费代币创建工具。用户可设置转账费率、单笔最高费用，以及增发、冻结和税费管理权限，快速完成代币发行。

代币交易及转账时，协议会自动扣取费用；被扣费用先记录在接收方代币账户中，再由税费提取权限方归集至指定账户，并非每次转账后立即进入收税钱包。[Solana 官方说明](https://solana.com/docs/tokens/extensions/transfer-fees)

**适用场景：**

* **社区金库：** 将归集的税费投入研发、运营和社区激励
* **通缩机制：** 定期销毁归集代币，减少流通供应量
* **收益分配：** 为特定代币设计可持续的费用分配机制
* **机制创新：** 结合兼容的 Token-2022 扩展，构建更多应用场景

立即在 Solana 网络上，用 CiaoTool​ 创建税费代币：

{% embed url="https://ciaotool.io/zh-Hans/token/tax-token" %}

***

## 核心优势

* **安全可控：** 交易在前端构建并由钱包签名，私钥无需上传，代币及税费权限由创建者自主设置。
* **零代码创建：** 通过可视化界面配置税率、单笔税费上限等参数，无需编写智能合约。
* **协议级执行：** 基于 Token-2022 转账费扩展，由链上协议自动计算并扣取费用。
* **配套完善：** 可衔接 CiaoTool 的税费管理、流动性及市值管理工具，满足代币从创建到运营的需求。

***

## **视频教程**

{% hint style="info" %}
如果你更偏好视频形式的学习，该功能页面与 税费代币 页面结构类似，参考并观看本教程
{% endhint %}

{% embed url="https://www.youtube.com/watch?v=FtfJagh1u2s" %}

***

## **图文指南**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角【连接钱包】按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (747).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 填写代币信息

<figure><img src="../../../.gitbook/assets/image (815).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**克隆：** 点击克隆按钮，克隆其他代币的信息。
{% endhint %}

* **代币名称：**&#x60A8;希望展示在钱包或区块浏览器中的完整代币名称（_例如：MyFirstToken_）。
* **代币简称：**&#x4EE3;币的缩写，通常为 3\~6 个大写字母（_例如：MYT_）。
* **精度：**&#x6307;的是一种代币最小可以分割到的小数位数。简单来说，它决定了你可以将一枚代币分成多小的单位。常见为 6 / 9 位。
* **总供应量：**&#x53D1;行的代币总量。
* **LOGO：**&#x4E0A;传项目或代币的标志图像，建议尺寸 1000\*1000 像素。
* **描述：** 简要介绍代币用途、故事或 Meme 背景（选填）。
* **添加社交链接**：虽然为可选项，但强烈建议填写，**官网、X / Twitter、Telegram。**
{% endstep %}

{% step %}
### 税费配置

<figure><img src="../../../.gitbook/assets/image (822).png" alt=""><figcaption></figcaption></figure>

* **费率：**&#x6BCF;次交易或转账所需的手续费率，单位为百分比。
* **最高费用：**&#x5355;笔转账或交易时的最大手续费用上限。
* **税费权限地址：**&#x9ED8;认为当前连接的钱包地址，控制此代币的所有权限。
* **提取税费地址：**&#x4EE3;币所产生的手续费，有权限进行提现的地址，默认为当前连接的钱包地址。
{% endstep %}

{% step %}
### 添加链接<mark style="color:$info;">（可选）</mark>

虽然为可选项，但强烈建议填写，**官网、X / Twitter、Telegram。Discord**，增加项目可信度。

<figure><img src="../../../.gitbook/assets/image (816).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Mint 地址<mark style="color:$info;">（可选）</mark>

生成自定义代币地址，提升代币辨识度。

{% tabs %}
{% tab title="靓号地址" %}
可以设置希望出现在钱包地址开头或结尾的字符，例如以 `soL` 开头、以 `pump` 结尾，工具会持续生成随机密钥对，直到找到符合条件的地址。

<figure><img src="../../../.gitbook/assets/image (817).png" alt=""><figcaption></figcaption></figure>

详细工作原理及教程请查看

{% content-ref url="../wallet-tool/vanity-address.md" %}
[vanity-address.md](../wallet-tool/vanity-address.md)
{% endcontent-ref %}
{% endtab %}

{% tab title="自定义地址" %}
* 提前生成您想要的钱包地址，可以是靓号地址。
* 将你提前生成的私钥粘贴导入（**地址必须要全新地址且没有付过SOL租金**）；
* 系统将使用该地址部署你的代币，确保合约地址与预期一致。
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 权限设置

关闭权限意味着您无法再编辑代币数据，但这会大大提升交易者信心。放弃权限不可恢复，请确认所有信息准确无误且无需再调整后关闭。

<figure><img src="../../../.gitbook/assets/image (818).png" alt=""><figcaption></figcaption></figure>

**元数据修改权**：“放弃元数据修改权”，意味着您将无法修改令牌元数据，让投资者感到更安全确实很有用。

**冻结权**：“放弃冻结权”，意味着您无法限制特定帐户执行发送交易等操作，CiaoTool 支持未放弃此权限的代币创建市场。

**铸币权**：“放弃铸币权”对于让投资者感到更加安全和作为代币的成功是必要的。如果您放弃铸币权，则意味着您将无法铸造更多代币供应。
{% endstep %}

{% step %}
### Jito 小费

通过 Jito 小费提升上链优先级并按顺序执行。
{% endstep %}

{% step %}
### 确认交易

<figure><img src="../../../.gitbook/assets/image (819).png" alt=""><figcaption></figcaption></figure>

确认信息无误后，点击下&#x65B9;**「创建 Token」**&#x6309;钮，您可以实时查看程序完成情况，并等待创建程序完成。

<figure><img src="../../../.gitbook/assets/image (820).png" alt=""><figcaption></figcaption></figure>
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
{% content-ref url="../multisender/one-to-many.md" %}
[one-to-many.md](../multisender/one-to-many.md)
{% endcontent-ref %}
{% endcolumn %}
{% endcolumns %}

## **常见问题**

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

## **寻求支持**

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
