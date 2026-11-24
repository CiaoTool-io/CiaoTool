---
description: >-
  CiaoTool Volume Bot automates token buys and sells on PancakeSwap V2/V3, with
  wallets and trade amounts configured in one place.
---

# BSC - Volume Bot Guide

{% hint style="info" %}
**CiaoTool PancakeSwap Market Making** supports all **V2 and V3** liquidity pool types. Please switch to the corresponding pool page to perform market-making operations based on your needs.
{% endhint %}

## Overview

The **CiaoTool BSC Volume Bot** is a no-code trading tool for PancakeSwap. To run repeated token buys and sells in a liquidity pool, select your trading pair, add participating wallets, and configure trade amounts in advance. Once started, the bot submits swaps according to your settings, eliminating the need to repeatedly switch wallets, enter amounts, and submit trades manually. As trades are executed, on-chain activity increases and trading volume accumulates in the selected pool.

{% hint style="info" %}
Select **V2** or **V3** based on your target liquidity pool. The same token may have liquidity in both versions, so confirm which pool you intend to trade in before starting.
{% endhint %}

<table data-card-size="large" data-view="cards"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td>PancakeSwap V2 Volume Bot</td><td><a href="https://bsc.ciaotool.io/zh-Hans/swap/v2/volume-bot-v2">https://bsc.ciaotool.io/zh-Hans/swap/v2/volume-bot-v2</a></td></tr><tr><td>PancakeSwap V3 Volume Bot</td><td><a href="https://bsc.ciaotool.io/zh-Hans/swap/v3/volume-bot-v3">https://bsc.ciaotool.io/zh-Hans/swap/v3/volume-bot-v3</a></td></tr></tbody></table>

***

## Step by Step

{% stepper %}
{% step %}
#### Connect Wallet <a href="#connect-wallet" id="connect-wallet"></a>

Click the button in the top right corner to connect a wallet that supports the EVM network.

<figure><img src="../../../.gitbook/assets/image (972).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Enter Token Address

{% hint style="info" %}
V2 / V3 layouts vary slightly. Click to switch and view the corresponding tutorial.
{% endhint %}

{% tabs %}
{% tab title="V2" %}
Select or enter the addresses of the Payment Asset and Trading Asset.\
The tool automatically detects the pair and displays its current price.

<figure><img src="../../../.gitbook/assets/image (15).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="V3" %}
Unlike V2 liquidity pools, each V3 liquidity pool with a different token pair and fee tier has a unique pool address; please enter the correct pair address to select the swap pair.

The tool automatically detects the pair and displays its current price.

<figure><img src="../../../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

**Can’t find the V3 Pool Address?**

{% content-ref url="../../../start/find-v3-token-pair-address.md" %}
[find-v3-token-pair-address.md](../../../start/find-v3-token-pair-address.md)
{% endcontent-ref %}
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Buy / Sell Setting

5 trade amount modes are available: **Fixed Amount**, **Random Range**, **Balance Percentage**, **Fixed Reserve**, and **Entire Balance**.

<figure><img src="../../../.gitbook/assets/image (32).png" alt=""><figcaption></figcaption></figure>

* **Fixed Amount:** Each wallet buys or sells using the specified fixed amount for every trade.
* **Random Range:** Each wallet buys or sells using a randomly selected amount within the specified range.
* **Balance Percentage:** Each wallet buys or sells using a specified percentage of its current balance.
* **Fixed Reserve:** Each wallet keeps the specified reserve amount and uses the remaining balance to buy or sell.
* **Entire Balance:** Each wallet uses its entire balance to buy or sell.
{% endstep %}

{% step %}
### Execution Settings

#### Buy and Sell Order

Determines whether each wallet buys or sells first. Each trade pair consists of one buy and one sell, executed sequentially.

#### Wallet Order

```
Round Robin: A → B → C → A → B → C → A → B → C
Random:      C → A → B → B → C → A → A → C → B (example)
Consecutive: A → A → A → B → B → B → C → C → C
```

* **Round Robin:** Wallets take turns in import order, each completing one buy-and-sell pair per cycle.
* **Random:** Wallet order is shuffled each cycle, with every wallet completing one buy-and-sell pair.
* **Consecutive:** Wallets run in import order. Each wallet completes all configured cycles before the next wallet starts.

#### Concurrency

The number of buy-and-sell pairs that can run simultaneously. The default is 1, with a maximum of 5 concurrent pairs.

Consecutive order only supports a concurrency of 1.

#### Trade Interval

Trade intervals are randomized within the specified range for more varied timing.

#### Stop Conditions

* **Cycle Count:** Automatically stops after completing the specified number of buy-and-sell cycles.
* **Price Range:** Set a price range for the payment asset. The bot automatically stops when the price moves outside this range. Consecutive order only supports Cycle Count.

#### Slippage and Transaction Deadline

Slippage limits the acceptable execution price deviation, while the transaction deadline sets the time limit for executing each swap. If a transaction fails or remains pending, the bot pauses further execution.

#### Gas Price and Swap Gas Limit

Gas Price is the cost per unit of gas. Swap Gas Limit is the maximum gas allowed for each swap. The actual network fee equals the gas consumed multiplied by the gas price.
{% endstep %}

{% step %}
### Import Trading Wallet Private Key

{% hint style="danger" %}
<mark style="color:red;">**Security Tips**</mark>

Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

Supports two import types for trading address private keys: "Manual Input" and "Upload File". Up to 20 addresses is supported.

1. Click the **"Import Private Key"** button to open the input pop-up.

<figure><img src="../../../.gitbook/assets/image (983).png" alt=""><figcaption></figcaption></figure>

2. Manually enter or import the private key file, and click confirm once the private key is displayed in the confirmation box.

<figure><img src="../../../.gitbook/assets/image (984).png" alt=""><figcaption></figcaption></figure>

Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.\
Click to download and view the template:

{% file src="../../../.gitbook/assets/EVM_Demo.xlsx" %}
{% endstep %}

{% step %}
### Enter Buy Amount

{% hint style="info" %}
Keep at least 0.0008 BNB in each wallet to cover gas fees.
{% endhint %}

Supports three trading amount types: **"Fixed Amount"**, **"Fixed Retain"**, and **"All Balance"**.

<figure><img src="../../../.gitbook/assets/image (985).png" alt=""><figcaption></figcaption></figure>

1. **Fixed Amount**\
   Swaps a set number of tokens across all wallets.
2. **Fixed Retain**\
   Keeps a set balance in wallets and swaps the rest.
3. **All Balance**\
   Swaps the entire wallet balance into the target token.
{% endstep %}

{% step %}
### Trading Setting

{% hint style="danger" %}
Closing / refreshing the page will **immediately stop** the bot strategy. Please ensure that the page remains open and running continuously in the background while the strategy is being executed. To ensure necessary strategy execution, **this feature is not recommended for use on mobile devices.**
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (986).png" alt=""><figcaption></figcaption></figure>

**Transaction Speed**\
Set higher priority fees to speed up block execution and frontrun MEV bots.

**Stop Methods**

* **Run Times:** Bot terminates automatically once the wallet swap loop hits your set limit.
* **Price Range:** Bot terminates automatically if the token price breaks outside your set boundary.

**Task Execution Interval**\
Randomizes the delay between multi-wallet orders to simulate organic retail trading.
{% endstep %}

{% step %}
### **Confirm** <a href="#confirm" id="confirm"></a>

After verifying all details, click the **"Start Swap"** button below and wait for the transaction process to complete.
{% endstep %}
{% endstepper %}

***

## Service Support

Need help? Join our community for real-time support:

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}

