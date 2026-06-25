---
description: >-
  An asset migration tool for Pump.fun that combines sells and multi-wallet buys
  within the same block. Creates natural trading activity, reducing MEV risk and
  optimizing on-chain asset distribution.
---

# PumpFun - Sell & Bundled Buy Tutorial

{% hint style="info" %}
**CiaoTool PumpFun Sell & Bundled Buy** now fully supports all quote tokens, including official **SOL and USDC**. Please switch to the specific pool function page first to perform bundled operations.
{% endhint %}

## What is CiaoTool PumpFun Sell & Bundled Buy?

<figure><img src="../../../.gitbook/assets/image (869).png" alt="CiaoTool Solana Toolkit Page about Pump.fun Sell and Bundled Buy Feature"><figcaption></figcaption></figure>

**CiaoTool PumpFun Sell & Bundled Buy** is an advanced tool focusing on transaction continuity and on-chain liquidity management. Utilizing underlying smart aggregation technology, it allows you to automatically enable a designated wallet to complete token sell operations on **Pump.fun** within the exact same block, while synchronously triggering the batch buy actions of multiple independent wallets.

Compared to manual trading or direct transfers, this feature simulates organic order book patterns to make position-switching look natural. By aggregating bidirectional buy and sell trades into a single block, it maximizes protection against MEV attacks, eliminates tedious manual account-switching, and securely optimizes token holder distribution.

Key Use Cases:

* Liquidity migration and secure asset restructuring in professional market making.
* Replacing direct transfers with authentic order book buying and selling to make chip transfer trajectories align better with natural market logic.
* Reducing slippage attrition and MEV sandwich risks during bidirectional buy and sell transactions.
* Eliminating the tedious operations of frequently switching wallets, drastically saving team operational time.
* Securely and steadily promoting a healthy distribution of token addresses and on-chain data optimization.Key Use Cases:

Start your Sell & Bundled Buy on PumpFun with CiaoTool now:

{% embed url="https://ciaotool.io/en-US/pump/bundled-sell-buy" %}

***

## Why Choose CiaoTool PumpFun Sell & Bundled Buy?

CiaoTool delivers a secure, low-attrition PumpFun position-switching solution. Unlike easily traceable direct batch transfers, this feature uses same-block smart aggregation to transform chip movements into authentic order book trades. This ensures multi-wallet rebalancing looks natural, aligns with market logic, and breaks up on-chain data clustering.

* Natural Market Logic: Replaces visible direct batch transfers with organic order book volume to cleanly optimize on-chain data footprints.
* Bidirectional Protection: The seamless connection of buy and sell trades slashes slippage and completely blocks MEV sandwich risks.
* Streamlined Operations: Eliminates the hassle of manual account-switching, multiplying time savings while building a robust liquidity defense line.

***

## **Step by Step |** PumpFun Sell & Bundled Buy

{% stepper %}
{% step %}
### Connect Wallet

Click the button in the top right corner to connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image (836).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select a Token to Trade

You can choose to enter the token address, or select a token currently owned by your wallet to perform the sell and buyoperation.

<figure><img src="../../../.gitbook/assets/image (867).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Input Seller Private Keys & Set Sell Amount

{% hint style="danger" %}
<mark style="color:$danger;">**Security Tips**</mark>

Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (868).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Input Buyer Wallet Private Key

{% hint style="danger" %}
<mark style="color:$danger;">**Security Tips**</mark>

Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

{% hint style="info" %}
<mark style="color:$primary;">**Bundle Settings**</mark>

There is no limit on the number of imported wallets for **PumpFun Sell & Bundled Buy**, but each transaction group supports a maximum of **20 addresses** for bundled buying.

The service fees for the Multi-address Bundled Buy are paid entirely by the first address of each group, and the Jito tip is paid by the last address imported. Please ensure that the first and last addresses imported have sufficient balances.
{% endhint %}

Supports two methods for importing sending private key: **"Manual Input"** and **"Upload File"**. Select an option to view the detailed tutorial.

{% tabs %}
{% tab title="Manual Input" %}
1. Click the **"Manual Input"** button to open the input field.

<figure><img src="../../../.gitbook/assets/image (842).png" alt=""><figcaption></figcaption></figure>

2. Enter / bulk paste private keys, one private key per line. Press Enter to start a new line.

<figure><img src="../../../.gitbook/assets/image (787).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (845).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Click the **"Upload File"** button to open the file upload window.

<figure><img src="../../../.gitbook/assets/image (843).png" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (790).png" alt=""><figcaption></figcaption></figure>

2. Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.   \
   Click to download and view the template:

{% file src="../../../.gitbook/assets/Solana_privateKey_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (791).png" alt=""><figcaption></figcaption></figure>

3. Click **"OK"** to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (844).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Enter Buy Amount

Supports three buy amount types: **"Individual Input", "Amount",** and **"Percentage"**.

1.  **Individual Input**\
    In the input fields, enter the buy amount for each address one by one.

    <figure><img src="../../../.gitbook/assets/image (846).png" alt=""><figcaption></figcaption></figure>
2. **Amount:**\
   Click the **"Batch Input"** button above the buy amount, select the "Amount" option, and enter the amount. All addresses will then have a uniform buy amount applied.
3. **Percentage:**\
   Click the **"Batch Input"** button above the buy amount, select the "Percentage" option, and enter the percentage parameter. All addresses will then execute the buy operation based on the specified percentage of their respective balances.

<figure><img src="../../../.gitbook/assets/image (847).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Confirm

After verifying all details, click the **"Bundled Buy"** button below and wait for the transaction process to complete.
{% endstep %}
{% endstepper %}

***

## **FAQs**

<details>

<summary><strong>What Is the PumpFun Sell &#x26; Bundle Buy Feature?</strong></summary>

Sell & Bundle Buy is an advanced asset migration tool built for Pump.fun. It allows a designated wallet to sell tokens while multiple wallets simultaneously execute buy orders within the same block. Using block-level transaction coordination, assets can be redistributed across wallets through real market trades.

</details>

<details>

<summary><strong>How Is It Different from Fragmentation?</strong></summary>

The main difference lies in how assets are moved on-chain.

**Fragmentation (Transfer-Based)**\
Tokens are distributed directly from one wallet to multiple wallets through standard transfers. No market trades occur, making it suitable for simple asset distribution without affecting market activity.

**Sell & Bundle Buy (Trade-Based)**\
Assets are redistributed through real sell and buy transactions on the market rather than direct transfers. This creates normal trading records on-chain and removes direct transfer links between wallets.

</details>

<details>

<summary><strong>Does Sell &#x26; Bundle Buy Affect Market Data?</strong></summary>

Yes. Since the process is completed through actual market transactions on Raydium, it naturally generates trading activity while redistributing assets. This can contribute to trading volume, active wallet participation, and broader token distribution across multiple addresses.

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
