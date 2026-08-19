---
description: Solana 冻结账户功能允许持有权限的账户暂时限制指定钱包的代币转出，防止恶意操作，保障资产安全。
---

# Solana - 冻结账户教程

{% hint style="success" %}
**Solana 冻结账户：**[https://ciaotool.io/zh-CN/token/freeze-account](https://ciaotool.io/zh-CN/token/freeze-account)
{% endhint %}

#### **🎯 什么是 Solana 冻结账户（黑名单）？**

Solana 冻结账户功能，也称“黑名单”，允许项目方通过 **Freeze Authority（冻结权限）** 阻止特定钱包执行代币相关操作，如转账或交易。该功能有助于防止恶意行为（如机器人操纵、套利攻击）对资产造成损害，同时为项目方提供更多控制手段，以优化市场策略和社区治理。

**常见用途：**

* 防护机器人：阻止恶意地址操纵市场或套利
* 风险控制：冻结异常账户，减少资产被滥用风险
* 活动管理：限制部分账户参与空投或激励
* 项目治理：黑名单违规用户，维护公平性
* 市场策略：在特定阶段控制流通筹码，优化开盘或价格节奏

#### 🧊 **如何冻结账户？**

**1. 连接钱包**

* 点击右上&#x89D2;**【连接钱包】**，选择钱包地址并确认授权。
* 页面右上角显示钱包地址即表示绑定成功

<figure><img src="../../../.gitbook/assets/image (302).png" alt=""><figcaption></figcaption></figure>

**2. 选择代币**

* 粘贴代币地址或下拉选择钱包内的代币。

![](https://docs.dogtools.meme/~gitbook/image?url=https%3A%2F%2F4028514454-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252Ft1j9LpucEChNmzQ1XqQO%252Fuploads%252F6CMikl9kp2S6kkPGswYs%252Fimage.png%3Falt%3Dmedia%26token%3D3a3d9606-258c-4378-9da9-f163d65d67dd\&width=768\&dpr=4\&quality=100\&sign=f7ccb818\&sv=2)

#### ⛓️ **交易流程**

* 任务开始执行时，会出现日志弹框为您实时更新交易进度。（需要一次交易签名）。
* 任何环节出了问题，我们都会为你清晰透出。操作失败不会收取任何费用。

**⚠️ 常见失败案例**

* 未持有 Freeze 权限，无法执行冻结操作
* 冻结错误地址，影响正常用户操作
* 多签或权限设置错误，导致无法解除冻结
* 操作未成功上链，但误以为已冻结
* 频繁冻结/解冻触发链上限制或延迟

![](https://docs.dogtools.meme/~gitbook/image?url=https%3A%2F%2F4028514454-files.gitbook.io%2F%7E%2Ffiles%2Fv0%2Fb%2Fgitbook-x-prod.appspot.com%2Fo%2Fspaces%252Ft1j9LpucEChNmzQ1XqQO%252Fuploads%252FXeeLJe4zNeykTEOviIGz%252Fimage.png%3Falt%3Dmedia%26token%3D70040d64-762e-40d0-a678-df4356c88659\&width=768\&dpr=4\&quality=100\&sign=b391782a\&sv=2)

#### ❓ 常见问题 <a href="#chang-jian-wen-ti" id="chang-jian-wen-ti"></a>

**1. 什么是冻结账户功能？**

* [x] 答：冻结账户是指暂时限制某个钱包地址对代币的转账和交易权限。

**2. 谁有权限冻结账户？**

* [x] 答：只有持有代币 Freeze 权限的账户才能执行冻结操作。

**3. 被冻结的账户还能接收代币吗？**

* [x] 答：可以，冻结只限制转出和交易，不影响接收。

**4. 冻结账户后如何解冻？**

* [x] 答：持有 Freeze 权限的账户可以随时发起解冻操作。

**5. 冻结账户会影响代币的正常流通吗？**

* [x] 答：只影响被冻结的账户，不会影响整体代币流通。

**🔰 更多快捷工具 & 指南**

《 [Solana 代币管理](https://ciaotool.io/zh-CN/token/management) 》《 [Solana 解冻账户](https://ciaotool.io/zh-CN/token/unfreeze-account) 》《 [Solana 代币快照](https://ciaotool.io/zh-CN/token/tokenTool/snapshot-token-holders) 》

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
