---
description: >-
  专为 Pump.fun 和 PumpSwap
  平台提供的高频微量交易执行工具。通过全自动执行连续的小额买卖交互，持续触发平台的活跃度排序机制，确保代币维持在首页前列，以极低成本最大化项目的市场曝光度与真实流量。
---

# Pump - 微单交易机器人指南

{% hint style="info" %}
**CiaoTool Pump 微单交易机器人**现已全面支持官方 **SOL** 和 **USDC** 全部的价值代币，输入代币地址将自动切换池子适配和价值代币。
{% endhint %}

## 功能介绍

**CiaoTool Pump 微单交易机器人**是一款面向 Pump.fun 与 PumpSwap 的自动化曝光工具。用户可自定义微额交易金额和执行间隔，由系统持续完成多地址、小金额的买卖操作。

该功能利用 Pump.fun 按近期交易活跃度展示代币的机制，通过持续产生微额链上交易，让代币保持活跃状态，增加其在首页及近期活跃列表中的展示机会，从而提升项目曝光度并吸引更多用户关注。

立即在 Pump.fun 和 PumpSwap 上，用 CiaoTool 微单交易机器人进行多地址自动买卖操作：

{% embed url="https://ciaotool.io/zh-Hans/pump/micro-trading" %}

***

## 核心优势

* **提升曝光机会：** 持续更新代币交易状态，增加首页及活跃列表的展示机会
* **微额低成本：** 通过小额交易控制单次执行成本与价格影响
* **多地址交易：** 自动调度多个钱包执行买入和卖出操作
* **参数灵活：** 支持自定义交易金额、执行间隔和运行次数
* **自动循环：** 一键启动并持续执行，无需频繁手动操作
* **本地签名：** 私钥仅在浏览器本地用于交易授权，无需上传

***

## **图文指南**

{% stepper %}
{% step %}
### **绑定钱包**

点击右上角【连接钱包】按钮，绑定支持 Solana 链的钱包

<figure><img src="../../../.gitbook/assets/image (748).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 选择交易代币

可以选择输入代币地址，也可以选择当前钱包拥有的代币进行交易。系统将自动识别锚定价值代币并匹配所在池位置。

<figure><img src="../../../.gitbook/assets/image (896).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 导入钱包私钥

{% hint style="danger" %}
请确保在安全环境下输入私钥信息，您的资金安全对我们来说至关重要，[**了解更多 CiaoTool 如何保障您的资金安全：资金安全保障**](../../../security-guide.md)**。**
{% endhint %}

{% hint style="info" %}
<mark style="color:$primary;">**操作钱包设置**</mark>

导入钱包没有数量限制。交易手续费由每个钱包独立支付。
{% endhint %}

导入钱包数量没有限制，支&#x6301;**「手动输入」**&#x548C;**「上传文件」**&#x4E24;种导入来源地址的类型，选择以查看详细教程

{% tabs %}
{% tab title="手动输入" %}
1. 点&#x51FB;**「批量输入」**&#x6309;钮，弹出手动输入框。

<figure><img src="../../../.gitbook/assets/image (846).png" alt=""><figcaption></figcaption></figure>

2. 输入 / 批量粘贴**钱包地址，**&#x6BCF;行仅输入一个钱包私钥，可在私钥后追加数量。

```
privateKey, 300
```

<figure><img src="../../../.gitbook/assets/image (737).png" alt=""><figcaption></figcaption></figure>

3. 点&#x51FB;**「确定导入」**，将所有输入地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (850).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="上传文件" %}
1. 下载 CiaoTool 模板文件，并将信息导入到文件内。

<figure><img src="../../../.gitbook/assets/image (847).png" alt=""><figcaption></figcaption></figure>

2. 点击![](<../../../.gitbook/assets/image (848).png>)**「导入文件」**&#x6309;钮，弹出文件上传窗口。
3. 点&#x51FB;**「确定导入」**，将所有地址导入到操作面板

<figure><img src="../../../.gitbook/assets/image (849).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### 循环设置

设置买入价格范围和钱包交易顺序，每次交易将在预设范围内进行。

<figure><img src="../../../.gitbook/assets/image (910).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 钱包间隔



可自由设置各地址完成一次买卖交易循环的执行间隔时间。

<figure><img src="../../../.gitbook/assets/image (911).png" alt=""><figcaption></figcaption></figure>

* **固定时间**\
  所有交易按固定时间提交广播。
* **随机时间**\
  将会在指定的时间范围内随机提交，模拟真实交易。
{% endstep %}

{% step %}
### 发送设置

* **RPC 发送**\
  RPC 发送策略是尽力而为，无需支付 Jito 小费。通过统一买卖交易广播交易，但不保证在同一区块内，可能会被机器人狙击造成损失。
* **Jito Bundle**\
  通过 Jito 小费，将买卖交易打包为一个捆绑包，确保买卖交易不被狙击，并提升上链优先级，但需要消耗更多费用。

<figure><img src="../../../.gitbook/assets/image (857).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 启动交易

{% hint style="danger" %}
关闭 / 刷新页面，机器人策略亦会**立即停止**。请保持策略执行期间，将网页持续处于后台并运行状态。为保证策略执行之必要，**该功能不推荐于**「**移动电子设备**」**使用。**
{% endhint %}

交易费用将由各钱包独立承担。确认信息无误后，点击下方「**确认并开始微量循环交易**」按钮，即可开启交易程序。

<figure><img src="../../../.gitbook/assets/image (912).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### 核实信息

程序自动运行，可实时查看交易情况：

* [x] 成功买入次数
* [x] 成功卖出次数
* [x] 失败和停止步骤

<figure><img src="../../../.gitbook/assets/image (913).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

***

## **常见问题**

<details>

<summary><strong>什么是 Pump 微单交易机器人？</strong></summary>

这是专为维持盘口活跃状态打造的自动化执行工具。系统会持续向 Pump.fun 发起微量资金的双向交互，借助平台的数据更新机制，确保代币的交易状态实时刷新，以此维持项目在首页的可见性。

</details>

<details>

<summary><strong>这与普通的「交易量机器人」有什么区别？</strong></summary>

两者的核心目的完全不同。普通的「交易量机器人」侧重于使用较大的资金进行买卖，目的是为了优化代币的总交易额数据；而「微量买卖」侧重于「交易频次」而非金额，它使用极其微小的资金高频交互，纯粹是为了获取并维持在平台首页的“曝光度”。

</details>

<details>

<summary><strong>为什么这种操作能让项目停留在 Pump.fun 首页？</strong></summary>

Pump.fun 平台的前端展示列表默认是按照代币的「最新一笔交易发生时间」进行排序的。微量买卖机器人通过高频次地产生最新交易记录，不断将您的代币顶回列表最上方，从而实现持续的曝光。

</details>

<details>

<summary><strong>运行微量买卖会导致我的资金快速消耗吗？</strong></summary>

消耗极低。因为该功能设定的单笔买卖金额非常微小，您的本金在买入和卖出之间是相互回滚流转的。主要的损耗仅为极少的 Solana 网络 Gas 费用以及 Pump.fun 平台针对这部分极小额度收取的微量手续费。

</details>

<details>

<summary><strong>开启这个功能会影响代币的价格走势吗？</strong></summary>

几乎没有影响。由于每次交互的资金量极小，它不足以在联合曲线上推动价格发生实质性的上涨或下跌。它在盘面上仅表现为密集的活跃记录点，完全不会破坏原有的价格走势与盘口结构。

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
