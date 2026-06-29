---
description: >-
  An automated market-making and trading tool built for meteora. Increasing
  token trading activity, simulate real on-chain trading, and improve the
  natural appearance of market activity and order flow.
---

# Meteora - Market Making Tutorial

## What is CiaoTool Meteora Market Making?

<figure><img src="../../../.gitbook/assets/image (797).png" alt="CiaoTool Solana Toolkit Page about Meteora Market Making Feature"><figcaption></figcaption></figure>

**CiaoTool Meteora Market Marking** is an advanced automated market-making and liquidity optimization tool custom-built for the Solana ecosystem. It allows project teams and professional groups to fully automate the execution of advanced market-making strategies on **Meteora** by customizing trading parameters, thereby safely and robustly managing token order book depth and market activity.

Compared to manual trading, which is cumbersome and difficult to control precisely, the core advantage of this feature lies in its fully automated strategy execution engine. The system can intelligently schedule multiple wallet addresses to conduct continuous, natural, two-way buy and sell interactions based on a set frequency and scale. This not only effectively optimizes the token's holder distribution and unique trading address structure, but also makes on-chain trading behaviors closer to authentic, natural market participation, comprehensively enhancing the naturalness of overall data performance.

Key Use Cases:

* **Smart Price Boosting**\
  Steadily optimizing the token's price presentation through reasonable order book interaction parameters.
* **Smooth and Orderly Retracement**\
  Smoothly managing the price retracement trajectory to prevent drastic market volatility.
* **Continuous Activity Enhancement**\
  Executing buy and sell operations through multi-address and randomized interval mechanisms to steadily increase trading volume and comprehensively optimize the naturalness of order book data performance.

Start your Market Making on Bonk with CiaoTool now:

{% embed url="https://ciaotool.io/en-US/meteora/market-making" %}

***

## Why Choose CiaoTool Meteora Market Making?

**CiaoTool** provides a professional market-making solution for asset management and long-term growth on the Solana chain, balancing intelligence and security. Whether you need to optimize early-stage liquidity presentation, steadily boost daily on-chain activity, or execute complex multi-address trading strategies, its market management feature guarantees precise and efficient strategy execution through fully automated parameter configurations.

Custom-built for the Meteora trading environment, it transforms complex market-making logic into a one-click, intelligent workflow. Combined with a pure front-end, local private-key signing mechanism for security, it exponentially saves team operational time and eliminates tedious manual operations, while constructing a secure, compliant, and highly cost-effective liquidity management defense line for Web3 project teams.

***

## **Video Tutorial |** Meteora Market Making

{% hint style="info" %}
The Market Making function pages for all platforms on the Solana chain are identical. You can watch the "Solana Market Management" video tutorial below to learn more about the detailed steps of the market management feature.
{% endhint %}

{% embed url="https://www.youtube.com/watch?v=WEwHuWE34WM" %}

***

## **Step by Step |** Meteora Market Making

{% stepper %}
{% step %}
### Connect Wallet

Click the button in the top right corner to connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image (757).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select Value Token and MM Token

You can choose to input the token address, or select a token currently owned by your wallet to perform the buy operation.

* **Value Token:** The token address used to pay the pair's price when executing trading operations.
* **MM Token:** The token address used to achieve the market management strategy goals when executing trading operations.

<figure><img src="../../../.gitbook/assets/image (794).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select Market-Making Strategy

Based on different market-making strategy requirements, select the appropriate bot type and switch to the corresponding strategy bot page.

* **Pull Up:** The operating wallet continuously performs buy operations to steadily build positions and drive up the trading pair's price.
* **Drop:** The operating wallet continuously performs sell operations to steadily liquidate positions and drive down the trading pair's price.
* **Trading Bot:** The operating wallet continuously performs both buy and sell operations to keep the order book constantly flashing.

<figure><img src="../../../.gitbook/assets/image (781).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### MM Bot Setting

{% hint style="danger" %}
Closing / refreshing the page will **immediately stop** the bot strategy. Please ensure that the page remains open and running continuously in the background while the strategy is being executed. To ensure necessary strategy execution, **this feature is not recommended for use on mobile devices.**
{% endhint %}

Click the market-making strategies below to display the full bot setup tutorial.

{% tabs %}
{% tab title="Pull Up" %}
#### Single Transaction Volume

The buy volume for each transaction, anchored to the settings of the **"Value Token".**

If the left and right range limits are identical, it will be a fixed amount; if the range amounts differ, each transaction will use a randomized amount within that specified range.

#### Condition Parameters

Three conditional parameters are provided: **Target Price, Total Maximum Transaction Amount, and Duration**. If left blank, transactions will proceed continuously. If any parameter is filled, the task will automatically stop once that condition is met.

* **Target Price:** When the trading pair price reaches the set **"USDT"** value, the strategy execution stops immediately.
* **Total Maximum Transaction Amount:** Anchored to the settings of the **"Value Token",** when the cumulative total reaches the set value, the strategy execution stops immediately.
* **Duration:** Measured in minutes, when the duration reaches the set value, the strategy execution stops immediately.

<figure><img src="../../../.gitbook/assets/image (782).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Drop" %}
#### Single Transaction Volume

The buy volume for each transaction, anchored to the settings of the **"MM Token".**

If the left and right range limits are identical, it will be a fixed amount; if the range amounts differ, each transaction will use a randomized amount within that specified range.

#### Condition Parameters

Three conditional parameters are provided: **Target Price, Total Maximum Transaction Amount, and Duration**. If left blank, transactions will proceed continuously. If any parameter is filled, the task will automatically stop once that condition is met.

* **Target Price:** When the trading pair price reaches the set **"USDT"** value, the strategy execution stops immediately.
* **Total Maximum Transaction Amount:** Anchored to the settings of the **"MM Token",** when the cumulative total reaches the set value, the strategy execution stops immediately.
* **Duration:** Measured in minutes, when the duration reaches the set value, the strategy execution stops immediately.

<figure><img src="../../../.gitbook/assets/image (783).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Traffic Bot" %}
#### Single Transaction Volume

The buy volume for each transaction, anchored to the settings of the **"Value Token".**

If the left and right range limits are identical, it will be a fixed amount; if the range amounts differ, each transaction will use a randomized amount within that specified range.

#### Condition Parameters

Three conditional parameters are provided: **Total Maximum Transaction Amount, and Duration**. If left blank, transactions will proceed continuously. If any parameter is filled, the task will automatically stop once that condition is met.

* **Total Maximum Transaction Amount:** Anchored to the settings of the **"Value Token",** when the cumulative total reaches the set value, the strategy execution stops immediately.
* **Duration:** Measured in minutes, when the duration reaches the set value, the strategy execution stops immediately.

<figure><img src="../../../.gitbook/assets/image (784).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Input Trading Wallet Private Key

{% hint style="danger" %}
<mark style="color:$danger;">**Security Tips**</mark>

Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

{% hint style="info" %}
<mark style="color:$primary;">**Trading Wallet Setting**</mark>

There are no quantity limits on importing wallets for **Meteora Market Making**. Transaction fees are paid independently by each wallet.
{% endhint %}

Supports two methods for importing sending private key: **"Manual Input"** and **"Upload File"**. Select an option to view the detailed tutorial.

{% tabs %}
{% tab title="Manual Input" %}
1. Click the **"Manual Input"** button to open the input field.

<figure><img src="../../../.gitbook/assets/image (785).png" alt=""><figcaption></figcaption></figure>

2. Enter / bulk paste private keys, one private key per line. Press Enter to start a new line.

<figure><img src="../../../.gitbook/assets/image (787).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (788).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Click the **"Upload File"** button to open the file upload window.

<figure><img src="../../../.gitbook/assets/image (786).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (790).png" alt=""><figcaption></figcaption></figure>

2. Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.   \
   Click to download and view the template:

{% file src="../../../.gitbook/assets/Solana_privateKey_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (791).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (789).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
#### **Confirm** <a href="#confirm" id="confirm"></a>

After verifying all details, click the **"Activate"** button below and wait for the transaction process to complete.

<figure><img src="../../../.gitbook/assets/image (792).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Common Failure Cases

* Over-pumping, leading to concentrated selling pressure that triggers a sharp crash.
* Insufficient liquidity, causing severe price volatility.
* Over-concentration of token holdings, leaving the market vulnerable to single-point dumping.
* Out-of-control pacing, where frequent operations lead to a decline in market trust.
* Ignoring external market conditions, resulting in failed counter-trend operations.

***

## **FAQs**

<details>

<summary><strong>What is Meteora Market Making?</strong></summary>

This feature is used to execute automated trading and market-making strategies within Meteora platfotm. Through multi-address buy and sell operations, it boosts trading activity, ensuring the project maintains continuous trading performance and market visibility. By utilizing multi-address and randomized interval mechanisms, it aligns trading behaviors closely with authentic market participation, comprehensively enhancing the naturalness of overall data performance.

</details>

<details>

<summary><strong>Is the operation secure?</strong></summary>

CiaoTool uses a fully client-side signing mechanism. Your private key is never uploaded or stored on any server, and all transactions are signed locally in your browser. This ensures, at a technical level, that the platform has no access to your private key.

</details>

***

**Need help? Join our community for real-time support:**

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
