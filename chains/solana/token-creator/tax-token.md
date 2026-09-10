---
description: >-
  One-click Solana token creation for Token-2022 deployment with built-in
  transfer tax support. Secure client-side processing with seamless support for
  liquidity management and multi-wallet operations.
---

# Solana - Tax Token Creator Guide

{% hint style="info" %}
You are currently on the **"Solana - Taxable Token Creator"** tutorial page.

Click [**"Solana - Standard Token Creator"**](standard-token.md) to view tutorials for strandard token creator.
{% endhint %}

## Overview

CiaoTool provides a no-code tax token creation tool based on Solana’s Token-2022 program. Users can configure the transfer fee rate, maximum fee per transaction, and mint, freeze, and fee management authorities to quickly launch a token.

During token trades and transfers, the program automatically deducts the configured fee. The withheld amount is first recorded in the recipient’s token account and can later be collected into a designated account by the fee withdrawal authority. It does not enter the fee-collection wallet immediately after each transfer. [Solana Documentation](https://solana.com/docs/tokens/extensions/transfer-fees)

**Use Cases:**

* **Community Treasury:** Allocate collected fees to development, operations, and community incentives
* **Deflationary Mechanism:** Periodically burn collected tokens to reduce the circulating supply
* **Revenue Distribution:** Build a sustainable fee distribution model for the token
* **Mechanism Innovation:** Combine compatible Token-2022 extensions to support additional use cases

Start your Standard Token Creator on Solana with CiaoTool now:

{% embed url="https://ciaotool.io/en/token/tax-token" %}

***

## Advantage

* **Secure and Controllable:** Transactions are created in the frontend and signed by the wallet. Private keys are not uploaded, and token and fee authorities remain configurable by the creator.
* **No-Code Creation:** Configure the fee rate, maximum fee per transaction, and other parameters through a visual interface without writing smart contract code.
* **Protocol-Level Execution:** Built on the Token-2022 transfer fee extension, with fees automatically calculated and deducted by the on-chain program.
* **Complete Toolset:** Connect with CiaoTool’s fee management, liquidity, and market management tools for needs ranging from token creation to ongoing operations.

***

## **Video Tutorial**

{% hint style="info" %}
If you prefer video tutorials, this feature has a similar workflow to the Tax Token Creator page. You can refer to and watch this tutorial.
{% endhint %}

{% embed url="https://www.youtube.com/watch?v=efxCzNAMpYE" %}

***

## **Step by Step**

{% stepper %}
{% step %}
### Connect Wallet

Click the button in the top right corner, and connect a wallet that supports the Solana network.

<figure><img src="../../../.gitbook/assets/image.png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Enter Token Info

<figure><img src="../../../.gitbook/assets/image (1144).png" alt=""><figcaption></figcaption></figure>

{% hint style="info" %}
**Clone:** Click the **"Clone"** button to copy information from another token.
{% endhint %}

* **Token Name:** The full name of the token as you wish it to be displayed in wallets or block explorers (e.g., MyFirstToken).
* **Token Symbol:** The abbreviation of the token, typically 3 to 6 uppercase letters (e.g., MYT).
* **Decimals:** Refers to the minimum number of decimal places a token can be divided into. The most common choice is 6 / 9.
* **Total Supply:** The total volume of tokens to be issued.
* **LOGO：**&#x55;pload the logo image for your project or token. A recommended dimension is 1000\*1000 pixels.
* **Description:** A brief introduction to the token's utility, story, or Memecoin background (Optional).
{% endstep %}

{% step %}
### Tax Fee Configuration

* **Fee Rate:** The percentage fee charged on each transaction or transfer.
* **Maximum Tax:** The maximum fee charged for a single transaction or transfer.
* **Fee Authority Address:** The address authorized to manage the token’s fee settings. Defaults to the connected wallet.
* **Fee Withdrawal Authority:** The address authorized to withdraw accumulated token fees. Defaults to the connected wallet.
{% endstep %}

{% step %}
### Add Links <mark style="color:$info;">(Ops)</mark>

Although optional, adding your **website, X / Twitter, Telegram, and Discord** is recommended to help improve project credibility.

<figure><img src="../../../.gitbook/assets/image (1145).png" alt=""><figcaption></figcaption></figure>
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
### Authority Settings

Revoking an authority permanently disables future changes to the related token settings but may help increase trader confidence. Revoked authorities cannot be restored, so confirm that all information is correct before proceeding.

<figure><img src="../../../.gitbook/assets/image (1147).png" alt=""><figcaption></figcaption></figure>

* **Metadata Update Authority:** Once revoked, the token name, symbol, description, image, and other metadata can no longer be modified.
* **Freeze Authority:** Once revoked, no token account can be frozen.
* **Mint Authority:** Once revoked, no additional tokens can be minted, keeping the token supply fixed.
{% endstep %}

{% step %}
### Jito Tips

Use a Jito tip to improve landing priority and execute transactions in the preset order.
{% endstep %}

{% step %}
### Confirm

After confirming the details, click **“Create Token”** to track the creation progress and result in real time.

<figure><img src="../../../.gitbook/assets/image (1148).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Create Liquidity Pool

Once the token creation is complete, it does not yet possess trading attributes and can only be used for transfer operations. Add a liquidity pool to enable your token to be freely traded and swapped on decentralized platforms.

Click to go to Raydium to create a liquidity pool:

{% embed url="https://raydium.io/liquidity-pools/" %}
{% endstep %}
{% endstepper %}

***

## **More Tools**

{% columns %}
{% column %}
{% content-ref url="tax-fee-claim.md" %}
[tax-fee-claim.md](tax-fee-claim.md)
{% endcontent-ref %}
{% endcolumn %}

{% column %}
{% content-ref url="../multisender/one-to-many.md" %}
[one-to-many.md](../multisender/one-to-many.md)
{% endcontent-ref %}
{% endcolumn %}
{% endcolumns %}

## **FAQs**

<details>

<summary><strong>Are transaction fees charged during trading or during transfers?</strong></summary>

Both transfers and trades will generate transaction fees, and this cannot be changed. Solana does not allow for scenario-specific configurations like BSC does.

</details>

<details>

<summary><strong>Can the transaction fees be paid in USDT or SOL?</strong></summary>

No. Under the Token-2022 standard, transaction fees can only be collected in the project's native token (the specific token you create).

</details>

<details>

<summary><strong>Is the token creation address whitelisted? Are transfers or trades from it tax-free?</strong></summary>

Solana tokens do not feature whitelist functionality. All address transfers and trades will incur transaction fees, and the authority address is no exception.

</details>

<details>

<summary><strong>Is the transaction fee paid by the sender's address or the recipient's address?</strong></summary>

If a user initiates a transfer of 1,000 tokens with an assumed tax rate of 10%, the recipient will receive 900 tokens.

</details>

<details>

<summary><strong>Can I still modify the metadata after the token is launched?</strong></summary>

As long as you have not revoke the update authority for the metadata, you are free to modify it. If you revoke the metadata update authority, the data can no longer be modified, and you would have to create a new token.

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
