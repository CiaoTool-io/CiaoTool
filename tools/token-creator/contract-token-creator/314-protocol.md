---
description: >-
  CiaoTool 提供免代码的 BSC ERC-314 协议代币智能合约部署服务。转账及买卖，让你轻松发行创新玩法代币，无需 Swap
  即可兑换，内置交易冷却机制防夹子，席卷全球潮流。
metaLinks:
  alternates:
    - https://app.gitbook.com/s/b56FKZGe1viFi67H1pPQ/token/314-protocol
---

# BSC - 314 协议代币创建教程

{% hint style="danger" %}
<mark style="color:red;">**检测风险提醒**</mark>

该类型代币由于采用特殊机制或扩展功能，部分安全检测平台可能会标记为**存在潜在风险或给予较低评分**。若您较为关注代币检测结果，建议选择[**「创建标准代币」**](standard-token-evm.md)，标准代币通常具有更好的兼容性与检测表现。继续创建此类型代币，**即表示您已了解并接受可能产生的检测提示或风险标记。**
{% endhint %}

## 314 协议代币是什么？

<figure><img src="../../../.gitbook/assets/image (538).png" alt="CIaoTool BSC 314协议代币创建页面"><figcaption></figcaption></figure>

{% hint style="warning" %}
314 协议尚处于实验阶段，可能存在未知风险。权限功能重要，请确认无误后再丢弃。
{% endhint %}

314 协议是一种新的实验性代币标准，该协议旨在降低用户交易时高昂的交易费用与繁琐的授权流程。和传统的 Swap 不同，314 协议实现了「转账即交易」的新型功效。

* **买币**：用户将 BNB 转入合约地址，即可获得代币。
* **卖币**：用户将代币转入合约地址，即可获得 BNB。
* **交易冷却**：设定时间内，全市场仅允许一笔买单，每个地址仅允许一笔卖单。

立即在 BSC 网络上，用 CiaoTool​ 创建 314 协议代币：

{% embed url="https://bsc.ciaotool.io/zh-Hans/token/314-protocol" %}

***

## 为什么选择 CiaoTool BSC 314 协议代币创建？

对于追求技术创新与极致安全的项目方，CiaoTool 构筑了最高效的落地通道：

* **零代码极速创建：**\
  彻底免去编写与调试复杂智能合约的繁琐流程，全前端表单化操作，一键支付 Gas 费即可实现链上资产的极速诞生，将技术门槛降至为零。
* **全矩阵生态闭环：**\
  完美衔接 CiaoTool 强大的市值管理（MM）与流动性管理工具，帮助项目从“创建”平稳过渡到“运营”，完美适配从资产生成到生态繁荣的全生命周期战略。

***

## **图文指南 | BSC 底池燃烧代币**创建

{% stepper %}
{% step %}
### **绑定钱包**

选择你要创建代币的**区块链**，并绑定支持 EVM 网络的钱包

<figure><img src="../../../.gitbook/assets/image (446).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 填写代币基础信息

<figure><img src="../../../.gitbook/assets/image (530).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
<mark style="color:blue;">**LOGO 及 项目描述**</mark>

EVM 网络创建代币并不会将 LOGO 和 项目描述信息同步上链，需要自行联系去中心化平台及钱包dapp申请 LOGO 及其附属信息。我们也有偿提供代币 LOGO 上传服务，各平台与网络要求与价格均不相同，[联系我们以获取 LOGO 上传服务费用。](https://t.me/CiaoTools)
{% endhint %}

* **代币名称：**&#x60A8;希望展示在钱包或区块浏览器中的完整代币名称（_例如：MyFirstToken_）。
* **代币简称：**&#x4EE3;币的缩写，通常为 3\~6 个大写字母（_例如：MYT_）。
* **精度：**&#x6307;的是一种代币最小可以分割到的小数位数。简单来说，它决定了你可以将一枚代币分成多小的单位。常见为 18 位。
* **总供应量：**&#x53D1;行的代币总量
{% endstep %}

{% step %}
### 填写收币地址

创建代币后，接收所有代币的地址。即将代币所有权和所有代币转移到指定地址
{% endstep %}

{% step %}
### 314 设置

<figure><img src="../../../.gitbook/assets/image (539).png" alt=""><figcaption></figcaption></figure>

* **流动性占比：**&#x53D1;币时，自动转入合约地址的代币比例,用以提供流动性。
* **冷却时间(秒)：**&#x6BCF;次买入之间的间隔时间,单个每次卖出的间隔时间
{% endstep %}

{% step %}
### 设置买卖税率

CiaoTool 支持买入卖出双税费机制，您可以自由配置买入和卖出税率。

<figure><img src="../../../.gitbook/assets/image (541).png" alt=""><figcaption></figcaption></figure>

* **营销税率**：交易中指定额度的代币将会自动转入指定的营销钱包中，用于进行其他营销活动。
* **销毁税率**：交易中指定额度的代币将会被打入黑洞地址，变相实现通缩机制，变相拉升代币价值。
* **营销钱包**：用于接收营销税费的钱包地址。
{% endstep %}

{% step %}
### 多功能开启

以下功能均可通过控制台调整参数，或永久关闭权限。

1. **最大持币量限制**\
   可设置单个钱包最大持有代币数量。此开关关闭后无法再次开启。
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下&#x65B9;**「创建合约」**&#x6309;钮，并等待合约创建完成。
{% endstep %}

{% step %}
### 添加代币到钱包dapp

部分钱包无法直接查看到流动性小的代币，但你可以通过手动添加的方式，将您的代币添加到钱包当中。

<details>

<summary><strong>添加教程</strong></summary>

1. 打开你的钱包，插件钱包或APP程序
2. 找到代币页面-选择添加代币

<img src="https://ciaotool.gitbook.io/docs/~gitbook/image?url=https%3A%2F%2Fcontent.gitbook.com%2Fcontent%2FRbU9EUruu3lWQ1GJ5WVC%2Fblobs%2FAPA2BpGAbSxRd0loKfVb%2Fimage.png&#x26;width=768&#x26;dpr=3&#x26;quality=100&#x26;sign=71aaa5bf&#x26;sv=2" alt="" height="218" width="443">

3. 选择你创建代币所在的链，两种模式添加，这里我们选择自定义代币

<figure><img src="../../../.gitbook/assets/image (521).png" alt=""><figcaption></figcaption></figure>

4. 粘贴你的代币合约，即可查看你的代币信息，点击导入即可

<figure><img src="../../../.gitbook/assets/image (520).png" alt=""><figcaption></figcaption></figure>

</details>
{% endstep %}

{% step %}
### 创建流动性池

{% hint style="danger" %}
不建议创建流动性池，该代币仍有很多限制条件且没有税率功能，创建流动性池仅支持 BNB。同时，一个代币会形成两个池子（薄饼池与转账池）、两个价格，容易被搬砖套利。
{% endhint %}

虽然 314 协议代币可以直接通过转账的形式实现代币的买卖操作，但您仍可以选择创建 V2 流动性资金池与 BNB 配对，让您的代币可以在去中心化交易所显示并参与交易。

点击查看创建流动性池教程：

<table data-card-size="large" data-view="cards"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td>创建流动性池 - V2</td><td><a href="../../../chains/bsc/swap/create-liquidity-v2.md">create-liquidity-v2.md</a></td></tr><tr><td>创建流动性池并捆绑买入 - V2</td><td><a href="../../../chains/bsc/swap/bundler-v2.md">bundler-v2.md</a></td></tr></tbody></table>
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>为什么批量转账失败？</strong></summary>

批量转账之前，须确保批量转账的**合约地址**在「交易冷却白名单」和「持币白名单」内，才能够实现批量转账。

批量转账合约地址：`0x7FF7E8Bb75De25d411Df3940eb96400d234cd62e`

</details>

<details>

<summary><strong>交易冷却如何生效？</strong></summary>

交易冷却在设置的时间内限制全网买单和每个地址卖单数量。冷却时间内，其他用户无法买入，单个地址也只能卖一次。冷却时间结束后，交易才会恢复。

</details>

<details>

<summary><strong>代币名称和代币简称能使用中文吗？</strong></summary>

可以，现在 BSC 链全面支持中文、英文以及中英混合文字。

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
