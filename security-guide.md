---
description: >-
  Your fund security is our top priority. CiaoTool protects your private keys
  with transparent, easy-to-verify mechanisms, ensuring a safe Web3 experience
  for everyone.
---

# CiaoTool Fund Security Assurance Guide

## How Does CiaoTool Ensure Your Fund Security?

Security is paramount at CiaoTool. Our platform operates on **a client-side signing architecture**, meaning **your private keys are processed locally** in your browser. **We never upload or store your private keys on any server, making it technically impossible for us to access your funds.** Your private keys remain exclusively in your control, with all signatures and transactions processed within your local browser, ensuring maximum security and operational transparency.

As a **frontend Web3 SaaS Tool**, we adhere to the "Four No" principle and a stateless operation strategy to comprehensively safeguard your assets.

***

## Core Security Commitments

#### 1. Zero Access Policy

* **No Uploads, No Storage, No Interception**
* Private keys and seed phrases are used only for local signing within your browser memory
* Sensitive data is never uploaded to our servers or stored in any cloud service
* The platform cannot freeze, transfer, or intercept your funds

#### 2. No Storage Mechanism

* Sensitive operations support both manual input and local file import
* All private key data is completely cleared from memory when the page is closed or refreshed
* **No storage service is provided**, ensuring private keys are never retained long-term

#### 3. Transparent Verification

{% columns %}
{% column width="50%" %}
* Any web tool that accesses private keys must send them to a backend server through an HTTPS request
* Users are encouraged to verify network activity using browser developer tools (**F12 → Network → Fetch/XHR**)
* After entering a private key and performing an operation, network requests contain only public data such as token prices and routing information
* No private keys, seed phrases, or signing credentials are transmitted to our servers
{% endcolumn %}

{% column width="50%" %}
<figure><img src=".gitbook/assets/image (670).png" alt=""><figcaption></figcaption></figure>
{% endcolumn %}
{% endcolumns %}

***

## Industry Comparison

<table><thead><tr><th width="139">Security Aspect</th><th width="266">CiaoTool</th><th>Traditional Dev Tools / Telegram Bots</th></tr></thead><tbody><tr><td>Private Keys</td><td>Local only</td><td>Server access required</td></tr><tr><td>Fund Ownership</td><td>100% user-owned</td><td>Platform involvement</td></tr><tr><td>Transparency</td><td>Fully auditable</td><td>Not auditable</td></tr><tr><td>Security Model</td><td>Non-custodial</td><td>Semi-custodial / Custodial</td></tr><tr><td>Verifiability</td><td>✅</td><td>❌</td></tr></tbody></table>

***

## User Security Guidelines

**Start with a Small Test**

* Test with a small amount before committing larger funds
* Verify that the entire process works as expected

**Isolate Operational Funds**

* Avoid using your primary asset wallet
* Use a dedicated wallet for transactions and transfer only the funds required

**Protect Your Devices**

* Ensure your device is free from malware and malicious extensions
* Avoid entering private keys on public devices or unsecured networks
* Disconnect your wallet and clear your clipboard after use

**Rotate Wallets Regularly**

* Avoid relying on the same wallet for extended periods
* Regular wallet rotation helps reduce potential exposure risks
