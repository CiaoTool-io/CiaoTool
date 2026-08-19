---
description: >-
  CiaoTool 提供免代码的 BSC 持币分红代币智能合约部署服务。支持自定义交易税率并全自动分发链上任意资产。助力 Web3
  项目方建立强大的长期持有共识模型。
metaLinks:
  alternates:
    - https://app.gitbook.com/s/b56FKZGe1viFi67H1pPQ/token/hold-ref-others
---

# BSC - 持币暴利分红创建教程

{% hint style="danger" %}
<mark style="color:red;">**检测风险提醒**</mark>

该类型代币由于采用特殊机制或扩展功能，部分安全检测平台可能会标记为**存在潜在风险或给予较低评分**。若您较为关注代币检测结果，建议选择[**「创建标准代币」**](standard-token-evm.md)，标准代币通常具有更好的兼容性与检测表现。继续创建此类型代币，**即表示您已了解并接受可能产生的检测提示或风险标记。**
{% endhint %}

## BSC 持币暴利分红是什么？

<figure><img src="../../../.gitbook/assets/image (542).png" alt=""><figcaption></figcaption></figure>

当链上发生任何一笔买入或卖出时，合约会自动拦截预设比例的税费，并在去中心化交易所底层自动触发 兑换指令，将扣除的税费兑换为您预先指定的任意链上资产（例如 USDT、WBNB，甚至是另一款热门 Meme 币），随后全自动空投给所有持币地址。

| 对比维度   | 分红本币               | 持币暴力分红                    |
| ------ | ------------------ | ------------------------- |
| 收益资产类型 | 项目代币本身             | 链上已有资产                    |
| 核心机制   | 交易税 ➔ 全网持币地址余额增加   | 交易税 ➔ 合约自动兑换 ➔ 转换为 BNB 空投 |
| 核心吸引力  | “币生币”，赌项目未来的百倍升值预期 | “持币生金”，获取真实的现金流与其他共识资产    |

立即在 BSC 网络上，用 CiaoTool​ 创建持币暴力分红代币：

{% embed url="https://bsc.ciaotool.io/zh-Hans/token/hold-ref-others" %}

***

## 为什么选择 CiaoTool BSC 持币暴力分红代币创建？

CiaoTool 为 BSC 链上的资产发行提供了一种兼顾绝对安全与极简操作的专业解决方案。对于需要处理复杂链上跨资产路由的项目方，CiaoTool 构筑了极致安全与高效的基础设施：

* **灵活的通缩矩阵配置：** \
  支持自定义买入税、卖出税的具体比例。不仅可以设置回流，还能灵活配置营销钱包抽水或自动销毁比例，完美适配各种复杂多变的操盘策略。
* **零代码极速创建：**\
  彻底免去编写与调试复杂智能合约的繁琐流程，全前端表单化操作，一键支付 Gas 费即可实现链上资产的极速诞生，将技术门槛降至为零。
* **全矩阵生态闭环：**\
  完美衔接 CiaoTool 强大的市值管理（MM）与流动性管理工具，帮助项目从“创建”平稳过渡到“运营”，完美适配从资产生成到生态繁荣的全生命周期战略。

***

## **图文指南 | BSC** 持币暴力分红代币创建

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

选择或输入分红的代币地址，产生税费时并分发给持有者的代币，可以是主流价值代币，也可以是任意 BEP-20 代币。

<figure><img src="../../../.gitbook/assets/image (543).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 设置买卖税率

CiaoTool 支持买入卖出双税费机制，您可以自由配置买入和卖出税率。

<figure><img src="../../../.gitbook/assets/image (544).png" alt=""><figcaption></figcaption></figure>

* **营销税率**：交易中指定额度的代币将会自动转入指定的营销钱包中，用于进行其他营销活动。
* **分红税率**：交易中指定额度的代币会按持币比例分配给所有 LP 代币持有者，实现分红。
* **销毁税率**：交易中指定额度的代币将会被打入黑洞地址，变相实现通缩机制，变相拉升代币价值。
* **回流税率**：交易中指定额度的代币将会自动添加到流动池内，保证交易始终存在流动性。
* **营销钱包**：用于接收营销税费的钱包地址。
* **分红最小持币量：**&#x94B1;包地址中持币量超过此门槛才获得分红资格，合理的门槛设置可以让用户更长期和更多数量的持有，不填默认为 0 。
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
2. **税率开关**\
   创建后可随时手动调整买卖税率，但是买卖税率都需要为 0 ≤ 25%。
3. **黑名单功能**\
   可拉黑部分钱包地址令其无法交易及转账。此按钮关闭后无法再次开启。
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

<summary><strong>黑洞地址、合约地址会分红吗？</strong></summary>

不会，黑洞、代币合约、流动性池地址默认排除。

</details>

<details>

<summary><strong>为什么钱包多出 Tracker 代币？</strong></summary>

Tracker 用于记录分红权重，不可转账，否则分红会混乱。

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
