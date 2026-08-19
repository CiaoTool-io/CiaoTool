---
description: >-
  CiaoTool 提供免代码的 BSC 多功能代币智能合约部署服务。内置增发、暂停交易、黑名单及防巨鲸（最大持币量）四大模块化开关，一键部署 BEP-20
  极速上链，助力灵活管控代币全生命周期。
metaLinks:
  alternates:
    - https://app.gitbook.com/s/b56FKZGe1viFi67H1pPQ/token/simple-control
---

# BSC - 多功能代币创建教程

{% hint style="danger" %}
<mark style="color:red;">**检测风险提醒**</mark>

该类型代币由于采用特殊机制或扩展功能，部分安全检测平台可能会标记为**存在潜在风险或给予较低评分**。若您较为关注代币检测结果，建议选择[**「创建标准代币」**](standard-token-evm.md)，标准代币通常具有更好的兼容性与检测表现。继续创建此类型代币，**即表示您已了解并接受可能产生的检测提示或风险标记。**
{% endhint %}

## CiaoTool BSC 多功能代币创建是什么？

<figure><img src="../../../.gitbook/assets/image (527).png" alt=""><figcaption></figcaption></figure>

**CiaoTool BSC 多功能代币创建**是一款专为 Web3 项目方及进阶运营者打造的高效智能合约部署工具。它允许用户突破复杂代码开发的限制，在 BSC 链上极速发行高阶的 BEP-20 代币。

相较于普通的标准代币，多功能代币的核心机制在于「底层合约的模块化权限管控」。在保持「零交易税费、零分红摩擦」的纯净流通属性基础上，系统额外开放了自定义收币地址选择，并内置了四大极具战略价值的管理开关：增发代币、暂停交易、黑名单、最大持币量。这种机制让项目方在面临做市起盘、机器人抢跑或产品测试时，拥有强大的链上治理与风控能力。

此工具通过灵活的权限组合，完美适配需要强风控与早期运营干预的 Web3 场景：

* **防机器人与防巨鲸首发：** \
  开盘前打开「最大持币量」和「黑名单」，把抢跑的机器人全部拉黑，保护真实散户玩家。
* **合规与风控测试：**\
  &#x20;利用「暂停交易」功能，遇到黑客攻击，确保经济系统安全。
* **生态持续扩容项目：** \
  开启「增发代币」权限，允许在未来出块、DAO 奖励发放时，动态增加流通供应量。

立即在 BSC 网络上，用 CiaoTool​ 创建多功能代币：

{% embed url="https://bsc.ciaotool.io/zh-Hans/token/simple-control" %}

***

## 为什么选择 CiaoTool BSC 多功能代币创建？

CiaoTool 为 BSC 链上的资产发行提供了一种兼顾绝对安全与极简操作的专业解决方案。对于需要快速部署纯净代币的用户而言，该工具构建了高效且稳健的执行防线：

* **灵活的开关配置：** \
  彻底免去复杂的代码编译。四大权限开关只需在界面上一键拨动，即可将复杂的风控逻辑无缝打包进智能合约。自定义收币地址功能更方便了多签名钱包或冷钱包进行初始资产隔离。
* **零代码极速创建：**\
  彻底免去编写与调试复杂智能合约的繁琐流程，全前端表单化操作，一键支付 Gas 费即可实现链上资产的极速诞生，将技术门槛降至为零。
* **信任与控制的完美平衡：**\
  工具内置了单向的「权限放弃」机制。当项目平稳度过首发期后，您可以将「黑名单」或「最大持币量」开关永久关闭，以此向社区证明合约的去中心化与绝对安全，极大增强持币者信心。
* **全矩阵生态闭环：**\
  完美衔接 CiaoTool 强大的市值管理（MM）与流动性管理工具，帮助项目从“创建”平稳过渡到“运营”，完美适配从资产生成到生态繁荣的全生命周期战略。

***

## 视频教程 | BSC 多功能代币创建

{% embed url="https://www.youtube.com/watch?v=cbBKmbMs32E" %}

***

## **图文指南 | BSC 多功能代币**创建

{% stepper %}
{% step %}
### **绑定钱包**

选择你要创建代币的**区块链**，并绑定支持 EVM 网络的钱包

<figure><img src="../../../.gitbook/assets/image (446).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 填写代币基础信息

<figure><img src="../../../.gitbook/assets/image (529).png" alt=""><figcaption></figcaption></figure>

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
### 多功能开启

以下功能均可通过控制台调整参数，或永久关闭权限。

1. **增发代币**\
   可通过控制台增发/铸造代币。增发可发送到指定地址
2. **暂停交易**\
   可以拥有暂停或开启全部的转账和交易的权限。
3. **黑名单功能**\
   可拉黑部分钱包地址令其无法交易及转账。此按钮关闭后无法再次开启。
4. **最大持币量限制**\
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

代币创建完成后，还不具有交易属性，只能进行转账操作。添加流动性资金池，让代币在去中心化平台自由兑换。

点击查看创建流动性池教程：

<table data-card-size="large" data-view="cards"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td>创建流动性池 - V2</td><td><a href="../../../chains/bsc/swap/create-liquidity-v2.md">create-liquidity-v2.md</a></td></tr><tr><td>创建流动性池并捆绑买入 - V2</td><td><a href="../../../chains/bsc/swap/bundler-v2.md">bundler-v2.md</a></td></tr><tr><td>创建流动性池 - V3</td><td><a href="../../../chains/bsc/swap/create-liquidity-v3.md">create-liquidity-v3.md</a></td></tr><tr><td>创建流动性池并捆绑买入 - V3</td><td><a href="../../../chains/bsc/swap/bundler-v3.md">bundler-v3.md</a></td></tr></tbody></table>
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>发币后还能修改参数吗？</strong></summary>

不能，创建完成后默认丢弃权限，无法修改代币参数，也没有后台控制功能。修改需重新创建新代币。

</details>

<details>

<summary><strong>为什么创建流动性池失败？</strong></summary>

因为池子地址内的代币数量已经达到了持仓上限，请确保池子地址在白名单内，或符合持币限制。

</details>

<details>

<summary><strong>为什么白名单在暂停交易期间还无法买币？</strong></summary>

暂停交易期间，池子地址无法转账。请确保池子地址在白名单内，才能拥有交易权限以维持交易。

</details>

<details>

<summary><strong>为什么正常交易期间用户无法卖出？</strong></summary>

池子地址内代币数量达到持仓上限，请确保池子地址在白名单内，或符合持币限制。

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
