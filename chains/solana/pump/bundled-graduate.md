---
description: >-
  Bundled Graduate is a sniping tool for Pump.fun tokens. Combines multi-wallet
  buys and PumpSwap launch sniping to help secure positions during liquidity
  migration.
---

# PumpFun - Bundled Graduate Tutorial

{% hint style="info" %}
**CiaoTool PumpFun Bundled Graduate** now fully supports all quote tokens, including official **SOL and USDC**. Please switch to the specific token page first to perform market management operations, meeting your rapid market-making service needs across various scenarios.
{% endhint %}

## What is CiaoTool PumpFun Bundled Graduate?

<figure><img src="../../../.gitbook/assets/屏幕截图 2026-06-12 155727.png" alt="CiaoTool Solana Toolkit Page about PumpFun Bundled Graduate Feature"><figcaption></figcaption></figure>

**PumpFun Bundled Graduate (Bundled & Migrated Buy)** is an elite liquidity orchestration protocol designed specifically for tokens already active on Pump.fun but yet to migrate their liquidity.

Unlike standard meme deployment utilities, this feature sharpens its focus entirely on the precise cross-market transition from the internal bonding curve to the external DEX. It empowers teams at any viable stage of a token’s lifecycle to forcibly bind two mission-critical operations via Jito's bundling matrix, executing them with absolute atomicity inside the exact same block:

1. **Multi-Address Curve Exhaustion:** Automatically calculates remaining curve quota and deploys multiple wallets to snap it up, instantly hitting the 85 SOL threshold to trigger automated migration.
2. **Synchronized DEX Snipe:** Executes your sniper buy orders at the tail end of the exact same migration block, capturing the absolute opening DEX supply before external bots can parse it.

Start your Bundled Graduate on PumpFun with CiaoTool now:

{% embed url="https://ciaotool.io/en-US/pump/bundled-graduate" %}

***

## Why Choose CiaoTool PumpFun Bundled Graduate

**An industry-first launch optimization tool on Solana.** It breaks the limitation of traditional tools by allowing teams to flexibly intervene at any stage of an active bonding curve, bundling curve finality and external listing sniping into a single on-chain block.

*   **Universal Compatibility**

    Not restricted to tokens deployed via CiaoTool. As long as the token is still on the bonding curve, you can deploy this sniping strategy at any moment.
* **Single-Block Atomic Linkage**\
  Bridges the gap between curve finality and external opening. Combined in one block, it bars external bots from injecting orders, eliminating front-running.
* **Decoupled Campaign Freedom**\
  Fully independent of token creation. Focus on early community warming and holder accumulation first, then execute graduation-and-snipe whenever ready.
* **Client-Side Security**\
  Absolute local isolation. Private keys and signatures execute solely within your browser—zero server uploads, guaranteeing total capital safety.

***

## **Step by Step |** PumpFun Bundled Graduate

{% stepper %}
{% step %}
### **Connect Wallet**

Click the button in the top right corner to connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image (757).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Input Bonding Curve Buyer Wallet Private Key

{% hint style="danger" %}
<mark style="color:$danger;">**Security Tips**</mark>

Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

Supports a maximum of **12 bundled wallets** for purchasing on the Pump.fun bonding curve. The combined buy volume of  bundled wallets must exceed **85 SOL** to systematically trigger the graduation/migration protocol.

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
### Set Jito Tip

Configure Jito MEV tips to accelerate transaction packaging and maximize sequence priority.

{% hint style="danger" %}
This feature relies entirely on Jito’s bundling capabilities. Due to the complex interplay of network volatility, Jito nodes, RPC providers, and block engines, bundled transactions may experience a higher failure rate.

If the execution fails, the token will NOT be launched and zero fees will be incurred (atomic reversion). To resolve this, please try switching your RPC node or block engine, increasing the Jito tip (0.001 SOL recommended), or re-executing during periods of lower network congestion.
{% endhint %}
{% endstep %}

{% step %}
### Confirm

After verifying all details, click the **"Pump Bundled Buy and Snipe"** button below and wait for the transaction process to complete.
{% endstep %}
{% endstepper %}

## Common Failure Cases

* **Insufficent Jito Tip**\
  If the execution fails because your Jito tip is below the market average or gets front-run by other bots, please appropriately increase the Jito tip and retry.
* **Node & Engine Latency**\
  If you miss the strict packaging window due to response latency from RPC nodes or block engines, please switch to a more stable alternative.
* **Insufficient Wallet Buffer**\
  If the primary wallet lacks the balance to cover hidden overheads like token creation fees and rent exemptions, please ensure you leave a buffer of at least 0.05 SOL.
* **Network Congestion & Packet Loss**\
  During periods of extreme Solana network congestion causing random underlying packet loss, please bypass peak trading hours and try again later.

***

## **FAQs**

<details>

<summary><strong>What is the core difference between "Bundled Graduate" and "Graduation Sniper"?</strong></summary>

"Graduation Sniper" includes token creation. "Bundled Graduate" does not—it is built for tokens already trading on the curve, allowing you to intervene and force graduation at any time.

</details>

<details>

<summary><strong>If my token wasn't deployed via CiaoTool, can I still use this feature?</strong></summary>

Yes. As long as the token is still on the Pump.fun bonding curve, you can use this feature regardless of where it was originally deployed.

</details>

<details>

<summary><strong>How is the capital for curve-filling calculated and allocated?</strong></summary>

The system reads the curve's remaining progress in real-time. Just ensure your imported wallets have enough SOL to cover the remaining curve supply, slippage, and Jito tips.

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
