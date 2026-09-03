---
description: 通过统一广播窗口向 Robinhood Chain 提交多个钱包的买入交易，减少逐笔发送产生的排队延迟和插队窗口，实现尽力而为的多地址并发执行。
---

# Robinhood Chain - 多地址并发买入教程

{% hint style="info" %}
**CiaoTool Uniswap 多地址并发买入**现已全面支持 **V2 / V3** 全部的流动性池类型，请先切换到指定池子功能页面进行市值管理操作，满足不同场景下的快捷多地址交易服务。
{% endhint %}

## CiaoTool Robinhood Chain 多地址并发买入是什么？

<figure><img src="../../../.gitbook/assets/image (700).png" alt="CiaoTool Robinhood 链 Uniswap V2 多地址捆绑买入 功能页面"><figcaption></figcaption></figure>

CiaoTool 多地址并发买入是一款面向 Robinhood Chain 时效性买入场景的多钱包自动化工具。

手动操作多个钱包时，每笔交易都需要分别准备、签名和提交。不同钱包之间的操作延迟会产生额外的排队窗口，在此期间，流动性池价格可能发生变化，其他交易也可能更早到达网络。

CiaoTool 会在执行前统一准备所有选中钱包的买入交易。用户确认任务后，交易将在浏览器本地完成签名，并通过一个较短的广播窗口并发提交。

与手动或逐笔顺序买入相比，这种统一并发广播方式可以缩短不同钱包之间的提交时间差，减少其他交易插入中间的机会，并提高多钱包买入的执行一致性。

### 核心优势

<table data-view="cards"><thead><tr><th></th><th></th></tr></thead><tbody><tr><td><strong>减少逐笔提交延迟</strong></td><td>逐个钱包提交交易会产生不必要的时间差。并发买入会预先准备交易并统一广播，无需等待前一个钱包的交易完成后再发送下一个钱包。</td></tr><tr><td><strong>减少排队与插入窗口</strong></td><td>不同钱包交易之间的提交间隔越长，其他交易插入其中的机会就越多。统一并发广播可以缩短这一时间窗口。</td></tr><tr><td><strong>提高买入一致性</strong></td><td>多个钱包在不同时间买入时，前面的交易可能已经改变池子状态，导致后续钱包获得更加不利的价格。并发提交有助于减少不同钱包之间的成交差异。</td></tr><tr><td><strong>简化多钱包协调</strong></td><td>用户可以通过一个页面统一设置多个钱包、买入金额、滑点和交易参数，无需逐个操作钱包。</td></tr><tr><td><strong>提高关键交易阶段的响应速度</strong></td><td>当用户需要在较短时间内提交多个买入交易时，并发广播可以提高整体响应速度，例如代币上线或其他具有时效性的买入场景。</td></tr></tbody></table>

### 常见用例

<table data-card-size="large" data-view="cards"><thead><tr><th></th><th></th></tr></thead><tbody><tr><td><strong>代币上线阶段买入</strong></td><td>在代币上线阶段，通过较短的广播窗口提交多个钱包的买入交易。</td></tr><tr><td><strong>多钱包建立仓位</strong></td><td>通过多个用户控制的钱包建立代币仓位，无需逐个切换钱包和手动提交交易。</td></tr><tr><td><strong>时效性买入执行</strong></td><td>当多个钱包需要在接近的时间提交买入交易时，减少逐笔操作产生的延迟。</td></tr><tr><td><strong>关键价格区间买入</strong></td><td>在滑点和池子流动性允许的情况下，协调多个钱包在用户选择的价格区间附近提交买入交易。</td></tr></tbody></table>

### 快速开始

立即在 Robinhood Chain 上，用 CiaoTool​ 多地址并发买入功能进行一键买入操作：

{% embed url="https://r.ciaotool.io/zh-Hans/swap/v2/multi-address-buy-v2" %}

{% embed url="https://r.ciaotool.io/zh-Hans/swap/v3/multi-address-buy-v3" %}

***

## 多地址并发买入在 Robinhood Chain 上如何工作？

### 交易排序机制

Robinhood Chain 使用**先到先得的排序机制**。交易顺序由每笔交易到达 Sequencer 的时间决定。根据 Robinhood Chain 官方说明，后到达的交易不能仅通过支付更高的费用绕过先到达的交易。

Robinhood Chain 的目标出块时间约为 **100 毫秒**，可以快速处理交易。但即使是很小的网络传播时间差或 Sequencer 到达时间差，也可能影响最终交易顺序。

可以查看 [Robinhood Chain 交易排序说明](https://docs.robinhood.com/chain/) 和 [网络基础设施介绍](https://robinhood.com/blockchain)。

### CiaoTool 的解决方案

在 Robinhood Chain 当前的交易提交模式下，CiaoTool 无法使用部分其他网络提供的捆绑通道，将多个独立钱包的买入交易组合成一个有顺序保证的交易单元。

每个交易钱包都是一个独立的 EVM 账户。每笔交易都有独立的私钥签名、Nonce、Gas 需求和交易哈希。这些独立签名的交易必须分别提交给 Robinhood Chain Sequencer。

因此，CiaoTool 采用统一并发广播策略：

1. 为每个钱包预先准备买入交易；
2. 在浏览器本地完成交易签名；
3. 在用户确认执行前保留已准备的交易；
4. 在较短时间窗口内统一触发交易广播；
5. 将每笔已签名交易分别提交到 Robinhood 链；
6. 分别跟踪每笔交易的执行结果。

{% hint style="warning" %}
**尽力执行机制**

**并发买入**采用尽力而为的广播策略。CiaoTool 会在极短的时间窗口内触发多笔交易广播，但无法保证这些交易以完全相同的时间到达、按照预设顺序执行、被打包进同一区块，或先于 MEV 机器人执行。

通过并发买入广播的交易可能进入同一区块、相邻区块或不同区块。交易最终的到达时间、执行顺序和确认结果取决于多种因素，包括用户的网络速度和延迟、设备及浏览器性能、RPC 的响应速度与可用性、Robinhood Chain 当前的链上活跃程度、区块时间、排序器负载以及流动性池状态。

即使 CiaoTool 几乎同时触发多笔交易广播，网络或 RPC 延迟仍可能导致部分钱包的交易晚于其他交易到达 Robinhood Chain 排序器。
{% endhint %}

### 与捆绑技术的差异

<table data-search="false"><thead><tr><th>对比项目</th><th>并发买入</th><th>捆绑买入</th></tr></thead><tbody><tr><td>提交方式</td><td>在较短时间窗口内广播多笔独立交易</td><td>将多笔交易组合成一个捆绑包后统一提交</td></tr><tr><td>交易排序</td><td>不保证，由每笔交易到达 Sequencer 的时间决定</td><td>保留预先设定的内部交易顺序</td></tr><tr><td>同区块执行</td><td>不保证，交易可能进入同一区块、相邻区块或不同区块</td><td>是，所有捆绑包内交易在同一区块执行</td></tr><tr><td>原子执行</td><td>否，每个钱包的交易相互独立</td><td>是，整个捆绑以原子方式执行</td></tr><tr><td>失败处理</td><td>每笔交易可以独立成功或失败</td><td>所有交易必须全部成功，任意一笔失败都会导致整个捆绑回滚</td></tr><tr><td>交易哈希</td><td>每个钱包都有独立的交易哈希</td><td>每笔交易仍可在捆绑包执行中进行追踪</td></tr><tr><td>MEV 防护</td><td>尽力而为，MEV 机器人偶尔可能更早到达 Sequencer</td><td>捆绑包执行可以减少外部交易插入内部交易之间的机会</td></tr><tr><td>执行结果</td><td>取决于网络延迟、RPC 状态、Sequencer 到达时间和池子状态</td><td>按照预先设定的捆绑顺序统一执行</td></tr></tbody></table>

***

## **分步式教程**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角按钮，绑定支持 Robinhood 链的钱包

<figure><img src="../../../.gitbook/assets/image (656).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入支付钱包私钥

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

当前功能仅支持 私钥导入以进行支付操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (668).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 输入币对地址

V2  在代币输入框中选择 /输入做市代币地址，V3 请输入指定池子的币对合约地址。

<figure><img src="../../../.gitbook/assets/image (669).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (670).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入并发买入私钥地址

{% hint style="danger" %}
<mark style="color:$danger;">**安全须知**</mark>

当前功能仅支持 私钥导入以进行多地址买入操作。请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

1. 点&#x51FB;**「导入私钥」**&#x6309;钮，弹出上传弹窗。

<figure><img src="../../../.gitbook/assets/image (671).png" alt=""><figcaption></figcaption></figure>

2. 支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入钱包私钥的类型，最多支持 **20 个地址**捆绑买入。

<figure><img src="../../../.gitbook/assets/image (672).png" alt=""><figcaption></figcaption></figure>

使用 CiaoTool 模板文件导入，并保存确定导入并显示在输入框内。\
点击下载并查看模板：

{% file src="../../../.gitbook/assets/EVM_privateKey_demo.xlsx" %}
{% endstep %}

{% step %}
### 输入买入金额

支持两种交易金额类型：“自定义输入”和“全部”。

1. **自定义输入**\
   为每个钱包单独输入交易金额。\
   如果填写了金额，则转账将使用该金额。\
   如果金额留空，则转账将默认使用全局设置中配置的金额。
2. **全部**   \
   将整个钱包余额兑换成目标代币。
{% endstep %}

{% step %}
### 确认交易

提交任务前，请仔细核对所有参数。页面会在执行前显示所有适用费用。

确认信息无误后，点击下&#x65B9;**「代币买入」**&#x6309;钮，并等待交易完成。

<figure><img src="../../../.gitbook/assets/image (674).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

***

## 常见问题

<details>

<summary><strong>什么是多地址并发买入？</strong></summary>

多地址并发买入会预先准备多个钱包的买入交易，并在较短时间窗口内统一广播，从而减少逐个钱包提交交易产生的延迟。

</details>

<details>

<summary><strong>并发买入和捆绑买入相同吗？</strong></summary>

不同。并发买入会在接近的时间广播多笔独立交易；捆绑买入则通过网络支持的捆绑机制组合交易。并发交易不是原子交易，也不保证进入同一区块。

</details>

<details>

<summary><strong>为什么 Robinhood 链使用并发买入而不是捆绑买入？</strong></summary>

在 Robinhood Chain 当前的交易提交模式下，CiaoTool 无法将多个用户控制钱包的独立签名交易组合成一个具有顺序保证的捆绑包。每笔交易都必须分别提交给 Sequencer。

</details>

<details>

<summary><strong>所有交易都会进入同一区块吗？</strong></summary>

不一定。并发广播可以提高交易被集中处理的可能性，但交易可能进入同一区块、相邻区块或不同区块。

</details>

<details>

<summary><strong>并发买入可以防止 MEV 机器人吗？</strong></summary>

不能完全防止。并发买入可以减少逐笔提交产生的延迟和暴露窗口，但不能保证防止 MEV 机器人。低延迟机器人偶尔可能更早到达 Sequencer。

</details>

<details>

<summary><strong>为什么不同钱包的成交价格可能不同？</strong></summary>

每个钱包都会提交一笔独立交易。每次买入成功后，池子状态都可能发生变化，其他交易也可能在 CiaoTool 的交易之间执行。滑点和池子流动性同样会影响最终成交价格。

</details>

<details>

<summary><strong>如果其中一个钱包交易失败会怎样？</strong></summary>

每个钱包的交易都是独立的。某笔交易失败不会自动撤销其他已经成功的交易。链上交易即使失败，也可能消耗 Gas。

</details>

<details>

<summary><strong>CiaoTool 如何保护导入的私钥？</strong></summary>

CiaoTool 采用完全客户端签名机制。私钥只在浏览器本地处理，不会被上传、传输、存储、记录或写入 Local Storage。关闭或刷新页面后，已导入的私钥数据将被清除。

</details>

***

## 联系我们

**如遇到问题？**&#x4F60;可以通过以下方即时联系 CiaoTool 团队：

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
