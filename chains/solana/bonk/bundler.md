---
description: >-
  专为 BONKfun
  平台提供的代币发行与多地址捆绑买入工具。支持在同区块内同步完成代币创建与首笔批量买入，有效阻断机器人抢跑，确保项目方以极低初始成本安全建仓并优化早期持币分布。
---

# Bonk - 创建并买入教程

{% hint style="info" %}
**CiaoTool Bonk 创建并买入**现已全面支持官方 **SOL** 和 **USD1** 全部的价值代币。
{% endhint %}

## 功能介绍

CiaoTool Bonk 创建并买入是一款代币发行与多钱包买入工具，可在创建 Bonk.fun 代币的同时，按预设金额完成多个钱包的首批买入。

系统将代币创建与买入交易按指定顺序组成 Bundle 提交。正常执行时，创建交易先完成，随后各钱包在同一区块内连续买入，减少发币与买入之间被其他交易插入的风险。

立即在 Bonk 上，用 CiaoTool​ 创建并买入功能进行一键开盘操作：

{% embed url="https://ciaotool.io/zh-CN/bonk/create-and-buy" %}

***

## 核心优势

* **创建买入一体化：** 一次配置代币信息和各钱包买入金额
* **顺序执行：** 创建与买入交易按预设顺序打包提交
* **多钱包配置：** 支持分别设置参与钱包及买入金额
* **自动化执行：** 完成资料上传、交易构建、钱包签名和 Bundle 提交
* **结果可核对：** 展示各笔交易的执行状态及交易记录

***

## 视频教程

{% embed url="https://www.youtube.com/watch?v=Ir3oB7Li7PM" %}

***

## **技术实现示意**

### 传统发射代币

代币创建与多个钱包的买入交易分别广播、独立上链，无法保证按预设顺序执行或进入同一区块。若其他交易抢先成交，池内价格可能提前变化，导致后续钱包买入成本上升、获得的代币数量减少。

<figure><img src="../../../.gitbook/assets/Frame 1321314906.png" alt=""><figcaption></figcaption></figure>

### 捆绑发射代币

将「代币创建」与「多达 8 个钱包」的买入交易按预设顺序打包至同一 Bundle 捆绑包内，并在同一区块内连续执行，减少交易间隙被其他交易插入的风险，提升发射与买入的执行一致性及上链优先级。

<figure><img src="../../../.gitbook/assets/Frame 1321314907.png" alt=""><figcaption></figcaption></figure>

***

## **图文指南**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角【连接钱包】按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (748).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 填写代币信息

<figure><img src="../../../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>

* **代币名称：**&#x60A8;希望展示在钱包或区块浏览器中的完整代币名称（_例如：MyFirstToken_）。
* **代币简称：**&#x4EE3;币的缩写，通常为 3\~6 个大写字母（_例如：MYT_）。
* **LOGO：**&#x4E0A;传项目或代币的标志图像，建议尺寸 1000\*1000 像素。
* **描述：** 简要介绍代币用途、故事或 Meme 背景（选填）。
{% endstep %}

{% step %}
### 添加链接<mark style="color:$info;">（可选）</mark>

虽然为可选项，但强烈建议填写，**官网、X / Twitter、Telegram**，增加项目可信度。

<figure><img src="../../../.gitbook/assets/image (14).png" alt=""><figcaption></figcaption></figure>
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
### 创建参数

#### 报价代币

Bonk.fun 现支持 SOL 和 USD1 作为报价代币，点击切换选择。

#### 开发者钱包买入

即当前绑定钱包进行买入操作，不填默认为 0。在 GMGN、DEXScreener 等链上监控平台会被标记为 Dev 钱包。
{% endstep %}

{% step %}
### 导入钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入接收地址的类型，选择以查看详细教程。最多支持 **8 个地址**捆绑买入。

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「批量输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (887).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x6BCF;行仅输入一个钱包私钥，可在私钥后追加数量。

```
privateKey, 300
```

<figure><img src="../../../.gitbook/assets/image (737).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 下载 CiaoTool 模板文件，并将信息导入到文件内。

<figure><img src="../../../.gitbook/assets/image (7).png" alt=""><figcaption></figcaption></figure>

2. 点击![](<../../../.gitbook/assets/image (848).png>)**「导入文件」**&#x6309;钮，弹出文件上传窗口。
3. 点&#x51FB;**「确定导入」**，将所有地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 输入交易金额

支&#x6301;**「逐一输入」「输入金额」**&#x4E24;种交易金额类型。开发者钱包买入 + 捆绑钱包买入代币数量 不能超过 86 SOL。

<figure><img src="../../../.gitbook/assets/image (8).png" alt=""><figcaption></figcaption></figure>

1. **逐一输入**\
   在输入框中，逐一输入交易金额数量。
2. **统一金额**\
   点击交易数量上方的![](<../../../.gitbook/assets/image (724).png>)按&#x94AE;**，**&#x9009;&#x62E9;**「输入金额」**&#x9009;项，所有地址将统一交易数量。
{% endstep %}

{% step %}
### 自动卖出

当代币价格在联合曲线期间，比初始买入金额达到指定目标涨幅时，所有捆绑买入地址将自动卖出，获取收益。

<figure><img src="../../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Jito 小费设置

{% hint style="danger" %}
此功能实现依赖于 Jito 的捆绑功能。由于网络环境、Jito节点、RPC节点和区块处理引擎的复杂影响，该功能可能面临较高的失败率。

若操作失败，不会开盘成功也不会产生任何费用，请尝试更换RPC节点，区块处理引擎，增加Jito的小费(建议0.01SOL)，并考虑在链上活跃度较低的时段再次尝试。
{% endhint %}

通过 Jito 小费，将创建代币+多地址交易打包为一个捆绑包，确保交易不被狙击，并提升上链优先级，但需要消耗更多费用。

<figure><img src="../../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 确认交易

确认信息无误后，点击下&#x65B9;**「创建并买入」**&#x6309;钮，并等待开盘完成。


{% endstep %}
{% endstepper %}

## **常见失败案例**

* 若因 Jito 小费低于市场均值或遭机器人抢跑导致失败，请适当提高 Jito 小费并重试。
* 若因 RPC 节点或区块引擎响应延迟导致错失打包时机，请切换至其他更稳定的节点。
* 若因主钱包余额不足以支付建币费与租金等隐藏消耗，请确保额外预留至少 0.05 SOL 的缓冲资金。
* 若因代币头像档案过大导致上传逾时，请将图片压缩至 1MB 以内再重新发起操作。
* 若遇 Solana 链上极度壅塞引发底层随机丢包，请直接避开交易尖峰时段，稍后再试。

***

## **常见问题 FAQ**

<details>

<summary><strong>什么是 Bonk 创建并买入功能？</strong></summary>

这是一款针对 BONKfun 平台的代币极速发行工具。它能够将“创建代币”与“多个地址买入”这两个独立动作打包在同一个区块内同步执行，确保您 100% 在底部买入筹码，实现开盘及多地址持仓分布。

</details>

<details>

<summary><strong>为什么要将“创建”和“买入”捆绑在一起执行？</strong></summary>

Bonk 采用联合曲线定价机制，代币价格会随着买入量的增加而迅速上涨。如果先发币再手动买入，中间产生的时间差极易被链上狙击机器人监控并抢先买入，导致您被迫以数倍的高价接盘。捆绑执行消除了时间差，彻底阻断了恶意抢跑，保护了初始建仓的资金成本。

</details>

<details>

<summary><strong>这项功能可以用来优化代币早期的持币结构吗？</strong></summary>

可以。由于该功能支持批量导入多个钱包地址同步执行买入，这些买入会在代币创建的瞬间独立完成。这能让代币在刚发布时就展现出健康、分散的持币者分布数据，避免筹码过于集中在单一地址中。

</details>

<details>

<summary><strong>为什么“创建并买入”操作会一直提示失败？</strong></summary>

失败是由于该功能依赖于 Jito 的捆绑打包机制。在网络拥堵或节点延迟时，Jito 捆绑包很难被验证者顺利打包上链，从而导致较高的失败率。\
完全不会扣钱。 该操作是绑定的，一旦失败，代币不会发行，本金和手续费也不会有任何损耗。若需提高成功率，建议尝试增加 Jito 小费（推荐 0.001 SOL）、更换 RPC 节点/区块引擎，或在链上交易低谷期重新操作。

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
