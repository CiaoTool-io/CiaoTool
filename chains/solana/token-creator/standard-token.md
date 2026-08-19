---
description: >-
  Solana 一键发币工具，快速创建 SPL 代币，通过纯前端安全处理，助力 Web3
  开发者与链上运营者以极低成本快速发行代币，并无缝衔接后续的流动性管理与多地址资产调度。
---

# Solana - 标准代币创建教程

{% hint style="info" %}
当前&#x662F;**「Solana - 标准代币创建」**&#x6559;程页面以查看标准代币创建教程。

点击[**「EVM - 标准代币创建」**](../../../tools/token-creator/contract-token-creator/standard-token-evm.md)查看 **BSC、Base、X Layer、IoTeX、BOT** 等 EVM 网络教程。
{% endhint %}

## CiaoTool Solana 标准代币创建是什么？

<figure><img src="../../../.gitbook/assets/image (641).png" alt=""><figcaption></figcaption></figure>

Solana 标准代币创建 是指在 Solana 区块链网络上，部署并发行原生数字资产的过程。CiaoTool 提供了完全无代码的代币创建开发工具。通过智能合约的自动化打包与前端可视化部署，并可设置或放弃代币权限（如增发、冻结）。发行方可以一键生成具备 Solana 极高并发处理能力与极低网络手续费特性的专属代币。

**适用场景：**

* Meme 发币：快速跟随热点叙事，抢占市场流量
* 社区积分系统：用于任务激励、DAO 治理或用户奖励
* 交易测试资产：用于机器人策略、套利或脚本测试
* 项目预发行 Token：为后续 IDO 或流动性部署做准备
* 克隆盘玩法：复制热门代币结构，快速参与市场博弈

立即在 Solana 网络上，用 CiaoTool​ 创建标准代币：

{% embed url="https://ciaotool.io/zh-CN/token/create-token" %}

***

## 为什么选择 CiaoTool Solana 标准代币创建？

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

## **视频教程 | Solana 标准代币创建**

{% embed url="https://www.youtube.com/watch?v=FtfJagh1u2s" %}

***

## **图文指南 | Solana 标准代币创建**

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
* **精度：**&#x6307;的是一种代币最小可以分割到的小数位数。简单来说，它决定了你可以将一枚代币分成多小的单位。常见为 6 / 9 位。
* **总供应量：**&#x53D1;行的代币总量。
* **LOGO：**&#x4E0A;传项目或代币的标志图像，建议尺寸 1000\*1000 像素。
* **描述：** 简要介绍代币用途、故事或 Meme 背景（选填）。
* **添加社交链接**：虽然为可选项，但强烈建议填写，**官网、X / Twitter、Telegram。**
{% endstep %}

{% step %}
### 自定义服务

#### 自定义合约地址

<figure><img src="../../../.gitbook/assets/image (644).png" alt=""><figcaption></figcaption></figure>

打造你的个性化代币地址，设置代币地址，**额外收费 0.01 SOL。**

1. **以「pump」结尾：**
   * 代币地址以「pump」结尾
2. **自定义代币地址**
   * 提前生成您想要的钱包地址，可以是靓号地址。
   * 将你提前生成的私钥粘贴导入（**地址必须要全新地址且没有付过SOL租金**）；
   * 系统将使用该地址部署你的代币，确保合约地址与预期一致。
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

## **常见问题 FAQ**

<details>

<summary><strong>我可以创建多个代币吗？</strong></summary>

当然可以，每次创建都是独立的代币合约，互不影响。

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
