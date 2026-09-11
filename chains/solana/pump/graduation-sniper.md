---
description: >-
  A launch and bundle buy tool for Pump.fun. Supports token creation,
  multi-wallet purchases, and PumpSwap sniping to help secure early positions.
---

# PumpFun - PumpFun Create, Graduate and Snipe Bot Guide

{% hint style="info" %}
**CiaoTool PumpFun Create, Graduate and Snipe Bot** now fully supports all quote tokens, including official **SOL and USDC**.
{% endhint %}

## Overview

**CiaoTool PumpFun Create, Graduate & Buy Bot** is a two-stage automation tool covering token creation, Bonding Curve purchases, and post-migration purchases. It reduces manual operations and waiting between stages.

The process consists of two independent Bundles:

1. **Creation and Bonding Curve Buys:** Token creation and multi-wallet Bonding Curve purchases are bundled in a predefined order and normally execute consecutively within the same block.
2. **Migration and Post-Migration Buy:** Once the token meets the graduation requirements, the PumpSwap migration and designated wallet purchase are submitted as a new Bundle and normally execute in sequence within the same block.

Start your Graduation Sniper on PumpFun with CiaoTool now:

{% embed url="https://ciaotool.io/en/pump/graduation-sniper" %}

***

## Advantage

* **Two-Stage Automation:** Connects token creation, Bonding Curve purchases, migration, and post-migration purchases
* **Ordered Execution:** Submits transactions within each Bundle in a predefined order to reduce execution gaps
* **Multi-Wallet Configuration:** Set participating wallets and purchase amounts for each stage
* **Improved Landing Priority:** Uses Jito tips to compete for higher Bundle landing priority
* **Local Signing:** Transactions are signed locally in the browser, and private keys are not uploaded to the server

***

## Video Tutorial

{% embed url="https://www.youtube.com/watch?v=MtfL8ynNKmc" %}

***

## Technology Workflow

#### Traditional Token Launch

{% columns %}
{% column %}
Token creation, multi-wallet purchases, DEX migration, and post-migration purchases are broadcast separately and confirmed independently. Their execution order and inclusion in consecutive blocks cannot be guaranteed.

If other transactions are inserted during the process, the token price may change, affecting purchase costs and the number of tokens received by later wallets.

During migration, bots may front-run the purchase, reducing the number of tokens received and causing additional losses.
{% endcolumn %}

{% column %}
<figure><img src="../../../.gitbook/assets/image (2).avif" alt=""><figcaption></figcaption></figure>
{% endcolumn %}
{% endcolumns %}

#### Bundled Token Launch

{% columns %}
{% column %}
The complete process is divided into two Bundles:

* **Launch Stage:** Token creation and purchases from six wallets are bundled and executed consecutively within the same block in a predefined order. These purchases fill the Bonding Curve and trigger the migration process.
* **Migration Stage:** The DEX migration and designated wallet purchase are bundled again and executed in sequence within the same block.

This significantly reduces transaction gaps and the risk of other transactions being inserted during migration, improving execution consistency, landing priority, and profit potential.
{% endcolumn %}

{% column %}
<figure><img src="../../../.gitbook/assets/image (1159).png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}
{% endcolumns %}

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
### Bonding Curve Private Keys

{% hint style="danger" %}
Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

Up to **6 wallets** to bundled buy. Add them **Manually Input** or **Upload File**. Click to view the guide.

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

Choose from 2 amount options: **Individual, or Fixed**. Dev and bundled wallet purchases must exceed **86 SOL** in total.

1. **Individual**\
   Enter a different amount for each address.
2. **Fixed Amount**\
   Click ![](<../../../.gitbook/assets/image (8).png>) above “Amount”, and select “Fixed Amount” to apply the same amount to all addresses.
{% endstep %}

{% step %}
### Migration Snipe Wallet

Enter the private keys of the wallets that will snipe the token when it migrates to PumpSwap, securing early positions while boosting initial activity.

No limit on the token purchase amount on PumpSwap.

<figure><img src="../../../.gitbook/assets/image (1160).png" alt=""><figcaption></figcaption></figure>
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

## Service Support

Need help? Join our community for real-time support:

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
