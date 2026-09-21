---
description: >-
  Batch query and claim holder rewards for Flap.sh tokens, with multi-address
  imports, automatic verification, grouped execution, and progress tracking.
---

# Flap - Dividend Claim Guide

## Overview

**CiaoTool Flap Dividend Claim** is a batch dividend claiming tool for BNB Chain. It supports Flap Standard dividend tokens.

Users can import multiple token and holder addresses. The system automatically queries claimable dividends, verifies claim status, and submits transactions in groups. The payment wallet covers BNB Gas and platform service fees, while dividends are sent directly to the corresponding entitlement addresses without changing their original ownership.

**Use Cases:**

* Batch claiming dividends for multiple wallets
* Consolidating rewards from project and operational wallets
* Paying claim fees on behalf of other holders
* Managing dividends across multiple tokens and addresses
* Checking claimable amounts and execution status in batches

{% embed url="https://bsc.ciaotool.io/en/flap/batch-claim-dividend" %}

***

## Key Advantages

* **Batch Claims:** Import multiple token and recipient address records at once
* **Flexible Configuration:** Use one shared token or recipient address, or configure each record individually
* **Automatic Verification:** Automatically query tax information, claimable amounts, and claim status
* **Local Security:** Private keys are used only for local transaction signing and are never uploaded or stored on a server

***

## Step by Step

{% stepper %}
{% step %}
### Payment Wallet

Enter the private key of the wallet used to execute the claiming task in the **Payment Wallet Private Key** field.

The payment wallet is responsible for:

* [x] Calling the Flap dividend contracts
* [x] Paying BNB Gas
* [x] Paying platform service fees
{% endstep %}

{% step %}
### Token Address

Select how token addresses should be configured:

* **Single Token Address:** All records use the same token contract address
* **Different Token Address for Each Entry:** Each claim record uses its own token address

When using a single token address, enter the token contract address in the field below.
{% endstep %}

{% step %}
### Recipient Address

Select how dividends should be received:

* **Single Recipient Address:** All dividends are sent to the same entitlement address
* **Original Address:** Each holder address receives its corresponding dividends

The recipient address must own the Flap dividend entitlement for the selected token. The payment wallet can only pay the claiming fees and cannot change dividend ownership.
{% endstep %}

{% step %}
### Dividend List

Click **Import Dividend List**, then paste Excel data or upload an address file.

Use the corresponding import format:

* **Single Token + Original Address:** Enter one recipient address per row
* **Different Tokens + Single Recipient:** Enter one token address per row
* **Different Tokens + Original Address:** Enter one token address and one recipient address per row
* **Single Token + Single Recipient:** The system automatically creates one claim record

Invalid records are automatically filtered out. Duplicate token-and-recipient combinations are removed without case sensitivity.
{% endstep %}

{% step %}
### Check

After importing the list, click **Refresh Check**.

The system checks the first 10 records and displays:

* Token and tax information
* Dividend recipient address
* Claimable dividend amount
* Current claim status
* Error or skip reason

The remaining records are checked in groups after the claiming task starts.
{% endstep %}

{% step %}
### Start

After confirming the information, click **Start Claiming Dividends**.

The system will automatically:

1. Check 10 claim records per group
2. Verify the claimable dividends again
3. Check Gas, service fees, and the payment wallet balance
4. Bundle and submit up to 20 claim transactions per batch
5. Continue processing the next batch after the previous batch is confirmed
{% endstep %}
{% endstepper %}

***

## Service Support

Need help? Join our community for real-time support:

<table data-header-hidden><thead><tr><th width="188"></th><th valign="top"></th><th data-hidden></th></tr></thead><tbody><tr><td>Email</td><td valign="top"><a href="mailto:ciaotoolglobal@gmail.com">ciaotoolglobal@gmail.com</a></td><td></td></tr><tr><td>Telegram</td><td valign="top"><a href="https://t.me/ciaotools">https://t.me/ciaotools</a></td><td></td></tr><tr><td>WhatsApp</td><td valign="top"><a href="https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J">https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J</a></td><td></td></tr></tbody></table>

{% hint style="danger" %}
CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
