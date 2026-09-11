---
description: >-
  A token launch and bundle buy tool for Pump.fun. Create a token and executes
  batch purchases within the same block, helping secure early positions and
  optimize token distribution.
---

# PumpFun - Bundler Tutorial

{% hint style="info" %}
**CiaoTool PumpFun Bundler** now fully supports all quote tokens, including official **SOL and USDC**. Please switch to the specific token page first to perform market management operations, meeting your rapid market-making service needs across various scenarios.
{% endhint %}

## Overview

CiaoTool PumpFun Bundler is a token launch and multi-wallet purchasing tool. It creates a Pump.fun token while executing initial purchases from multiple wallets using predefined amounts.

The token creation and buy transactions are arranged in a specified order and submitted as a Bundle. When successfully executed, the token is created first, followed by consecutive wallet purchases within the same block, reducing the risk of other transactions being inserted between creation and buying.

Start your Bundler on PumpFun with CiaoTool now:

{% embed url="https://ciaotool.io/en-US/pump/create-and-buy" %}

***

## Advatage

* **Create and Buy in One Flow:** Configure token information and wallet purchase amounts at once
* **Ordered Execution:** Bundle and submit creation and buy transactions in a predefined order
* **Multi-Wallet Configuration:** Set participating wallets and purchase amounts individually
* **Automated Execution:** Handles information upload, transaction creation, wallet signing, and Bundle submission
* **Verifiable Results:** View the execution status and transaction record of each transaction

***

## Video Tutorial

{% embed url="https://www.youtube.com/watch?t=12s&v=j381k3jjEyU" %}

***

## Technology Workflow

#### Traditional Token Launch

Token creation and wallet purchase transactions are broadcast separately and processed independently on-chain.

Their execution order and inclusion in the same block are not guaranteed. If other transactions execute first, the pool price may change, increasing the purchase cost and reducing the number of tokens received by later wallets.

<figure><img src="../../../.gitbook/assets/image (1).avif" alt=""><figcaption></figcaption></figure>

#### Bundled Token Launch

The token creation transaction and buy transactions from up to **8 wallets** are arranged in a predefined order and submitted within the same Bundle.

They execute consecutively in the same block, reducing the risk of other transactions being inserted between them while improving execution consistency and on-chain priority.

<figure><img src="../../../.gitbook/assets/image (1152).png" alt=""><figcaption></figcaption></figure>

***

## Step by Step

{% stepper %}
{% step %}
### Connect Wallet

Click the button in the top right corner, and connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Enter Token Info

<figure><img src="../../../.gitbook/assets/image (1153).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Clone:** Click the **"Clone"** button to copy information from another token.
{% endhint %}

* **Token Name:** The full name of the token as you wish it to be displayed in wallets or block explorers (e.g., MyFirstToken).
* **Token Symbol:** The abbreviation of the token, typically 3 to 6 uppercase letters (e.g., MYT).
* **LOGO：**&#x55;pload the logo image for your project or token. A recommended dimension is 1000\*1000 pixels.
* **Description:** A brief introduction to the token's utility, story, or Memecoin background (Optional).
{% endstep %}

{% step %}
### Add Links <mark style="color:$info;">(Ops)</mark>

Although optional, adding your **website, X / Twitter, and Telegram** is recommended to help improve project credibility.

<figure><img src="../../../.gitbook/assets/image (1154).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Mint Address <mark style="color:$info;">(Ops)</mark>

Generate a custom token Mint address to make your token easier to recognize.

Customize your personalized token address; setting up a token address incurs **an additional fee of 0.1 SOL**.

{% tabs %}
{% tab title="Vanity Address" %}
Set the characters you want at the beginning or end of the address, such as starting with `soL` or ending with `pump`. The tool will continue generating random keypairs until a matching address is found.

<figure><img src="../../../.gitbook/assets/image (1146).png" alt=""><figcaption></figcaption></figure>

See the related guide for detailed instructions

{% content-ref url="../wallet-tools/vanity-address.md" %}
[vanity-address.md](../wallet-tools/vanity-address.md)
{% endcontent-ref %}
{% endtab %}

{% tab title="Custom Private Key" %}
* Generate the desired wallet address in advance; it may also be a vanity address
* Import the corresponding private key; the address must be new, unused, and must not have paid SOL rent
* The system will use this address to create the token, ensuring the Mint address matches your selection
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Launch Settings

#### **Quote Token**

Pump.fun currently supports SOL and USDC as quote tokens. Click to switch between them.

#### Mayhem Mode

For 24 hours after launch, bots execute randomized buys and sells to increase trading activity and price volatility. Price increases are not guaranteed. An additional 1 billion tokens will be issued for bot activity, and any remaining tokens will be burned when the mode ends.

View the [**PumpFun Mayhem Mode Rules**](https://pump.fun/docs/mayhem-mode-disclaimer).

#### Cashback Reward

When enabled, creator fees that would normally go to the token creator are returned to traders and accumulated according to their trading volume. Simply holding the token does not generate cashback.

View the [**PumpFun Creator Fee Rates**](https://pump.fun/docs/fees).
{% endstep %}

{% step %}
### Dev Wallet Purchase

Uses the currently connected wallet to purchase the token. If left blank, the amount defaults to `0`. The wallet may be labeled as the **Dev Wallet** on on-chain analytics platforms such as GMGN and DEXScreener.
{% endstep %}

{% step %}
### **Import Private Keys**

{% hint style="danger" %}
Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

Up to **8 wallets** to bundled buy. Add them **Manually Input** or **Upload File**. Click to view the guide.

{% tabs %}
{% tab title="Manual Input" %}
1. Click the "Bulk Input" button to open the input field.

<figure><img src="../../../.gitbook/assets/image (1155).png" alt=""><figcaption></figcaption></figure>

2. Enter / paste wallet private keys, one per line. Optionally add the transfer amount after each wallet.

```
privateKey, 300
```

<figure><img src="../../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

3. Click "Import" to import all entered wallets into the operation panel.

<figure><img src="../../../.gitbook/assets/image (1123).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Download the CiaoTool template and fill in the transfer details.

<figure><img src="../../../.gitbook/assets/image (1156).png" alt=""><figcaption></figcaption></figure>

2. Click ![](<../../../.gitbook/assets/image (7).png>)"Import File" button to open the input field.
3. Click "Import" to import all entered wallets into the operation panel.

<figure><img src="../../../.gitbook/assets/image (1124).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Enter  Amount

Choose from 2 amount options: **Individual, or Fixed**. Dev and bundled wallets purchases are limited to **86 SOL** in total.

1. **Individual**\
   Enter a different amount for each address.
2. **Fixed Amount**\
   Click ![](<../../../.gitbook/assets/image (8).png>) above “Amount”, and select “Fixed Amount” to apply the same amount to all addresses.
{% endstep %}

{% step %}
### Auto Sell

During the bonding curve phase, all bundled wallets automatically sell when the token reaches the target gain from the initial purchase price.
{% endstep %}

{% step %}
### Jito Tips

{% hint style="danger" %}
This feature uses Jito Bundles and may fail due to network, RPC, or Block Engine conditions. If the Bundle does not land, the token will not be created and no on-chain fees will be charged. Try another RPC or Block Engine, increase the Jito tip, or retry later.
{% endhint %}

Use a Jito tip to bundle token creation and multi-wallet transactions, reducing sniping risk and improving landing priority at an additional cost.

<figure><img src="../../../.gitbook/assets/image (1158).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Confirm

After confirming the details, click **“Create and Buy”** to track the creation progress and result in real time.

<figure><img src="../../../.gitbook/assets/image (1148).png" alt=""><figcaption></figcaption></figure>
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

<summary><strong>What is the PumpFun "Bundler" (Create &#x26; Buy) feature?</strong></summary>

It is a high-speed token deployment engine custom-built for the Pump.fun platform. By atomically bundling "token creation" and "multi-wallet buys" into the exact same block for simultaneous execution, it guarantees you secure early supply at the absolute initial floor price while instantly establishing a decentralized holder footprint at launch.

</details>

<details>

<summary><strong>Why must "Creation" and "Buying" be bundled together?</strong></summary>

Pump.fun utilizes a bonding curve pricing mechanism where token prices surge sharply alongside early buy order inflows. If you deploy a token first and execute manual buys later, the resulting latency window leaves you vulnerable to malicious on-chain sniper bots that front-run your launch, forcing you to buy back your own token at inflated prices. Bundling completely eradicates this timing gap, neutralizing snipers to lock in your initial capital efficiency.

</details>

<details>

<summary><strong>Can this feature be used to optimize the early holder structure?</strong></summary>

Absolutely. Since the feature supports batching multiple independent wallet addresses for simultaneous buy execution, these allocations are completed at the exact microsecond of token deployment. This allows your token to present a healthy, well-distributed holder ledger right at birth, preventing red flags caused by capital over-concentration in a single address.

</details>

<details>

<summary><strong>Why does the "Create &#x26; Buy" execution frequently fail</strong></summary>

* Why it fails: This feature relies on Jito's bundling protocol. High network congestion or node latency can miss strict packaging windows, causing transactions to be dropped.
* Is my capital safe? Yes, 100% safe. The execution is fully atomic. If it fails, the token will not launch, and all assets/fees instantly revert with zero attrition.
* How to fix: Increase your Jito tip (0.001 SOL recommended), switch to a premium RPC node/block engine, or retry during off-peak hours.

</details>

<details>

<summary><strong>Is the operation secure?</strong></summary>

CiaoTool uses a fully client-side signing mechanism. Your private key is never uploaded or stored on any server, and all transactions are signed locally in your browser. This ensures, at a technical level, that the platform has no access to your private key.

</details>

***

## Service Support

Need help? Join our community for real-time support:

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
