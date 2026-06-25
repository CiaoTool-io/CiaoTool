---
description: >-
  CiaoTool batch rent reclamation frees SOL by closing unused token and NFT
  accounts across multiple Solana addresses.
---

# Solana - Batch Rent Recovery Tutorial

{% hint style="success" %}
**Solana Batch Rent Recovery：**[https://ciaotool.io/en-US/wallet/manage/reclaim-rent-batch](https://ciaotool.io/en-US/wallet/manage/reclaim-rent-batch)
{% endhint %}

#### 🔗 Steps to Operate

**Step 1: Import Wallets**

* You can manually enter private keys or upload a CSV file containing multiple private keys.
* The system will scan the account usage under each wallet.

**Step 2: Select Reclamation Type**

* ✅ Reclaim Empty Accounts Only: Automatically identifies and closes accounts with zero balance.
* 🔁 Reclaim All Accounts: Includes burnable token and NFT accounts; assets are burned before closing the accounts.

<figure><img src="../../../.gitbook/assets/image (739).png" alt=""><figcaption></figcaption></figure>

**Step 3: Configure SOL Reclamation Address**

* By default, the released SOL is returned to the original accounts.
* You can also manually specify a single unified address to centrally manage the reclaimed rent.

**Step 4: Payer Settings (Optional)**

* Supports one wallet paying GAS (fees) on behalf of other addresses, useful for airdrop addresses or accounts without leftover SOL.

<figure><img src="../../../.gitbook/assets/image (740).png" alt=""><figcaption></figcaption></figure>

#### ❓Frequently Asked Questions <a href="#frequently-asked-questions" id="frequently-asked-questions"></a>

**1. What types of accounts can be reclaimed?**

* **Answer:** SPL Token accounts, NFT accounts, and zero-balance accounts can all be reclaimed to release the associated rent if no longer needed.

**2. Can all reclaimed SOL be sent to a single address?**

* **Answer:** Yes. You can manually set a single collection address, and all released SOL will be transferred there for centralized management.

**3. Can wallets without GAS (SOL) still perform reclamation?**

* **Answer:** Yes. By enabling the "Fee Payer" feature, the system will use a designated wallet to cover gas fees for other wallets, allowing for low-cost batch operations.

**4. Is batch processing of multiple addresses supported?**

* **Answer:** Yes. You can import multiple wallets (via private keys or JSON files) and perform unified account scanning and reclamation in one go.

💬 **Need help? Join our community for real-time support:** [https://t.me/ciaotool](https://t.me/ciaotool)

* **Email:** [support@ciaotool.io](mailto:support@ciaotool.io)
* **Website:** [https://ciaotool.io](https://ciaotool.io/)
* **X (Twitter):** [https://x.com/CiaoTool](https://x.com/CiaoTool)
* **Blog**: [https://www.ciaoailiquidity.com/blog](https://www.ciaoailiquidity.com/blog)
* **Medium:** [https://medium.com/@ciaotool](https://medium.com/@ciaotool)
* **YouTube:** [https://www.youtube.com/@CiaoTool](https://www.youtube.com/@CiaoTool)
* **WhatsApp：**[https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J](https://whatsapp.com/channel/0029VbAuLrVAojYxRNw95W1J)

{% hint style="danger" %}
**Note:** CiaoTool is committed to providing convenient tooling services but does not offer any form of investment advice. Platform content may change with product iterations. Users are advised to exercise judgment and stay informed about updates.
{% endhint %}
