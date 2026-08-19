---
description: >-
  一键部署 BEP-20 流动性激励智能合约，自定义交易税率并全自动回馈流动性提供者，加池即可参与收益，持币奖励增加，助力 Web3
  项目打造深厚的流动性护城河与长效通缩经济模型。
metaLinks:
  alternates:
    - https://app.gitbook.com/s/b56FKZGe1viFi67H1pPQ/token/lp-reflection
---

# BSC - LP 分红代币创建教程

{% hint style="danger" %}
<mark style="color:red;">**检测风险提醒**</mark>

该类型代币由于采用特殊机制或扩展功能，部分安全检测平台可能会标记为**存在潜在风险或给予较低评分**。若您较为关注代币检测结果，建议选择[**「创建标准代币」**](standard-token-evm.md)，标准代币通常具有更好的兼容性与检测表现。继续创建此类型代币，**即表示您已了解并接受可能产生的检测提示或风险标记。**
{% endhint %}

## CiaoTool BSC LP 分红代币创建是什么？

<figure><img src="../../../.gitbook/assets/image (532).png" alt="CiaoTool BSC LP分红代币创建 页面"><figcaption></figcaption></figure>

**CiaoTool BSC LP 分红代币创建**是一款专为解决 Web3 项目「流动性枯竭」痛点而设计的高阶智能合约部署工具。它允许项目方突破复杂开发的瓶颈，在 BSC 链上极速发行带有「专属 LP 收益池」的 BEP-20 协议代币。

相较于将收益平均分发给所有持币者的普通分红代币，该功能的核心机制在于「定向赋能流动性提供者」。系统在智能合约底层内置了自动化税收分配协议：当链上发生任何代币交易时，合约会自动按预设比例扣除税费，并在同区块内，精准计算 PancakeSwap 等去中心化交易所中的 LP Token 持有权重，将红利全自动「空投」给所有为项目做市加池的LP地址。

| 对比维度   | 分红本币         | LP 分红代币                             |
| ------ | ------------ | ----------------------------------- |
| 激励对象   | 所有只要钱包里有代币的人 | 仅激励在交易所添加了流动性资金（LP）的人               |
| 对项目的好处 | 鼓励大家囤币不卖     | 极大加厚资金池底池深度，减少价格剧烈波动                |
| 用户收益来源 | 被动等待交易产生分红   | 赚取双份收益：既能拿 DEX 交易手续费，又能拿智能合约的自动代币分红 |
| 防砸盘效果  | 一般           | 极强                                  |

立即在 BSC 网络上，用 CiaoTool​ 创建 LP 分红代币：

{% embed url="https://bsc.ciaotool.io/zh-Hans/token/lp-reflection" %}

***

## 为什么选择 CiaoTool BSC LP 分红代币创建？

CiaoTool 为 BSC 链上的资产发行提供了一种兼顾绝对安全与极简操作的专业解决方案。对于需要快速部署纯净代币的用户而言，该工具构建了高效且稳健的执行防线：

* **灵活的通缩矩阵配置：** \
  支持自定义买入税、卖出税的具体比例。不仅可以设置全额分红，还能灵活配置营销钱包抽水或自动销毁比例，完美适配各种复杂多变的操盘策略。
* **零代码极速创建：**\
  彻底免去编写与调试复杂智能合约的繁琐流程，全前端表单化操作，一键支付 Gas 费即可实现链上资产的极速诞生，将技术门槛降至为零。
* **信任与控制的完美平衡：**\
  工具内置了单向的「权限放弃」机制。当项目平稳度过首发期后，您可以将「黑名单」或「最大持币量」开关永久关闭，以此向社区证明合约的去中心化与绝对安全，极大增强持币者信心。
* **全矩阵生态闭环：**\
  完美衔接 CiaoTool 强大的市值管理（MM）与流动性管理工具，帮助项目从“创建”平稳过渡到“运营”，完美适配从资产生成到生态繁荣的全生命周期战略。

***

## **图文指南 | BSC LP 分红代币**创建

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
### 选择分红代币

选择或输入想要分红的代币。

**选择的分红代币必须在有 BNB 的交易对**，且可以正常买卖。如果该代币流动性过低或者没有 BNB 交易对，很可能导致无法分红。通常使用主流币。
{% endstep %}

{% step %}
### 设置买卖税率

CiaoTool 支持买入卖出双税费机制，您可以自由配置买入和卖出税率。

<figure><img src="../../../.gitbook/assets/image (531).png" alt=""><figcaption></figcaption></figure>

* **营销税率**：交易中指定额度的代币将会自动转入指定的营销钱包中，用于进行其他营销活动。
* **分红税率**：交易中指定额度的代币会按持币比例分配给所有 LP 代币持有者，实现分红。
* **销毁税率**：交易中指定额度的代币将会被打入黑洞地址，变相实现通缩机制，变相拉升代币价值。
* **回流税率**：交易中指定额度的代币将会自动添加到流动池内，保证交易始终存在流动性。
* **营销钱包**：用于接收营销税费的钱包地址。
{% endstep %}

{% step %}
### 流动性初始设置

<figure><img src="../../../.gitbook/assets/image (526).png" alt=""><figcaption></figcaption></figure>

初始创建流动性池时，必须使用初始设置，以触发 LP 分红机制。

* **交易所：**&#x42;SC 链目前只支持 PancakeSwap。
* **底池代币：**&#x5373;与新代币配对的价值代币，通常使用主流币。
{% endstep %}

{% step %}
### 多功能开启

以下功能均可通过控制台调整参数，或永久关闭权限。

1. **手动开启交易**\
   添加池子后的首次交易需要在控制台手动开启。
2. **杀区块**\
   将对开启交易后在n个区块内交易的地址全部拉入黑名单，用于防止机器人抢跑买入，必须手动开启交易。

<figure><img src="../../../.gitbook/assets/image (533).png" alt=""><figcaption></figcaption></figure>

3. **税率开关**\
   创建后可随时手动调整买卖税率，但是买卖税率都需要为 0 ≤ 25%。
4. **自动空投**\
   每笔交易向随机最多 5 个地址空投少量代币，以增加持币人数。
5. **黑名单功能**\
   可拉黑部分钱包地址令其无法交易及转账。此按钮关闭后无法再次开启。
6. **最大持币量限制**\
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
初始创建流动性资产池必须&#x4E3A;**「V2」流动性池**，「V3」流动性池无法参与任何税费机制。
{% endhint %}

代币创建完成后，还不具有交易属性，只能进行转账操作。添加流动性资金池，让代币在去中心化平台自由兑换。

点击查看创建流动性池教程：

<table data-card-size="large" data-view="cards"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td>创建流动性池 - V2</td><td><a href="../../../chains/bsc/swap/create-liquidity-v2.md">create-liquidity-v2.md</a></td></tr><tr><td>创建流动性池并捆绑买入 - V2</td><td><a href="../../../chains/bsc/swap/bundler-v2.md">bundler-v2.md</a></td></tr><tr><td>创建流动性池 - V3</td><td><a href="../../../chains/bsc/swap/create-liquidity-v3.md">create-liquidity-v3.md</a></td></tr><tr><td>创建流动性池并捆绑买入 - V3</td><td><a href="../../../chains/bsc/swap/bundler-v3.md">bundler-v3.md</a></td></tr></tbody></table>
{% endstep %}
{% endstepper %}

***

## **常见问题 FAQ**

<details>

<summary><strong>分红币种如何选择？</strong></summary>

创建代币时可选择主流币（如 wBNB、USDT、USDC、DOGE）作为分红币，所选币必须与 BNB 有交易对且流动性充足。

</details>

<details>

<summary><strong>如何确保可以获得分红？</strong></summary>

必须自己加池并产生买卖交易才能激活分红，转账获得的 LP 或仅买入而不卖出都无法获得分红。

</details>

<details>

<summary><strong>为什么买了很多笔还是没有分红？</strong></summary>

不要使用白名单地址交易，如发币地址、营销钱包地址交易都无法触发分红。

交易税费以「买 + 卖」为一个循环，必须先触发卖出机制才能触发分红条件。

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
