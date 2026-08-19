---
description: 同一个代币交易对可能存在多个不同手续费等级的 V3 Pool。每个 Pool 都有独立的合约地址、流动性深度、价格和交易活动。
---

# 如何查找 V3 币对地址教程 | CiaoTool

## 什么是 V3 Pool Address？

V3 Pool Address 是某个特定 V3 流动性池的智能合约地址，由以下条件共同确定：

* 所属区块链网络；
* DEX 和协议版本；
* Token0；
* Token1；
* 手续费等级。

与 V2 不同，同一组代币可能存在多个不同手续费等级的 V3 Pool。例如，Token A 和 Token B 可能分别存在 0.01%、0.05%、0.30% 或 1.00% 手续费等级的 V3 Pool。

这些 Pool 分别拥有不同的 Pool Address、流动性深度、当前价格、交易活动和成交结果。

根据 V3 的合约架构，一个 Pool 由两种代币和手续费等级共同确定。因此，同一交易对可以存在多个手续费等级不同的 Pool。[查看 Uniswap V3 架构说明](https://developers.uniswap.org/docs/protocols/v3/concepts/architecture)。

***

## 为什么必须使用准确的 Pool Address？

当 V3 工具要求输入 Pool Address 时，仅输入代币合约地址是不够的。

准确的 Pool Address 可以帮助 CiaoTool 确定需要使用哪个流动性池，从而：

* 读取池子当前价格；
* 识别 Token0 和 Token1；
* 确认手续费等级；
* 估算流动性和价格影响；
* 构建 Swap 路径；
* 将交易提交至目标 Pool。

如果输入错误的 Pool Address，页面可能加载错误的代币交易对、选择非预期的手续费等级、显示错误的市场数据，或者无法正常提交交易。

***

## 开始前准备

请提前准备以下信息：

* 目标区块链网络；
* 基础代币合约地址；
* 报价代币合约地址；
* 目标 DEX；
* 协议版本，例如 V3；
* 目标手续费等级。

请始终使用准确的**代币合约地址**进行搜索，不要只搜索代币名称或符号。不同代币可能使用完全相同的名称和符号。

***

## 分步式教程

许多第三方链上数据工具都可以快速查询某个代币当前存在的全部流动性池。

本教程将以 **DEXTools** 为例，用户只需搜索代币合约地址，即可比较该代币在不同区块链网络、DEX、协议版本、报价代币和手续费等级下的 Pool。

{% stepper %}
{% step %}
### 打开 DEXTools

访问 DEXTools 官方网站

<figure><img src="../.gitbook/assets/image (689).png" alt=""><figcaption></figcaption></figure>

{% embed url="https://www.dextools.io/app/hot-pairs" %}
{% endstep %}

{% step %}
### 选择正确的网络

选择目标 V3 Pool 所在的区块链网络。

相同的代币名称或相似格式的合约地址可能出现在不同网络中。请确保 DEXTools 当前选择的网络与 CiaoTool 使用的网络一致。

<figure><img src="../.gitbook/assets/image (690).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 搜索代币合约地址

将准确的代币合约地址粘贴到 DEXTools 搜索框中。

与只搜索代币名称或符号相比，通过合约地址搜索更加准确，也可以降低选择仿冒代币的风险。

显示搜索结果后，请核对：

* 代币名称；
* 代币符号；
* 代币合约地址。
{% endstep %}

{% step %}
### 查看代币的全部池子

选择目标代币，并进入对应的 Pair Explorer 页面。

<figure><img src="../.gitbook/assets/image (691).png" alt=""><figcaption></figcaption></figure>

DEXTools 可能会优先显示其中一个活跃或推荐交易对。如需查看该代币的其他 Pool，可以打开 Pool 选择区域、**Other Pairs**，或者点击 Pool 信息附近的望远镜图标。

DEXTools 更新界面后，按钮的名称或位置可能发生变化。

<figure><img src="../.gitbook/assets/image (692).png" alt=""><figcaption></figcaption></figure>

请根据以下信息比较可用 Pool：

* DEX 名称；
* 协议版本；
* 报价代币；
* 流动性；
* 交易量；
* Pool 创建时间；
* 手续费等级，如页面显示。
{% endstep %}

{% step %}
### 复制 Pair Address

找到与 CiaoTool 当前任务完全对应的 Pool。

<figure><img src="../.gitbook/assets/image (693).png" alt=""><figcaption></figcaption></figure>

请确认：

* 区块链网络正确；
* Pool 属于目标 DEX；
* 协议版本为 V3；
* 两种代币的合约地址正确；
* 报价代币正确；
* 手续费等级正确；
* Pool 拥有符合预期的流动性。

请勿仅因为某个 Pool 的交易量或流动性最高就直接选择。Pool Address 必须首先与任务所需的网络、DEX、代币交易对、协议版本和手续费等级完全一致。
{% endstep %}

{% step %}
### 将币对输入 CiaoTool

返回对应的 CiaoTool V3 功能页面，将复制的币对地址粘贴到输入框中。

<figure><img src="../.gitbook/assets/image (694).png" alt=""><figcaption></figcaption></figure>

页面加载 Pool 后，请检查 CiaoTool 识别出的信息：

* 代币交易对；
* 代币符号；
* 手续费等级；
* 当前价格；
* Pool 流动性；
* 买入或卖出方向。

只有当页面显示的信息与 DEXTools 中选择的 Pool 完全一致时，才继续下一步操作。
{% endstep %}
{% endstepper %}

***

## 常见错误

#### 复制了代币地址

代币合约地址只代表一种代币，并不能代表具体的 V3 流动性池。

#### 选择了错误的网络

相同名称的代币可能出现在多个区块链网络中。

#### 选择了错误的 DEX

同一个代币可能在多个 DEX 上拥有流动性池，不同 DEX 使用不同的 Pool 合约。

#### 选择了 V2 或 V4 Pool

DEXTools 可能会同时显示多个协议版本的 Pool。
