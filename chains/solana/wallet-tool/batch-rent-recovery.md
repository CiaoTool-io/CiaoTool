---
description: >-
  在 Solana 链上，大量无用代币账户和 NFT 账户会持续占用存储空间并锁定 SOL 租金。通过 CiaoTool
  的批量租金回收工具，您可以轻松回收多个地址的空账户、代币账户或 NFT 账户，统一释放 SOL 资金，提高资产利用率。
---

# Solana 批量租金回收教程

{% hint style="success" %}
**Solana 批量租金回收：**[https://ciaotool.io/zh-CN/wallet/claim-rent-batch](https://ciaotool.io/zh-CN/wallet/claim-rent-batch)
{% endhint %}

#### 🔗 操作步骤

**第 1 步：导入钱包**

* 可选择手动输入私钥或上传包含多个私钥的 CSV 文件。
* 系统将扫描每个钱包下的账户使用情况。

**第 2 步：选择回收类型**

* ✅ **仅回收空账户**：自动识别余额为零的账户并关闭。
* 🔁 **回收所有账户**：包括可销毁的代币和 NFT 账户，将资产烧毁后关闭账户。

<figure><img src="../../../.gitbook/assets/image (280).png" alt=""><figcaption></figcaption></figure>

**第 3 步：配置 SOL 回收地址**

* 默认将释放的 SOL 回收到原账户。
* 也可手动指定一个**统一接收地址**，用于集中管理回收的租金。

**第 4 步：代付设置（可选）**

* 支持由一个钱包为其他地址支付 GAS（手续费），适用于空投地址或未留 SOL 的账号回收。

<figure><img src="../../../.gitbook/assets/image (281).png" alt=""><figcaption></figcaption></figure>

**第 5 步：执行回收操作**

* 点击【开始回收】，系统将自动发起批量交易，每笔交易均由本地签名完成。
* 可实时查看处理状态与释放的 SOL 数量。

#### ❓常见问题

**1. 可以回收哪些账户类型？**

* [x] 答： 包括 SPL Token 账户、NFT 账户、空余额账户，只要不再使用都可以释放对应租金。

**2. 是否可以将所有 SOL 统一回收到一个地址？**

* [x] 答： 可以。你可以手动设定一个回收地址，所有释放的 SOL 将集中转入该地址，便于统一管理。

**3. 导入的钱包没有 GAS（SOL）还能回收吗？**

* [x] 答： 可以。如果开启“代付功能”，系统会使用你指定的钱包为其他钱包代付手续费，实现低成本批量操作。

**4. 是否支持批量处理多个地址的账户？**

* [x] 答： 支持。你可以批量导入多个钱包（私钥/JSON），统一执行账户扫描和回收操作。

**💬 如遇到问题？加入社群实时咨询**：[https://t.me/ciaotool](https://t.me/ciaotool)

* **Email**：[support@ciaotool.io](mailto:support@ciaotool.io)
* **官网**：[https://ciaotool.io](https://ciaotool.io/)
* **X（Twitter）**：[https://x.com/CiaoTool](https://x.com/CiaoTool)
* **Medium**： [https://medium.com/@ciaotool](https://medium.com/@ciaotool)
* **Blog**：[https://www.ciaoailiquidity.com/zh/blog](https://www.ciaoailiquidity.com/zh/blog)
* **YouTube**：[https://www.youtube.com/@CiaoTool](https://www.youtube.com/@CiaoTool)
* **WhatsApp**：[https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J](https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J)

{% hint style="danger" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
