---
description: >-
  Learn how to find and verify the correct V3 Pool Address using DEXTools. Check
  the network, DEX, token pair, protocol version, fee tier, and liquidity before
  using CiaoTool V3 tools.
---

# How to Find a V3 Pool Address | CiaoTool Guide

## What Is a V3 Pool Address?

A V3 Pool Address is the smart-contract address of a specific V3 liquidity pool. It is determined by the following information:

* Blockchain network;
* DEX and protocol version;
* Token0;
* Token1;
* Fee tier.

Unlike V2, the same two tokens may have multiple V3 pools with different fee tiers. For example, Token A and Token B may have separate V3 pools using 0.01%, 0.05%, 0.30%, or 1.00% fee tiers.

Each of these pools has a different Pool Address, liquidity depth, current price, trading activity, and execution result.

Under the V3 contract architecture, a pool is defined by two tokens and a fee tier. Therefore, the same token pair can have multiple pools with different fee tiers.

[Learn more about the Uniswap V3 architecture](https://developers.uniswap.org/docs/protocols/v3/concepts/architecture).

***

## Why Must You Use the Exact Pool Address?

When a V3 tool asks for a Pool Address, entering only the token contract address is not enough.

The exact Pool Address helps CiaoTool determine which liquidity pool should be used to:

* Read the current pool price;
* Identify Token0 and Token1;
* Confirm the fee tier;
* Estimate liquidity and price impact;
* Build the Swap route;
* Submit the transaction to the intended pool.

If the wrong Pool Address is entered, the page may load the wrong token pair, select an unintended fee tier, display incorrect market information, or fail to submit the transaction.

***

## Before You Start

Prepare the following information:

* Target blockchain network;
* Base-token contract address;
* Quote-token contract address;
* Target DEX;
* Protocol version, such as V3;
* Target fee tier.

Always search using the exact **token contract address** instead of only the token name or symbol. Different tokens may use identical names and symbols.

***

## Step-by-Step Guide

Many third-party on-chain data tools can quickly display all liquidity pools currently associated with a token.

In this guide, we use **DEXTools** as an example. By searching for the token contract address, users can compare the token’s pools across different blockchain networks, DEXs, protocol versions, quote tokens, and fee tiers.

{% stepper %}
{% step %}
### Open DEXTools

Visit the official DEXTools website:

<figure><img src="../.gitbook/assets/image (1101).png" alt=""><figcaption></figcaption></figure>

{% embed url="https://www.dextools.io/app/hot-pairs" %}
{% endstep %}

{% step %}
### Select the Correct Network

Select the blockchain network where the target V3 Pool is deployed.

Tokens with the same name or similar address formats may appear on different networks. Make sure the network selected in DEXTools matches the network currently used by CiaoTool.

<figure><img src="../.gitbook/assets/image (1102).png" alt=""><figcaption></figcaption></figure>
{% endstep %}

{% step %}
### Search the Token Contract Address

Paste the exact token contract address into the DEXTools search box.

Searching by contract address is more accurate than searching only by token name or symbol and can reduce the risk of selecting an unrelated or counterfeit token.

After the results appear, verify:

* Token name;
* Token symbol;
* Token contract address.
{% endstep %}

{% step %}
### View All Available Pools

Select the target token and open its corresponding Pair Explorer page.

<figure><img src="../.gitbook/assets/image (1103).png" alt=""><figcaption></figcaption></figure>

DEXTools may display one active or recommended trading pair first. To view the token’s other pools, open the pool-selection area, select **Other Pairs**, or click the binoculars icon near the pool information.

The exact button name or location may change when DEXTools updates its interface.

<figure><img src="../.gitbook/assets/image (1104).png" alt=""><figcaption></figcaption></figure>

Compare the available pools based on:

* DEX name;
* Protocol version;
* Quote token;
* Liquidity;
* Trading volume;
* Pool creation time;
* Fee tier, if displayed.
{% endstep %}

{% step %}
### Copy the Pair Address

Find the Pool that exactly matches the current CiaoTool task.

<figure><img src="../.gitbook/assets/image (1105).png" alt=""><figcaption></figcaption></figure>

Confirm that:

* The blockchain network is correct;
* The Pool belongs to the intended DEX;
* The protocol version is V3;
* Both token contract addresses are correct;
* The quote token is correct;
* The fee tier is correct;
* The Pool has the expected liquidity.

Do not select a Pool only because it has the highest volume or liquidity. The Pool Address must first match the network, DEX, token pair, protocol version, and fee tier required by the task.

After confirming the correct Pool, locate and copy its **Pair Address** from the Pair Explorer page. For a V3 Pool, this Pair Address is the Pool Address required by CiaoTool.

Do not copy the token contract address displayed on the same page.
{% endstep %}

{% step %}
### Enter the Pool Address in CiaoTool

Return to the corresponding CiaoTool V3 page and paste the copied Pair Address into the Pool Address field.

<figure><img src="../.gitbook/assets/image (1106).png" alt=""><figcaption></figcaption></figure>

After the page loads the Pool, review the information detected by CiaoTool:

* Token pair;
* Token symbols;
* Fee tier;
* Current price;
* Pool liquidity;
* Buy or sell direction.

Only continue after the displayed information completely matches the Pool selected in DEXTools.
{% endstep %}
{% endstepper %}

***

## Common Mistakes

#### Copying the Token Address

A token contract address identifies only one token. It does not identify a specific V3 liquidity pool.

#### Selecting the Wrong Network

Tokens with the same name may appear on multiple blockchain networks.

#### Selecting the Wrong DEX

The same token may have liquidity pools on multiple DEXs. Different DEXs use different Pool contracts.

#### Selecting a V2 or V4 Pool

DEXTools may display pools from multiple protocol versions at the same time. Make sure the selected Pool uses V3.
