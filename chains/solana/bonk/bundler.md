---
description: >-
  A token launch and bundle buy tool for Bonk.fun. Create a token and executes
  batch purchases within the same block, helping secure early positions and
  optimize token distribution.
---

# Bonk - Bundler Tutorial

{% hint style="info" %}
**CiaoTool Bonk Bundler** now fully supports all quote tokens, including official **SOL and USD1**. Please switch to the specific token page first to perform market management operations, meeting your rapid market-making service needs across various scenarios.
{% endhint %}

## What is CiaoTool Bonk Bundler?

<figure><img src="../../../.gitbook/assets/image (891).png" alt="CiaoTool Solana Toolkit Page about BonkFun Bundler Feature"><figcaption></figcaption></figure>

CiaoTool Bonk Bundler is an elite token issuance and automated position-building engine custom-built for Solana's **Bonk.fun platform**. It allows developers to deploy a brand-new token while simultaneously orchestrating multiple wallet addresses to execute the foundational batch buy within the exact same block.

Unlike the traditional "deploy first, manual buy later" method, Bundler uses atomic bundling to merge token creation and multi-wallet buys into a single, indivisible on-chain package. This eliminates any time gap, ensuring instant execution alongside the launch.

Start your Bundler on Bonk with CiaoTool now:

{% embed url="https://ciaotool.io/en-US/bonk/create-and-buy" %}

***

## Why Choose CiaoTool Bonk Bundler?

CiaoTool delivers an elite, ultra-secure, and low-cost token launch solution for the Bonk.fun platform. For teams requiring absolute control over initial token supply and foolproof protection against sniper interference, this tool establishes an ironclad execution matrix:

* **Absolute Sniper Eradication:** \
  Utilizing underlying bundle packaging technology, token deployment and multi-wallet buy orders are atomic-aggregated into the exact same block, completely disabling on-chain snipers from front-running and inflating early prices.
* **Guaranteed Floor Price Entry:** \
  Ensures your multi-address buy orders execute as the absolute first transactions of the token's genesis block, locking in early positions at the pristine initial floor price to maximize capital efficiency.
* **Optimized Holder Distribution:** \
  Supports customizable, synchronous buys across multiple independent wallets, executing an organic, decentralized holder structure at the exact microsecond of launch to beautifully optimize early on-chain metrics.
* **1-Click Automated Autopilot:** \
  Fully automates metadata uploads, parameter configurations, and multi-wallet asset distribution in one single click, totally liberating your team from tedious manual account-switching and frantic panic-buying.

***

## Video Tutorial | Bonk Bundler

{% embed url="https://www.youtube.com/watch?t=8s&v=8J9Xx3VCn0o" %}

***

## **Step by Step |** Bonk Bundler

{% stepper %}
{% step %}
### Connect Wallet

Click the button in the top right corner to connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image (757).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Enter Token Information

<figure><img src="../../../.gitbook/assets/image (882).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Clone:** Click the **"Clone"** button to copy information from another token.
{% endhint %}

* **Token Name:** The full name of the token as you wish it to be displayed in wallets or block explorers (e.g., MyFirstToken).
* **Token Symbol:** The abbreviation of the token, typically 3 to 6 uppercase letters (e.g., MYT).
* **LOGO：**&#x55;pload the logo image for your project or token. A recommended dimension is 1000\*1000 pixels.
* **Description:** A brief introduction to the token's utility, story, or Memecoin background (Optional).
* **Social Links:** Although optional, it is highly recommended to fill this in, including Official Website, X / Twitter, and Telegram.
{% endstep %}

{% step %}
### Dev Wallet Buy

Uses the currently connected wallet to execute the buy order. Defaults to 0 if left blank.

<figure><img src="../../../.gitbook/assets/image (883).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Input Buyer Wallet Private Key

{% hint style="danger" %}
<mark style="color:$danger;">**Security Tips**</mark>

Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

Supports two methods for importing sending private key: **"Manual Input"** and **"Upload File"**. Support a maximum of **8 addresses** for bundled buying. Select an option to view the detailed tutorial.

{% tabs %}
{% tab title="Manual Input" %}
1. Click the **"Manual Input"** button to open the input field.

<figure><img src="../../../.gitbook/assets/image (892).png" alt=""><figcaption></figcaption></figure>

2. Enter / bulk paste private keys, one private key per line. Press Enter to start a new line.

<figure><img src="../../../.gitbook/assets/image (787).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (887).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Click the **"Upload File"** button to open the file upload window.

<figure><img src="../../../.gitbook/assets/image (893).png" alt=""><figcaption></figcaption></figure>

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
### Custom Service

#### Custom Contract Address

<figure><img src="../../../.gitbook/assets/image (890).png" alt=""><figcaption></figcaption></figure>

Customize your personalized token address; setting up a token address incurs **an additional fee of 0.01 SOL**.

1. **Custom Token Address**
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

After verifying all details, click the **"Bonk Launch and Buy"** button below and wait for the transaction process to complete.

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

<summary><strong>What is theBonk "Bundler" (Create &#x26; Buy) feature?</strong></summary>

It is a high-speed token deployment engine custom-built for the Bonk.fun platform. By atomically bundling "token creation" and "multi-wallet buys" into the exact same block for simultaneous execution, it guarantees you secure early supply at the absolute initial floor price while instantly establishing a decentralized holder footprint at launch.

</details>

<details>

<summary><strong>Why must "Creation" and "Buying" be bundled together?</strong></summary>

Bonk.fun utilizes a bonding curve pricing mechanism where token prices surge sharply alongside early buy order inflows. If you deploy a token first and execute manual buys later, the resulting latency window leaves you vulnerable to malicious on-chain sniper bots that front-run your launch, forcing you to buy back your own token at inflated prices. Bundling completely eradicates this timing gap, neutralizing snipers to lock in your initial capital efficiency.

</details>

<details>

<summary><strong>Can this feature be used to optimize the early holder structure?</strong></summary>

Absolutely. Since the feature supports batching multiple independent wallet addresses for simultaneous buy execution, these allocations are completed at the exact microsecond of token deployment. This allows your token to present a healthy, well-distributed holder ledger right at birth, preventing red flags caused by capital over-concentration in a single address.

</details>

<details>

<summary><strong>Why does the "Create &#x26; Buy" execution frequently fail?</strong></summary>

* Why it fails: This feature relies on Jito's bundling protocol. High network congestion or node latency can miss strict packaging windows, causing transactions to be dropped.
* Is my capital safe? Yes, 100% safe. The execution is fully atomic. If it fails, the token will not launch, and all assets/fees instantly revert with zero attrition.
* How to fix: Increase your Jito tip (0.001 SOL recommended), switch to a premium RPC node/block engine, or retry during off-peak hours.

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
