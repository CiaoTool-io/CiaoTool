---
description: >-
  One-to-Multi transfer is an efficient token distribution tool that sends
  tokens from a single wallet to multiple addresses in bulk. It is suitable for
  airdrops, rewards, and batch settlements.
---

# EVM - Multisender | One-to-Multi Transfer Tutorial

{% hint style="info" %}
You are currently on the **"EVM - One-to-Multi Transfer"** tutorial page for EVM networks including **BSC, opBNB, Base, X Layer, IoTeX, and BOT Chain.**

Demonstrated on BSC. Universally compatible across all EVM networks, please switch to your target chain to operate.

Click [**"Solana - One-to-Multi Transfer"**](../../../chains/solana/multisender/one-to-many.md) to view the Solana network multisender tutorial.
{% endhint %}

## What is CiaoTool EVM One-to-Multi Transfer? <a href="#definition" id="definition"></a>

<figure><img src="../../../.gitbook/assets/image (901).png" alt="CiaoTool BSC Toolkit Page about BSC One-to-Multi Transfer Feature"><figcaption></figcaption></figure>

CiaoTool EVM One-to-Multi Transfer is a batch asset distribution tool designed for BSC and EVM-compatible networks. It enables users to send native tokens (BNB, ETH, etc.) or BEP-20 / ERC-20 tokens from a single wallet to hundreds of recipient addresses in one operation.

By automating large-scale transfers, it eliminates repetitive manual transactions and significantly improves distribution efficiency, making it ideal for token airdrops, team payments, treasury allocation, and large-scale Web3 campaigns.

**Common Use Cases:**

* Token airdrops and distributions
* DAO rewards and incentives
* Batch payments
* Marketing campaigns and Web3 growth initiatives

Start your One-to-Multi Transfer on EVM Network with CiaoTool now:

<table data-view="cards"><thead><tr><th></th><th data-hidden data-card-target data-type="content-ref"></th></tr></thead><tbody><tr><td><img src="../../../.gitbook/assets/BSC.png" alt="" data-size="line">BSC (BNB Chain)</td><td><a href="https://bsc.ciaotool.io/en/transfer/one-to-many">https://bsc.ciaotool.io/en/transfer/one-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/BSC.png" alt="" data-size="line">opBNB</td><td><a href="https://opbnb.ciaotool.io/en/transfer/one-to-many">https://opbnb.ciaotool.io/en/transfer/one-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/Base3.png" alt="" data-size="line">Base</td><td><a href="https://base.ciaotool.io/en/transfer/one-to-many">https://base.ciaotool.io/en/transfer/one-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/3 (1).png" alt="" data-size="line">X Layer</td><td><a href="https://xlayer.ciaotool.io/en/transfer/one-to-many">https://xlayer.ciaotool.io/en/transfer/one-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/IoTex.png" alt="" data-size="line">IoTeX</td><td><a href="https://iotex.ciaotool.io/en/transfer/one-to-many">https://iotex.ciaotool.io/en/transfer/one-to-many</a></td></tr><tr><td><img src="../../../.gitbook/assets/BOT-2.png" alt="" data-size="line"> BOT</td><td><a href="https://bot.ciaotool.io/en/transfer/one-to-many">https://bot.ciaotool.io/en/transfer/one-to-many</a></td></tr></tbody></table>

***

## Why Choose CiaoTool EVM One-to-Multi Transfer?

CiaoTool provides a secure and efficient solution for large-scale asset distribution across EVM networks.

**Massive Efficiency Gains**\
Execute hundreds or thousands of transfers in a single operation, eliminating repetitive manual transactions and wallet switching.

**Lower Transaction Costs**\
Batch processing reduces the number of on-chain interactions, helping minimize overall network fees for large distributions.

**Flexible Distribution Options**\
Import recipient lists via spreadsheet and configure equal, fixed, or random distribution amounts to match different allocation strategies.

**Local Security**\
All signing is performed locally in your browser. Private keys are never uploaded or stored, ensuring full control of your assets.

***

## Video Tutorial <a href="#video-guide" id="video-guide"></a>

{% embed url="https://www.youtube.com/watch?v=xgrsLeEC9Ok" %}

***

## **Step by Step** <a href="#solana-one-to-multi-guide" id="solana-one-to-multi-guide"></a>

{% stepper %}
{% step %}
### Switch Chain & Connect Wallet

Select your target blockchain and connect an EVM-compatible wallet.

<figure><img src="../../../.gitbook/assets/image (902).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Select Funding Wallet

{% hint style="danger" %}
<mark style="color:$danger;">**Security Tips**</mark>

When use private key import. Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (905).png" alt=""><figcaption></figcaption></figure>

**Connected Wallet:** Use your connected wallet to perform transfers directly, without entering a private key. This provides enhanced security. Due to wallet signature limitations, a **maximum of 200 recipient addresses** is supported per transfer.

**Other Wallets:** Use a private key to perform transfers from another wallet. This allows quick access to backup wallets. Since transactions are not limited by wallet signature prompts, there is **no limit on the number of recipient addresses**, and transfer intervals can be configured.
{% endstep %}

{% step %}
### Select Transfer Token

You can select BNB or choose any token currently held in your wallet to execute the multi-transfer.

<figure><img src="../../../.gitbook/assets/image (906).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### **Import Recipient Addresses** <a href="#import-recipient-addresses" id="import-recipient-addresses"></a>

Supports two methods for importing recipient addresses: **"Manual Input"** and **"Upload File"**. Select an option to view the detailed tutorial.

{% tabs %}
{% tab title="Manual Input" %}
Enter / bulk paste wallet addresses, one address per line. Press Enter to start a new line.

<figure><img src="../../../.gitbook/assets/image (903).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Click the "Upload File" button to open the file upload window.

<figure><img src="../../../.gitbook/assets/image (904).png" alt=""><figcaption></figcaption></figure>

2. Use a CiaoTool-compatible file template, then confirm import to display the data in the input field.   \
   Click to download and view the template:

{% file src="../../../.gitbook/assets/EVM_address_demo.xlsx" %}

<figure><img src="../../../.gitbook/assets/image (903).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Enter Transfer Amount

<figure><img src="../../../.gitbook/assets/image (907).png" alt=""><figcaption></figcaption></figure>

Supports two transfer amount types: "Same Amount" and "Custom Amount". Click to view the detailed walkthrough for each.

{% tabs %}
{% tab title="Same Amount" %}
Below the wallet address input field, enter the uniform token amount to be transferred.

<figure><img src="../../../.gitbook/assets/image (908).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Custom Amount" %}
1. **Import via Excel**\
   Create an additional column in your sheet and enter the specific token amount for each recipient address.

<figure><img src="../../../.gitbook/assets/image (507).png" alt=""><figcaption></figcaption></figure>

2. **Manual Text Input**\
   Enter the token amount directly after each wallet address, using a standard English comma to separate the address and the transfer amount.

```
例如：0x0000000000000000000000000000000000000000,300
```

<figure><img src="../../../.gitbook/assets/image (909).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Multisender Time Interval

{% hint style="warning" %}
_Available for "Other Wallets" only. Set custom delay intervals between transactions._
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (910).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### **Confirm** <a href="#confirm" id="confirm"></a>

After verifying all details, click the **"Send"** button below and wait for the transaction process to complete.
{% endstep %}
{% endstepper %}

***

## **FAQs**

<details>

<summary><strong>What Is One-to-Multi Multisender?</strong></summary>

One-to-Multi Multisender allows a single wallet to send tokens to multiple recipient addresses in one operation. It is commonly used for airdrops, reward distribution, and asset allocation.

</details>

<details>

<summary><strong>How Do I Import Recipient Addresses?</strong></summary>

You can manually enter addresses or upload an Excel file containing recipient addresses (supports address + amount format). The system will automatically recognize and preview the imported data.

</details>

<details>

<summary><strong>Can I Send Different Amounts to Different Addresses?</strong></summary>

Yes. You can assign a different transfer amount to each address, or set a unified amount or fixed amount for all recipient addresses.

</details>

<details>

<summary><strong>Is It Secure?</strong></summary>

The platform uses a fully client-side signing mechanism. Your private key is never uploaded or stored on any server, and all transactions are signed locally in your browser, ensuring the platform cannot access your private key.

</details>

<details>

<summary><strong>How Many Addresses Can I Send To at Once?</strong></summary>

The limit depends on the wallet mode selected. When using the private key import mode, there is no limit on the number of recipient addresses, as transfers can be executed without individual wallet signature prompts.

</details>

<details>

<summary><strong>Can I Transfer Multiple Tokens at the Same Time?</strong></summary>

The current version supports batch transfers of one token per operation. To distribute multiple assets, you can run multiple transfers or use the [**Batch One-to-Multi**](one-to-many-multi.md) feature.

</details>

***

**Need help? Join our community for real-time support:**

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
