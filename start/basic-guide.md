---
description: 如果你是第一次接触“发币”这个概念，请放轻松——看完这篇，你就能从“币圈小白”变成“发币专家”。
metaLinks:
  alternates:
    - https://app.gitbook.com/s/b56FKZGe1viFi67H1pPQ/basic-guide
---

# 新人发币最全指南

区块链的世界看似复杂：各种术语、不同公链、费用机制、权限设置……\
但其实，发币这件事并不神秘。借助像 **CiaoTool** 这样的智能一键发币平台，你无需会代码，也不用担心安全与部署问题，只要几分钟，就能完成。

***

### 🧩 第一部分：发币前的准备与概念入门

#### **🔹 什么是“发币”？**

**发币（Create Token）指的是：** 在一条已有的区块链上，部署一个属于你的代币合约。你定义名字、符号、总量、功能 —— 你就是它的创造者。

> 🧠 举个例子：比特币是独立公链（挖矿产出），而你要创建的是部署在某条链上的“代币”，比如在 BSC 或 Solana 上生成自己的 Token。

***

#### **🔹 选链：在哪条链上发？**

不同公链的规则、成本都不同，这个是你需要提前计划的，BSC链和Solana链热度偏高。\
目前主流选择如下：

| 区块链                        | 特点         | 适合人群            |
| -------------------------- | ---------- | --------------- |
| **BSC（币安链）**               | 成熟稳定、交易成本低 | 新手/项目方          |
| **Solana**                 | 速度快、生态活跃   | 想做 Meme 或轻项目的用户 |
| **Base / X Layer / IoTeX** | 新兴链，操作灵活   | 想玩新生态的开发者       |

![](<../.gitbook/assets/image (5)>)

***

#### **🔹 如何发币？**

一般来说，发行代币必须由开发者编写智能合约并完成上链部署。但如果你不懂技术，其实可以直接利用 **一键式发币工具（CiaoTool）** 来跳过写代码这一步。支付一笔很低的服务费，就能在几分钟内生成属于你的代币。

#### **🔹 发币要多少钱？**

费用随链而异，一般用该链的原生代币支付，可参考官方费用获取实时数据：

* **Solana ➜ 用 SOL**，费用：[https://ciaotool.gitbook.io/ciaotool/sol/price](https://ciaotool.gitbook.io/ciaotool/sol/price)
* **BSC ➜ 用 BNB** ，费用：[https://ciaotool.gitbook.io/ciaotool/bsc/price](https://ciaotool.gitbook.io/ciaotool/bsc/price)
* **Base ➜ 用 ETH**，费用：[https://base.ciaotool.io/](https://base.ciaotool.io/)
* **IoTeX ➜ 用IOTX**，费用：[https://ciaotool.gitbook.io/ciaotool/iotex/price](https://ciaotool.gitbook.io/ciaotool/iotex/price)
* **OKX链（X Layer) ➜ 用 OKB**，费用：[https://xlayer.ciaotool.io/](https://xlayer.ciaotool.io/)

***

#### **🔹 发完币之后能做什么？**

✅ 你可以：

* 转账或空投给他人
* 创建流动性池（Liquidity Pool）供交易
* 查看代币在 DEX 平台的行情

⚠️ 注意：要想让你的代币能交易、有价格、并在 GMGN、DexScreener 上显示，必须创建流动性池。

***

#### **🔹 内盘 vs 一键发币的区别？**

| 类型       | 特征                 | 说明          |
| -------- | ------------------ | ----------- |
| **内盘发币** | 自动加池、代币需购买、项目方控制力弱 | 适合轻量应用      |
| **一键发币** | 代币直接到账、自主加池、功能可配置  | 项目方完全掌控代币逻辑 |

> 💡 CiaoTool 支持两种模式：既能做「一键发币」，也能连接 PumpFun、BonkFun、Fourmeme、Flap 等内盘生态创建并买入。

***

#### **⚙️ 发币前准备清单**

| 工具                          | 用途                                          |
| --------------------------- | ------------------------------------------- |
| 💻 电脑/手机                    | 建议用电脑操作（更稳定便捷）                              |
| 🌐 可用的网络配置环境                | 访问链上资源与教程                                   |
| 💰 钱包（MetaMask/Phantom/OKX） | 存放链上资产                                      |
| 🪙 资产准备                     | 钱包中需有 BNB、SOL 等支付 Gas 的代币                   |
| 💬 Telegram                 | 加入 CiaoTool 官方群组获取帮助： https://t.me/ciaotool |

{% hint style="warning" %}
重要提醒：

* 不会用钱包 ❌ 不建议发币
* 钱包没资产 ❌ 不建议发币
* 不懂基础概念 ❌ 不建议发币
{% endhint %}

***

### 💥 第二部分：发币实操指南

准备好了吗？这一部分，我们正式进入实战！无论你打算做一个社群 Token、Meme 币还是实验项目，流程都大同小异。

{% stepper %}
{% step %}
#### 填写基本信息

参数说明与建议：

* 名称（Name）：代币全称，可中英文。示例：SolDog、喵币
* 符号（Symbol）：简称，通常 3-5 字母。示例：DOG、MEOW
* 总量（Supply）：代币最大数量，建议整数、非小数
* 精度（Decimals）：最小分割单位，推荐 18
* 头像（Logo）：Solana 链支持上传，其他链有时上传了也不一定显示（Solana 链可自行替换，其他链需联系对应官方客服）
{% endstep %}

{% step %}
#### 可选功能配置

常见功能与适合人群：

* 燃烧（销毁部分代币，推高价格）—— 想做通缩模型的项目
* 黑名单（冻结特定地址）—— 防御恶意钱包
* 增发（动态增加供应量）—— 测试用途
* 标准代币（无任何权限功能）—— 新手推荐，全绿检测

> 建议新手创建「标准代币」—— 功能最简洁、安全性最高、风控检测最友好。
{% endstep %}

{% step %}
#### 选择区块链

选择要部署的链与其优劣：

* EVM 系（BSC/Base/X Layer）：功能强大、兼容性高，成本略高
* Solana：速度快、头像显示友好，功能较简洁
{% endstep %}

{% step %}
#### 支付与创建

确认参数后，系统会提示支付发币费用。支付完成后，代币会自动生成并发送到当前绑定的钱包，如果未在钱包查看到请自行添加到钱包中。
{% endstep %}
{% endstepper %}

***

### 💼 第三部分：发币后的管理与维护

恭喜你！到这里，你已经正式拥有了自己的代币。但接下来还有更关键的部分——如何运营与维护代币生态。

#### **💡 常见问题速查**

<details>

<summary>Q1：代币在哪？为什么钱包看不到？</summary>

所有代币都在你连接的钱包中。若未显示，请手动添加代币地址。

</details>

<details>

<summary>Q2：怎么交易？</summary>

创建流动性池（Liquidity Pool），例如：

* **BSC：**&#x50;ancakeSwap，[https://pancakeswap.finance/liquidity/pools?](https://pancakeswap.finance/liquidity/pools?)
* **Solana：**&#x52;aydium，[https://raydium.io/liquidity-pools/](https://raydium.io/liquidity-pools/)
* **Base:** PancakeSwap，[https://pancakeswap.finance/liquidity/pools?](https://pancakeswap.finance/liquidity/pools?)
* **X Layer:** potatoswap，[https://potatoswap.finance/swap](https://potatoswap.finance/swap)

</details>

<details>

<summary>Q3：代币价格怎么来？</summary>

价格 = 流动池内两种资产比例。例如：100 USDT + 100 TOKEN = 初始价 1 USDT/TOKEN。

</details>

<details>

<summary>Q4：为什么风险检测显示红？</summary>

若添加“增发”“黑名单”等功能，检测会判为高风险。建议用「标准代币」保持绿色标识。

</details>

<details>

<summary>Q5：别人买了我的代币，钱去哪？</summary>

买入资金进入资金池。要取出收益，可通过“移除流动性”操作。

</details>

***

#### **🧠 资金池知识要点**

| 项目                | 说明                    |
| ----------------- | --------------------- |
| 谁都能创建资金池          | 只要有代币与资产即可            |
| 投入多少合适？           | 没有固定门槛，几十美金也能建池       |
| 池子代币会被买完吗？        | 理论上不会，价格会上升直到趋近 0     |
| 如何稳定价格？           | 采用 CLMM 或单币加池可提升稳定性   |
| Solana 需要市场 ID 吗？ | 仅 AMM 模式需创建 Market ID |

***

### 🧰 第四部分：发币后的实用工具推荐

发币只是起点，想运营得好，还要会用工具。CiaoTool 提供了一整套配套功能：

| 功能     | 用途        | 说明            |
| ------ | --------- | ------------- |
| 批量转账   | 一次空投上百个地址 | 可上传表格或导入文件    |
| 快照导出   | 导出持币名单    | 用于空投、治理、奖励    |
| 市值管理   | 多地址交易操盘   | 控制价格曲线        |
| 批量生成钱包 | 一次生成上百个地址 | 支持 Solana、BSC |
| 批量归集   | 多地址资产回收   | 方便资金管理        |

* 🌐 教程站：[https://ciaotool.gitbook.io/ciaotool](https://ciaotool.gitbook.io/ciaotool)
* 💬 Telegram：[t.me/ciaotool](https://t.me/ciaotool)

***

#### ✅ [在 CiaoTool 的加持下，发币不再需要懂代码或部署节点。](https://ciaotool.io/)

只需准备好钱包与资产，你就能完成从「想法 → Token → 市场」的闭环。

> 🚀 发币的门槛越来越低，但运营的门槛越来越高。真正的竞争，不在“谁先发”，而在“谁能运营好”。愿你在链上的第一枚代币，成为你进入 Web3 世界的钥匙。
