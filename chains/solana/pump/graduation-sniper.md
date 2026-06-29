---
description: >-
  A launch and bundle buy tool for Pump.fun. Supports token creation,
  multi-wallet purchases, and PumpSwap sniping to help secure early positions.
---

# PumpFun - Graduation Sniper Tutorial

{% hint style="info" %}
**CiaoTool PumpFun Graduation Sniper** now fully supports all quote tokens, including official **SOL and USDC**. Please switch to the specific token page first to perform market management operations, meeting your rapid market-making service needs across various scenarios.
{% endhint %}

## What is CiaoTool PumpFun Graduation Sniper?

<figure><img src="../../../.gitbook/assets/image (898).png" alt="CiaoTool Solana Toolkit Page about PumpFun Graduation Sniper Feature"><figcaption></figcaption></figure>

The CiaoTool PumpFun Graduation Sniper is an elite launch and position-building engine that deeply integrates token deployment with multi-stage automated buying. Breaking the limitations of traditional siloed tools, it compresses the entire execution span—from internal market genesis to external market migration—into a single, indivisible blockchain block. This tool builds an ironclad, automated defense line that guarantees front-running protection and optimal holder distribution at the absolute birth of a token.

Core Execution Stages

1.  **Bonding Curve Bundle**

    Utilizing Jito's bundling protocols at the infrastructure layer, the system seamlessly packages the token deployment command and the primary batch of independent buying wallets into the exact same block. This ensures that the moment the token is born, the team’s pre-configured wallets execute instantly to fill the bonding curve and trigger migration, locking in the absolute initial floor price.
2. **PumpSwap Migration Snipe**\
   The exact microsecond the platform migrates liquidity to PumpSwap, the pre-configured sniper wallet transactions are already tightly locked at the tail end of that very same block. This means that while the external liquidity pool is freshly deployed—and before public sniper bots can even parse the chain data—the team's capital has already snipped the initial external supply, flawlessly executing a full-lifecycle token allocation loop.

Start your Graduation Sniper on PumpFun with CiaoTool now:

{% embed url="https://ciaotool.io/en-US/pump/graduation-sniper" %}

***

## Why Choose CiaoTool PumpFun Graduation Sniper？

An industry-first, pinnacle launch engine on Solana. Graduation Sniper compresses the entire lifecycle—from token creation and filling the bonding curve to protocol migration and the first external DEX snipe—into a single on-chain block, erecting an unbreachable fortress against snipers.

*   **Single-Block Aggregation**

    Unified execution of deployment, migration, and sniping within one block. No external bot can insert transactions—front-running is completely neutralized.
* **Zero Bonding Time**
* Instantly max out the curve to bypass malicious swing bots, locking in the absolute floor price internally and the pristine opening price externally.
* **Automated Matrix Orchestration**\
  Automated asset routing, quota calculation, and cross-market sniping with zero broken strategies or latency gaps.
* **Client-Side Security**\
  Strict local isolation. All private keys and signatures execute solely within your browser—zero server uploads, guaranteeing source-level safety.

***

## Video Tutorial | PumpFun Graduation Sniper

{% embed url="https://www.youtube.com/watch?v=MtfL8ynNKmc" %}

***

## **Step by Step |** PumpFun Graduation Sniper

{% stepper %}
{% step %}
### **Connect Wallet**

Click the button in the top right corner to connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image (757).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Enter Token Information

{% hint style="info" %}
**Clone:** Click the **"Clone"** button to copy information from another token.
{% endhint %}

* **Token Name:** The full name of the token as you wish it to be displayed in wallets or block explorers (e.g., MyFirstToken).
* **Token Symbol:** The abbreviation of the token, typically 3 to 6 uppercase letters (e.g., MYT).
* **LOGO：**&#x55;pload the logo image for your project or token. A recommended dimension is 1000\*1000 pixels.
* **Description:** A brief introduction to the token's utility, story, or Memecoin background (Optional).

<figure><img src="../../../.gitbook/assets/image (882).png" alt=""><figcaption></figcaption></figure>

* **Social Links:** Although optional, it is highly recommended to fill this in, including Official Website, X / Twitter, and Telegram.
{% endstep %}

{% step %}
### Dev Wallet Buy

Uses the currently connected wallet to execute the buy order. Defaults to 0 if left blank.

<figure><img src="../../../.gitbook/assets/image (883).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Input Bonding Curve Buyer Wallet Private Key

{% hint style="danger" %}
<mark style="color:$danger;">**Security Tips**</mark>

Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

Supports a maximum of **9 bundled wallets** for purchasing on the Pump.fun bonding curve. The combined buy volume of the Dev wallet and bundled wallets must exceed **85 SOL** to systematically trigger the graduation/migration protocol.

Supports two methods for importing sending private key: **"Manual Input"** and **"Upload File"**. Select an option to view the detailed tutorial.

{% tabs %}
{% tab title="Manual Input" %}
1. Click the **"Manual Input"** button to open the input field.

<figure><img src="../../../.gitbook/assets/image (896).png" alt=""><figcaption></figcaption></figure>

2. Enter / bulk paste private keys, one private key per line. Press Enter to start a new line.

<figure><img src="../../../.gitbook/assets/image (787).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (887).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Click the **"Upload File"** button to open the file upload window.

<figure><img src="../../../.gitbook/assets/image (897).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (790).png" alt=""><figcaption></figcaption></figure>

2. Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.   \
   Click to download and view the template:

{% file src="../../../.gitbook/assets/Solana_privateKey_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (791).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (886).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Enter Buy Amount

Supports three buy amount types: **"Individual Input", "Amount",** **"Percentage"** and **"All"**.

1.  **Individual Input**\
    In the input fields, enter the buy amount for each address one by one.

    <figure><img src="../../../.gitbook/assets/image (846).png" alt=""><figcaption></figcaption></figure>
2. **Amount:**\
   Click the **"Batch Input"** button above the buy amount, select the "Amount" option, and enter the amount. All addresses will then have a uniform buy amount applied.
3. **Percentage:**\
   Click the **"Batch Input"** button above the buy amount, select the "Percentage" option, and enter the percentage parameter. All addresses will then execute the buy operation based on the specified percentage of their respective balances.
4. **All Amount**\
   All wallets will buy 100% of their token holdings into the designated token.
{% endstep %}

{% step %}
### Input DEX Buyer Wallet Private Key

* **Wallet Addresses for Migration Snipe:** Configure the sniper wallet addresses to execute buy orders the exact moment the token migrates to Raydium/PumpSwap.
* **Snipe Amount Setting:** Specify the exact purchase amount (in SOL) for each sniper walle

<figure><img src="../../../.gitbook/assets/image (16).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Custom Service

#### Custom Contract Address

<figure><img src="../../../.gitbook/assets/image (890).png" alt=""><figcaption></figcaption></figure>

Customize your personalized token address; setting up a token address incurs **an additional fee of 0.01 SOL**.

1. **Ending with "pump"**
   * The token address will end with "pump".
2. **Custom Token Address**
   * Generate your desired wallet address in advance, which can be a vanity address.
   * Paste and import the private key you generated in advance **(the address must be completely new and must not have paid any SOL rent);**
   * The system will use this address to deploy your token, ensuring the contract address matches your expectations.

#### Pre-generate Token Contract

Pre-generate your token contract address while preserving all currently edited token metadata securely on-chain. This feature is ideal for scenarios requiring pre-launch marketing, community warming, or early third-party integrations before trading officially opens.
{% endstep %}

{% step %}
### Set Jito Tip

Configure Jito MEV tips to accelerate transaction packaging and maximize sequence priority.

{% hint style="danger" %}
This feature relies entirely on Jito’s bundling capabilities. Due to the complex interplay of network volatility, Jito nodes, RPC providers, and block engines, bundled transactions may experience a higher failure rate.

If the execution fails, the token will NOT be launched and zero fees will be incurred (atomic reversion). To resolve this, please try switching your RPC node or block engine, increasing the Jito tip (0.001 SOL recommended), or re-executing during periods of lower network congestion.
{% endhint %}
{% endstep %}

{% step %}
### Confirm

After verifying all details, click the **"Pump Launch and Buy Sniper"** button below and wait for the transaction process to complete.

<figure><img src="../../../.gitbook/assets/image (760).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

## Common Failure Cases

* **Insufficent Jito Tip**\
  If the execution fails because your Jito tip is below the market average or gets front-run by other bots, please appropriately increase the Jito tip and retry.
* **Node & Engine Latency**\
  If you miss the strict packaging window due to response latency from RPC nodes or block engines, please switch to a more stable alternative.
* **Insufficient Wallet Buffer**\
  If the primary wallet lacks the balance to cover hidden overheads like token creation fees and rent exemptions, please ensure you leave a buffer of at least 0.05 SOL.
* **Metadata Upload Timeout**\
  If the token avatar file is too large and causes an upload timeout, please compress the image to under 1MB before re-initiating the operation.
* **Network Congestion & Packet Loss**\
  During periods of extreme Solana network congestion causing random underlying packet loss, please bypass peak trading hours and try again later.

***

## **FAQs**

<details>

<summary><strong>What is the PumpFun "Graduation Sniper" feature?</strong></summary>

It is an advanced full-lifecycle automation engine custom-built for the Pump.fun ecosystem. In one seamless operation, it encapsulates token deployment, multi-wallet bonding curve buys, and the initial external market snipe into a single unified matrix, guaranteeing a flawless, uninterrupted transition from token genesis to DEX listing.

</details>

<details>

<summary><strong>Why aggregate bonding curve deployment and DEX sniping into a single block?</strong></summary>

The exact millisecond a token graduates from the bonding curve and migrates to the external DEX, it is instantly exposed to a massive influx of aggressive public sniper bots vying to snap up cheap early supply. Compressing the core pipeline into a single-block atomic bundle completely eliminates any execution gap, barring external bots from injecting malicious transactions and ensuring your market-making capital commands absolute priority.

</details>

<details>

<summary><strong>Can this feature be used to optimize the early holder structure?</strong></summary>

Absolutely. By supporting the batch onboarding of multiple independent wallet addresses for simultaneous execution, these buy orders are triggered independently at the exact microsecond of token deployment. This allows your project to present an organic, highly decentralized holder profile on-chain right at launch, effectively bypassing any single-address risk red flags.

</details>

<details>

<summary><strong>Why does the "Graduation Sniper" execution sometimes fail?</strong></summary>

Failures stem from the feature's underlying reliance on Jito’s specialized bundling mechanism. During spikes in network congestion or RPC latency, Jito bundles face tight validation windows and may be dropped by validators, resulting in elevated failure rates.

To significantly scale up your success rate, we highly recommend increasing your Jito tip (0.001 SOL or higher recommended), upgrading to premium RPC nodes/block engines, or executing during lower network congestion periods.

</details>

<details>

<summary><strong>If the launch fails on-chain, will my funds be at risk?</strong></summary>

Completely zero risk. Operating on a strict atomic bundling architecture, the system enforces a zero-friction safety reversion. If the transaction bundle encounters network saturation or latency and fails to secure inclusion, the entire operation safely reverts. Your SOL principal remains untouched in your wallets with absolute safety—free from the risks of partial buys, capital leakage, or slippage attrition. You can recalibrate your parameters and re-initiate instantly.

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
