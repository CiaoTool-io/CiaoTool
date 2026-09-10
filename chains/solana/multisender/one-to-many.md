---
description: >-
  One-to-Multi Transferis a bulk distribution tool that sends SOL or SPL tokens
  from a single wallet to multiple addresses in one operation. Ideal for
  airdrops, rewards, and batch payments.
---

# Solana - Multisender | One-to-Multi Transfer Tutorial

{% hint style="info" %}
You are currently on the **"Solana - One-to-Multi Transfer"** tutorial page.

Click [**"EVM - One-to-Multi Transfer"**](../../../tools/multisender/one-to-multi/one-to-many.md) to view multisender tutorials for EVM networks such as BSC, opBNB, Base, X Layer, IoTeX, BOT, and Robinhood Chain.
{% endhint %}

## Overview <a href="#definition" id="definition"></a>

CiaoTool Solana One-to-Many Transfer is a batch asset distribution tool that allows users to send SOL or supported SPL tokens from one wallet to multiple recipient addresses in a single operation.

The system automatically creates and groups transfer tasks based on the number of recipients. Each transaction supports up to five recipient addresses and is broadcast using the selected sending method, reducing repetitive address entry and individual signing.

**Use Cases:**

* Token airdrops and community rewards
* DAO distributions and contributor incentives
* Team payments and bulk user payouts
* Multi-wallet fund allocation and operational management

Start your One-to-Multi Transfer on Solana with CiaoTool now:

{% embed url="https://ciaotool.io/en/transfer/one-to-many" %}

***

## Advatage

* **Efficient Batch Processing:** Configure multiple recipient addresses and transfer amounts at once, and let the system automatically group and execute the transactions.
* **Flexible Configuration:** Enter details manually or import them in bulk from Excel, with support for equal, fixed, or randomized amounts.
* **Multiple Sending Options:** Choose between RPC broadcasting and Jito bundle submission to suit different execution requirements.
* **Pre-Submission Review:** Verify the number of recipients, total transfer amount, and estimated fees before submitting.
* **Local Signing:** Transactions are authorized by the wallet without uploading private keys.

***

## Tutorial Video <a href="#video-guide" id="video-guide"></a>

{% embed url="https://www.youtube.com/watch?v=u0QQwYpX7WM" %}

***

## Step by Step <a href="#solana-one-to-multi-guide" id="solana-one-to-multi-guide"></a>

{% stepper %}
{% step %}
### Connect Wallet

Click the button in the top right corner, and connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Choose Sender Wallet

{% hint style="danger" %}
Please ensure a secure environment. Your fund security is our top priority. [Learn more about how CiaoTool protects your assets: \[Fund Security Assurance\]](../../../security-guide.md).
{% endhint %}

<figure><img src="../../../.gitbook/assets/image (1).png" alt=""><figcaption></figcaption></figure>

* **Connected Wallet:** Transfer directly with the currently connected wallet. Transactions are authorized through the wallet without entering the private key.
* **Other Private-Key Wallet:** Enter private key to quickly use additional wallet for transfers without switching the connected wallet.
{% endstep %}

{% step %}
### Select a Token to Send

You can choose SOL or any SPL token currently held in your wallet for transfer.

<figure><img src="../../../.gitbook/assets/image (2).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### **Import Recipient Addresses**

Unlimited recipient addresses. Add them **Manually Input** or **Upload File**. Click to view the guide.

{% tabs %}
{% tab title="Manual Input" %}
1. Click the "Bulk Input" button to open the input field.

<figure><img src="../../../.gitbook/assets/image (3).png" alt=""><figcaption></figcaption></figure>

2. Enter / paste wallet addresses, one per line. Optionally add the transfer amount after each address.

```
address, 300
```

<figure><img src="../../../.gitbook/assets/image (4).png" alt=""><figcaption></figcaption></figure>

3. Click "Import" to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>
{% endtab %}

{% tab title="Upload File" %}
1. Download the CiaoTool template and fill in the transfer details.

<figure><img src="../../../.gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

2. Click ![](<../../../.gitbook/assets/image (7).png>)"Import File" button to open the input field.
3. Click "Import" to import all entered addresses into the operation panel.

<figure><img src="../../../.gitbook/assets/image (681).png" alt=""><figcaption></figcaption></figure>
{% endtab %}
{% endtabs %}
{% endstep %}

{% step %}
### Enter Transfer Amount

Choose from 3 amount options: **Individual, Fixed, or Random Range**.

1. **Individual**\
   Enter a different amount for each address.
2. **Fixed Amount**\
   Click ![](<../../../.gitbook/assets/image (8).png>) above “Amount”, and select “Fixed Amount” to apply the same amount to all addresses.
3. **Random Range**\
   Click ![](<../../../.gitbook/assets/image (8).png>) above “Amount”, and select “Random Range” and set the minimum and maximum. The system will generate an amount within that range for each address.
{% endstep %}

{% step %}
### Send Interval

Set the submission interval between transactions.

<figure><img src="../../../.gitbook/assets/image (9).png" alt=""><figcaption></figcaption></figure>

* **Fixed Interval**\
  Set to `0` to broadcast all transactions immediately.
* **Random Interval**\
  Transactions are submitted randomly within the selected time range. Keep the page open during execution.
{% endstep %}

{% step %}
### Send method

The system automatically groups recipients, with up to 5 addresses per group.

<figure><img src="../../../.gitbook/assets/image (10).png" alt=""><figcaption></figcaption></figure>

* **RPC**\
  Broadcasts transactions through an RPC node without a Jito tip. Execution order is not guaranteed.
* **Jito Bundle**\
  Each Bundle supports up to 5 groups, totaling 25 recipients. A Jito tip increases landing priority, and transactions execute in the specified order.
{% endstep %}

{% step %}
### Review Details

Click **“Next”** to review:

* [x] Recipient addresses, total recipients, and transfer amount
* [x] Estimated fees

<figure><img src="../../../.gitbook/assets/image (11).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### **Confirm**

After confirming the details, click **“Confirm and Send”** to track the transfer progress and results in real time.

<figure><img src="../../../.gitbook/assets/image (12).png" alt=""><figcaption></figcaption></figure>
{% endstep %}
{% endstepper %}

***

## **FAQs**

<details>

<summary><strong>What is One-to-Multi Batch Transfer?</strong></summary>

One-to-Multi batch transfer refers to sending tokens from a single wallet address t**o multiple recipient addresses** in one operation. It is commonly used for airdrops, reward distribution, and asset allocation.

</details>

<details>

<summary><strong>How to import recipient addresses?</strong></summary>

You can either manually enter addresses or upload a CSV file to import a list of recipient addresses (supports address + amount format). The system will automatically recognize and display a preview.

</details>

<details>

<summary><strong>Does it support different amounts for different addresses?</strong></summary>

Yes. You can assign different transfer amounts to each address, or set a unified amount or random range to distribute tokens across all recipient addresses.

</details>

<details>

<summary><strong>Is the operation secure?</strong></summary>

CiaoTool uses a fully client-side signing mechanism. Your private key is never uploaded or stored on any server, and all transactions are signed locally in your browser. This ensures, at a technical level, that the platform has no access to your private key.

</details>

<details>

<summary><strong>How many addresses can be sent at once?</strong></summary>

Using the private key import mode, the One-to-Multi Transfer feature eliminates the hassle of signing for every individual wallet, with no limit on the number of recipient addresses.

</details>

<details>

<summary><strong>Can I send multiple types of tokens at the same time?</strong></summary>

The current version supports selecting a single SPL token or SOL for multisender. For multiple asset distributions, you can perform the operation multiple times.

</details>

***

## Service Support

Need help? Join our community for real-time support:

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
