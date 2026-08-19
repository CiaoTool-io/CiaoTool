---
description: CiaoTool 代币快照工具可帮助你在短时间内完成指定代币的持有人快照统计，适用于市值监控、精细化用户分析或空投分发准备。
---

# Solana  - 代币快照

{% hint style="success" %}
**Solana 代币快照：**[https://ciaotool.io/zh-CN/token/tokenTool/snapshot-token-holders](https://ciaotool.io/zh-CN/token/tokenTool/snapshot-token-holders)
{% endhint %}

#### **🎯 什么是 Solana 代币快照？**

Solana 代币快照是指在某一时间点，对代币持有者地址及其余额进行记录与导出，用于分析当前筹码分布情况。通过工具可以快速筛选、生成持仓数据，为空投、激励或市值管理提供关键依据。

**常见用途：**

* 空投名单：筛选符合条件的持币地址
* 用户分层：按持仓大小划分核心/普通用户
* 筹码分析：了解持币集中度与分布结构
* 精准营销：针对特定用户做活动或激励
* 市值管理：辅助制定控盘或释放策略

#### 一、选择代币

在输入框中填写目标代币地址，或点击下拉菜单选择当前钱包持有的代币。

<figure><img src="../../../.gitbook/assets/image (304).png" alt=""><figcaption></figcaption></figure>

#### 二、设置筛选规则

**✅ Top 筛选（可选）**

从预设选项中选择你要统计的前N名持有人：

* Top 100 / 500 / 1000 / 2000 / 5000 / 10000

系统将自动抓取该代币持有人排名靠前的钱包地址及其持有数量。

**✅ 自定义最低持仓（可选）**

如果你希望筛选掉“尘埃地址”或设置参与门槛，例如只保留持有量 ≥ 1000 的钱包，可以在此设定一个最小持币门槛。

<figure><img src="../../../.gitbook/assets/image (305).png" alt=""><figcaption></figcaption></figure>

#### 三、生成并导出快照

点击【生成快照】，系统将连接 Solana 链上数据并提取符合条件的钱包地址列表。\
完成后，你可以选择以下格式导出数据：

* CSV 文件（用于导入空投工具）

<figure><img src="../../../.gitbook/assets/image (307).png" alt=""><figcaption></figcaption></figure>

**⚠️ 常见失败案例**

* 快照时间选择不当，数据参考价值低
* 未过滤交易所或合约地址，影响结果准确性
* 地址格式或数据导出异常
* 使用过旧数据，导致策略偏差

#### ❓常见问题

**1. 快照工具支持哪些类型的代币？**

* [x] **答：** 支持所有符合 SPL 标准的代币，包括标准代币和 Token2022 类型。

**2. 快照可以筛选哪些地址？**

* [x] **答：** 可筛选 Top 100–10000 的持币地址，或设定最低持仓数量，自定义筛选精准用户。

**3. 快照结果能导出吗？**

* [x] **答：** 可以导出为 xlsx 文件，方便进行空投分发或市场分析。

**4. 快照的数据准确吗？**

* [x] **答：** 代币快照的数据是基于某一个区块高度或者时间的，过了这个时间，数据可能就会有变化。

**5. CiaoTool的代币快照工具需要收费吗？**

* [x] **答：** 不收费，该工具是免费使用的

**🔰 更多快捷工具 & 指南**

《 [Solana 一对多转账](https://ciaotool.io/zh-CN/wallet/manage/one-to-multi) 》《 [Solana 代币管理 ](https://ciaotool.io/zh-CN/token/management)》

**💬 如遇到问题？加入社群实时咨询**：[https://t.me/ciaotool](https://t.me/ciaotool)

* Email：[support@ciaotool.io](mailto:support@ciaotool.io)
* 官网：[https://ciaotool.io](https://ciaotool.io/)
* X（Twitter）：[https://x.com/CiaoTool](https://x.com/CiaoTool)
* Medium： [https://medium.com/@ciaotool](https://medium.com/@ciaotool)
* Blog：[https://www.ciaoailiquidity.com/zh/blog](https://www.ciaoailiquidity.com/zh/blog)
* YouTube：[https://www.youtube.com/@CiaoTool](https://www.youtube.com/@CiaoTool)
* WhatsApp：[https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J](https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J)

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
