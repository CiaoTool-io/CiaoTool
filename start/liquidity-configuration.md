---
description: >-
  流动性不足往往会导致高滑点、价格剧烈波动以及 bot
  狙击，直接影响市场对项目的信任度。从实操角度出发，给出不同类型项目在主流公链上的合理流动性区间参考，帮助你在稳定性与资金效率之间取得平衡。
metaLinks:
  alternates:
    - https://app.gitbook.com/s/b56FKZGe1viFi67H1pPQ/liquidity-configuration
---

# Token 流动性该如何配置？

{% hint style="success" %}
**Solana 发币：**[https://ciaotool.io/zh-CN/token/create](https://ciaotool.io/zh-CN/token/create)

**Pump：**[https://ciaotool.io/zh-CN/pump/launch-and-buy](https://ciaotool.io/zh-CN/pump/launch-and-buy)

**Bonk：**[https://ciaotool.io/zh-CN/letsbonkZone/bundled-buy](https://ciaotool.io/zh-CN/letsbonkZone/bundled-buy)
{% endhint %}

{% hint style="success" %}
**BSC 发币：**[https://bsc.ciaotool.io/token/create-token](https://bsc.ciaotool.io/token/create-token)

**Fourmeme：**[https://bsc.ciaotool.io/fourmeme/bnb/create-and-buy](https://bsc.ciaotool.io/fourmeme/bnb/create-and-buy)

**Flap：**[https://bsc.ciaotool.io/flap/usd1/create-and-buy](https://bsc.ciaotool.io/flap/usd1/create-and-buy)
{% endhint %}

{% hint style="success" %}
**Base 发币：**[https://base.ciaotool.io/token/create-token](https://base.ciaotool.io/token/create-token)
{% endhint %}

***

### 📈 为什么流动性很关键？

* **交易顺畅度：**&#x6D41;动性直接影响滑点大小。流动性越低，单笔交易对价格的冲击越大，交易越不顺畅。
* **价格稳定性：**&#x66F4;高的流动性能有效吸收买卖波动，提升价格稳定性，但同时也会带来更高的资金占用成本。
* **操纵风险与匹配度**：流动性不足时，池子更容易被操纵；但流动性并非越多越好，过高的流动性还会放大潜在的无常损失。关键在于流动性配置是否与项目所处阶段相匹配。

***

### 📊 先确定你的流动性等级

无论在哪条链上发币，你都需要先判断项目所处的流动性等级，这会直接影响投资者预期和价格行为。

* **极低流动性：**&#x5B9E;验性项目或低成本 Meme，滑点高，极易被 bot 操纵。
* **低流动性：**&#x521D;期项目，有少量社区，但价格仍不稳定。
* **中等流动性：**&#x5DF2;有一定用户和交易频率，价格相对可控。
* **高流动性**：成熟项目阶段，市场信任度明显提升。
* **极高流动性：**&#x8D44;金雄厚或已验证成功的项目，几乎不易被操纵。

***

### 🔗 不同区块链的流动性参考区间

* 下表基于实际市场情况整理，用于帮助你快速定位合理区间（非硬性标准）：

<table><thead><tr><th width="107.41796875" align="center">流动性等级</th><th align="center">Solana (Raydium)</th><th align="center">Solana (PumpSwap)</th><th align="center">BSC (BNB)</th><th align="center">Base</th></tr></thead><tbody><tr><td align="center">极低</td><td align="center">1 – 100 SOL</td><td align="center">1 – 25 SOL</td><td align="center">0.15 – 15 BNB</td><td align="center">0.1 – 5 WETH</td></tr><tr><td align="center">低</td><td align="center">101 – 500 SOL</td><td align="center">26 – 125 SOL</td><td align="center">15 – 75 BNB</td><td align="center">6 – 25 WETH</td></tr><tr><td align="center">中等</td><td align="center">501 – 2,000 SOL</td><td align="center">126 – 500 SOL</td><td align="center">75 – 300 BNB</td><td align="center">26 – 100 WETH</td></tr><tr><td align="center">高</td><td align="center">2,001 – 10,000 SOL</td><td align="center">501 – 2,500 SOL</td><td align="center">300 – 1,500 BNB</td><td align="center">101 – 500 WETH</td></tr><tr><td align="center">极高</td><td align="center">>10,000 SOL</td><td align="center">>2,500 SOL</td><td align="center">>1,500 BNB</td><td align="center">>500 WETH</td></tr></tbody></table>

![](<../.gitbook/assets/image (6)>)

### ⚠️ 流动性不足会带来哪些直接问题？

* **流动性不足的影响：**&#x5F53;流动性不足时，滑点会被显著放大，直接影响交易体验；同时，池子也更容易成为 bot 抢跑和拉砸的目标，增加市场风险。
* **流动性管理的必要性：**&#x5373;便通过提高流动性可以在一定程度上缓解上述问题，仍需关注无常损失，尤其是在价格波动剧烈的阶段。因此，流动性需要进行动态管理，而不是一次性投入。

***

### 🔎 是否应该把全部 Token 都放进池子？

* 通常不建议。更合理的做法是将 **40%–70%** 的 Token 用于流动性，其余部分留作**质押激励、生态奖励、社区运营或未来空投。**
* 这种结构既能保证交易深度，也能为项目后续发展保留空间。

![Token Allocation 示例](<../.gitbook/assets/image (7)>)

***

流动性是 Token 的基础设施。在不同公链上，区间虽有差异，但核心逻辑一致：

> 足够的流动性 = 更稳定的价格 + 更高的市场信任 + 更低的操纵风险

提前规划流动性等级与 Token 分配，是避免项目在早期阶段“死在起跑线”的关键一步。

***

**💬 如遇到问题？加入社群实时咨询**：[https://t.me/ciaotool](https://t.me/ciaotool)

* **Email**：[support@ciaotool.io](mailto:support@ciaotool.io)
* **官网**：[https://ciaotool.io](https://ciaotool.io/)
* **X（Twitter）**：[https://x.com/CiaoTool](https://x.com/CiaoTool)
* **Medium**： [https://medium.com/@ciaotool](https://medium.com/@ciaotool)
* **Blog**：[https://www.ciaoailiquidity.com/zh/blog](https://www.ciaoailiquidity.com/zh/blog)
* **YouTube**：[https://www.youtube.com/@CiaoTool](https://www.youtube.com/@CiaoTool)
* **WhatsApp**：[https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J](https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J)

{% hint style="warning" %}
CiaoTool 致力于提供便捷的工具服务，但不构成任何投资建议。平台内容可能根据产品迭代进行调整，敬请用户自行判断并留意更新。
{% endhint %}
