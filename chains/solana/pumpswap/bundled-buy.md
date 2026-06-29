---
description: >-
  Custom-built for PumpSwap, this tool executes multi-wallet purchases within a
  single block, securely optimizing holder distribution and boosting asset
  allocation efficiency.
---

# PumpSwap - Multi-Address Bundled Buy Tutorial

{% hint style="info" %}
**CiaoTool PumpSwap Multi-Address Bundled Buy** now fully supports all quote tokens, including official **SOL and USDC**. Please switch to the specific pool function page first to perform bundled operations.
{% endhint %}

## What is CiaoTool PumpSwap Multi-Address Bundled Buy?

<figure><img src="../../../.gitbook/assets/image (851).png" alt="CiaoTool Solana Toolkit Page about PumpSwap Multi-address Bundled Buy Feature"><figcaption></figcaption></figure>

**CiaoTool PumpSwap Multi-address Bundled Buy** is an advanced tool for trade execution optimization and on-chain liquidity management. Utilizing smart aggregation technology, it enables multiple independent wallets to synchronously execute batch token purchases on **PumpSwap** within the exact same block.

The core advantage lies in preventing MEV bot interference and capital attrition. By aggregating multiple transactions into a single block, the system minimizes "sandwich attack" risks, drastically enhances execution efficiency, and ensures maximum cost-effectiveness.

This tool helps teams securely and steadily optimize token holder distribution, serving as a critical weapon for executing advanced market making and sophisticated liquidity strategies.

Key Use Cases:

* Initial position building and liquidity layout in professional market making.
* Reducing slippage and MEV sandwich risks during multi-wallet batch buying.
* Securely and steadily promoting a healthy distribution of token addresses.
* Enhancing the overall efficiency of multi-address on-chain asset allocation and funds deployment.

Start your Multi-address Bundled Buy on PumpSwap with CiaoTool now:

{% embed url="https://ciaotool.io/en-US/pumpSwap/multi-address-buy" %}

***

## Why Choose CiaoTool PumpSwap Multi-Address Bundled Buy?

CiaoTool offers a professional Solana liquidity solution, balancing execution efficiency with cost protection. Whether for initial position building, evading MEV sandwich attacks, or optimizing holder distribution, its Multi-address Bundled Buy leverages same-block smart aggregation to eliminate manual account-switching, saving valuable operational time.

* Anti-MEV & Low Slippage: Custom-built for Solana to minimize slippage attrition and completely block interference from predatory on-chain bots.
* Automated Batching: Powering efficient multi-wallet asset allocation and fast positioning without tedious manual address management.
* Elite Tooling: Serving as an indispensable liquidity management weapon for Web3 project parties and professional teams.

***

## **Step by Step |** PumpSwap Multi-address Bundled Buy

{% stepper %}
{% step %}
### Connect Wallet

Click the button in the top right corner to connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image (836).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select a Token to Trade

You can choose to enter the token address, or select a token currently owned by your wallet to perform the buy operation.

<figure><img src="../../../.gitbook/assets/image (841).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Input Trading Wallet Private Key

{% hint style="danger" %}
<mark style="color:$danger;">**Security Tips**</mark>

Currently supports private key import only. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

{% hint style="info" %}
<mark style="color:$primary;">**Bundle Settings**</mark>

There is no limit on the number of imported wallets for **PumpSwap Multi-address Bundled Buy**, but each transaction group supports a maximum of **20 addresses** for bundled buying.

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

<summary><strong>What is the PumpSwap Multi-address Bundled Buy feature?</strong></summary>

Multi-address Bundled Buy refers to the synchronous execution of buy operations across multiple wallets within the exact same block. By packaging multiple transactions together for execution, it minimizes price fluctuations caused by time gaps, thereby reducing slippage and enhancing overall execution efficiency. This mechanism is especially suitable for critical trading phases such as market opening and position building.

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
