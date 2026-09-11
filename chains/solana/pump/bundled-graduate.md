---
description: >-
  Bundled Graduate is a sniping tool for Pump.fun tokens. Combines multi-wallet
  buys and PumpSwap launch sniping to help secure positions during liquidity
  migration.
---

# PumpFun - Bundled Buy, Graduate and Snipe Bot Guide

{% hint style="info" %}
**CiaoTool PumpFun Bundled Graduate** now fully supports all quote tokens, including official **SOL and USDC**.&#x20;
{% endhint %}

## Overview

CiaoTool PumpFun Bundled Buy & Migration is an automated tool for tokens that are **already live on Pump.fun but have not yet migrated**. The token does not need to be recreated.

The system calculates the remaining Bonding Curve progress and bundles the following operations in order:

1. **Bundled Bonding Curve Buys:** Multiple wallets purchase the remaining amount required to reach the platform’s migration threshold.
2. **Migration and PumpSwap Buy:** After liquidity is migrated, a designated wallet buys the token on PumpSwap.

When successfully executed, all transactions in the Bundle are completed in the predefined order within the same block. If any critical transaction fails, the entire Bundle is not executed.

Start your Bundled Graduate on PumpFun with CiaoTool now:

{% embed url="https://ciaotool.io/en/pump/bundled-graduate" %}

***

## Advantage

* **Supports Existing Tokens:** Works with compatible tokens still in the Bonding Curve stage
* **Automatic Amount Calculation:** Estimates the amount required to reach the migration threshold using real-time on-chain data
* **Multi-Wallet Execution:** Configure multiple Bonding Curve buying wallets and individual purchase amounts
* **Connected Migration Flow:** Bundles Bonding Curve purchases, liquidity migration, and the PumpSwap purchase in order
* **Impro Finder? Landing Priority:** Uses a Jito tip to improve Bundle landing priority
* **Local Signing:** Transactions are signed locally in the browser, and private keys are not uploaded

***

## Technology Workflow

#### Traditional Token Launch

{% columns %}
{% column %}
Multi-wallet purchases, DEX migration, and post-migration purchases are broadcast separately and confirmed independently. Their execution order and inclusion in adjacent blocks cannot be guaranteed.

If other transactions are inserted during execution, the token price may change, increasing purchase costs and reducing the number of tokens received by later wallets.

During migration, bots may front-run transactions, resulting in fewer tokens received and potential losses.
{% endcolumn %}

{% column %}
<figure><img src="../../../.gitbook/assets/image (1161).png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}
{% endcolumns %}

#### Bundled Token Launch

{% columns %}
{% column %}
The process is executed in two bundled stages:

* **Launch Stage:** Purchases from eight wallets are bundled and executed consecutively within the same block in a predefined order, filling the Bonding Curve and triggering migration.
* **Migration Stage:** The DEX migration and designated wallet purchase are bundled and executed in sequence within the same block.

This reduces transaction gaps and the risk of other transactions being inserted during migration, improving execution consistency, landing priority, and profit potential.
{% endcolumn %}

{% column %}
<figure><img src="../../../.gitbook/assets/image (1162).png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}
{% endcolumns %}

***

## Step by Step

{% stepper %}
{% step %}
### Connect Wallet

Click the button in the top right corner, and connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Bonding Curve Private Keys

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
### Enter Amount

The system checks the current Bonding Curve status in real time and calculates the amount required to complete it. The total purchase amount across bundled wallets must exceed the displayed amount.

Choose from 2 amount options: **Individual, or Fixed**.

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

## Service Support

Need help? Join our community for real-time support:

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
