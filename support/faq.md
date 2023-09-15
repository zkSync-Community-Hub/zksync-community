# ❓ FAQ

<details>

<summary>Table of Contents</summary>

* [What is zkSync?](faq.md#what-is-zksync)
* [What is zkSync Era?](faq.md#what-is-zksync-era)
* [What is zkSync Lite?](faq.md#what-is-zksync-lite)
* [How do fees work on zkSync?](faq.md#how-do-fees-work-on-zksync)
* [How long are withdrawal times?](faq.md#how-long-are-withdrawal-times)
* [Where can I see my funds after a withdrawal?](faq.md#where-can-i-see-my-funds-after-a-withdrawal)
* [Can I send funds to or from a Centralized Exchange to zkSync?](faq.md#can-i-send-funds-to-or-from-a-centralized-exchange-to-zksync)
* [What is the account activation fee?](faq.md#what-is-the-account-activation-fee-on-zksync-lite)
* [What do the statuses mean of a transaction?](faq.md#what-do-the-statuses-mean-of-a-transaction)
* [How long does a deposit take?](faq.md#how-long-does-a-deposit-take)
* [Is there a token for zkSync?](faq.md#is-there-a-token-for-zksync)
* [Can I run a validator or a node for zkSync?](faq.md#can-i-run-a-validator-or-a-node-for-zksync)
* [Is there a list of projects in the zkSync Ecosystem?](faq.md#is-there-a-list-of-projects-in-the-zksync-ecosystem)

</details>

## What is zkSync?

zkSync is a user-centric, Layer 2, zkRollup platform from [Matter Labs](https://matter-labs.io/). It is a scaling solution for Ethereum, with two different versions, zkSync Era and zkSync Lite.

{% tabs %}
{% tab title="zkSync Era" %}
## What is zkSync Era?

<table><thead><tr><th>Feature</th><th>zkSync Era (formerly zkSync 2.0)</th><th data-hidden>zkSync Lite (formerly zkSync 1.0)</th></tr></thead><tbody><tr><td><strong>Description</strong></td><td>zkSync Era is a Zero Knowledge (ZK) rollup that supports generalized EVM compatibility for the Ethereum blockchain.</td><td>zkSync Lite is a trustless protocol for scalable low-cost payments on Ethereum, powered by zkRollup technology.</td></tr><tr><td><strong>Mainnet</strong></td><td><a href="https://blog.matter-labs.io/gm-zkevm-171b12a26b36">March 24, 2023</a></td><td><a href="https://blog.matter-labs.io/zksync-is-live-bringing-trustless-scalable-payments-to-ethereum-9c634b3e6823">June 18, 2020</a></td></tr><tr><td><strong>Purpose</strong></td><td>Universal</td><td>Payments, NFTs, Atomic Swaps</td></tr><tr><td><strong>Smart Contracts</strong></td><td>✅</td><td>❌</td></tr></tbody></table>

You can learn more about both protocols on [L2beat.com](https://l2beat.com/scaling/projects/zksync-era).
{% endtab %}

{% tab title="zkSync Lite" %}
## What is zkSync Lite?

<table><thead><tr><th>Feature</th><th>zkSync Lite (formerly zkSync 1.0)</th><th data-hidden>zkSync Era (formerly zkSync 2.0)</th></tr></thead><tbody><tr><td><strong>Description</strong></td><td>zkSync Lite is a trustless protocol for scalable low-cost payments on Ethereum, powered by zkRollup technology.</td><td>zkSync Era is a Zero Knowledge (ZK) rollup that supports generalized EVM compatibility for the Ethereum blockchain.</td></tr><tr><td><strong>Mainnet</strong></td><td><a href="https://blog.matter-labs.io/zksync-is-live-bringing-trustless-scalable-payments-to-ethereum-9c634b3e6823">June 18, 2020</a></td><td><a href="https://blog.matter-labs.io/gm-zkevm-171b12a26b36">March 24, 2023</a></td></tr><tr><td><strong>Purpose</strong></td><td>Payments, NFTs, Atomic Swaps</td><td>Universal</td></tr><tr><td><strong>Smart Contracts</strong></td><td>❌</td><td>✅</td></tr></tbody></table>

You can learn more about zkSync Lite on [L2beat.com](https://l2beat.com/scaling/projects/zksync-lite).
{% endtab %}
{% endtabs %}

## How do fees work on zkSync?

{% tabs %}
{% tab title="zkSync Era" %}
### How do fees work on zkSync Era?

In zkSync Era, the way fees are calculated is similar to Ethereum. Fees are needed for:

1. The work done by the protocol (computational cost).
2. The cost to put data on-chain (publishing data).
3. The effects of storage.
4. Putting data on the L1 chain (publishing to L1).
5. Creating proofs (proof generation).

The fees for putting data on the L1 chain can change a lot due to volatile L1 gas prices. Because of this, the fees on a L2 will rise and fall with L1 fees.
{% endtab %}

{% tab title="zkSync Lite" %}
### How do fees work on zkSync Lite?

Fees depend on Ethereum Layer 1 (L1) gas prices because with every zkSync Layer 2 (L2) transaction, we post related data on Layer 1 — this allows us to inherit the security of Ethereum.
{% endtab %}
{% endtabs %}

## How long are withdrawal times?

{% tabs %}
{% tab title="zkSync Era" %}
### How long are withdrawal times on zkSync Era?

There is currently a 24 hour delay on withdrawals from zkSync Era mainnet to Ethereum L1. You can learn more about the process and reason in our latest [blog post](https://blog.matter-labs.io/securing-zksync-era-execution-delay-ee32b11d6f9)

Once the transaction is ["Committed"](faq.md#what-do-the-statuses-mean-ofa-transaction) the 24 hour delay starts.

You can check our tutorial for <mark style="background-color:blue;">"How to Withrdraw"</mark> for details on how to check if your transaction is past the withdrawal delay.
{% endtab %}

{% tab title="zkSync Lite" %}
### How Long are Withdrawal Times on zkSync Lite?

At peak usage of zkSync, the withdrawal time is about 15 minutes. During lower use, it can take up to 10 hours. Currently, withdrawal times depend on the activity on zkSync, when we finalize blocks, and submit them to L1.
{% endtab %}
{% endtabs %}

## Where can I see my funds after a withdrawal?

{% tabs %}
{% tab title="zkSync Era" %}
### Where can I see my funds after a withdrawal from zkSync Era?

You can find fully verified withdrawals on [Etherscan](https://etherscan.io/) in the "**Internal Transactions**" tab\*. You will have a transaction from the [`zkSync Era:Diamond Proxy` contract](https://etherscan.io/address/0x32400084c286cf3e17e7b677ea9583e60a000324).

\* If you withdrew a token other than ETH then you would find the transaction in the "**Token Transfers(ERC-20)**" tab.
{% endtab %}

{% tab title="zkSync Lite" %}
### Where can I see my Funds after a Withdrawal from zkSync Lite?

You can find fully verified withdrawals on [Etherscan](https://etherscan.io/) in the "**Internal Transactions**" tab\*. You will have a transaction from the [`zkSync` contract](https://etherscan.io/address/0xabea9132b05a70803a4e85094fd0e1800777fbef#tokentxns).

\* If you withdrew a token other than ETH then you would find the transaction in the "**Token Transfers(ERC-20)**" tab.
{% endtab %}
{% endtabs %}

## Can I send funds to or from a Centralized Exchange to zkSync?

{% tabs %}
{% tab title="zkSync Era" %}
### Can I send funds to or from a Centralized Exchange to zkSync Era?

No, you cannot send funds to or from a Centralized Exchange (CEX) until the network is supported by the exchange. To prevent loss of funds, please check with the specific exchange for their policies and support before sending funds to or from zkSync Era to a CEX.

Until there is more CEX support for zkSync Era you can use some third-party bridges to deposit funds from a CEX to zkSync. See our [Ecosystem page](https://ecosystem.zksync.io/) for a list of bridges.
{% endtab %}

{% tab title="zkSync Lite" %}
### Can I send funds to or from a Centralized Exchange to zkSync Lite?

Yes, you can send funds to and from a Centralized Exchange (CEX) to zkSync as long as the CEX supports the zkSync network. However, always ensure to check with the specific exchange for their policies and support. Some third-party bridges allow you to deposit funds from a CEX to zkSync. See our [Ecosystem page](https://ecosystem.zksync.io/) for a list of bridges.
{% endtab %}
{% endtabs %}

## What is the account activation fee on zkSync Lite?

The account activation fee is a one-time fee to register your account with zkSync. This fee only applies to your first zkSync transaction on zkSync Lite and **does not apply to zkSync Era**.

On a deeper level, to be better suited for zero-knowledge proofs, zkSync accounts are defined over a different elliptic curve than Ethereum's. Activating your account generates and publishes a new private-public key pair over this curve associated with your Ethereum address.

The registration process happens directly on the Ethereum smart contract and therefore it is an L1 transaction, so the activation fee is to pay the Ethereum miners and not zkSync validators.

ERC-1271 compatible wallets (like Argent) increase this one-time fee because of higher interaction with the zkSync smart contract. This operation is cheaper if you are using a CREATE2 smart-contract-based wallet.

## What do the statuses mean for a transaction?

{% tabs %}
{% tab title="zkSync Era" %}
### What do the statuses mean for a transaction on zkSync Era?

* **`Indexing`** - In the mempool but not yet included in a block.
* **`Failed`** - Unverified/failed transaction.
* **`zkSync Era Processed, Ethereum Sending`** - Included in a block but the batch containing the block has not yet been committed.
* **`zkSync Era Processed, Ethereum Validating`** -  Included in a block and committed on the Ethereum L1 network.
* **`zkSync Era Processed, Ethereum Executing`** - Included in a block and proven on the Ethereum L1 network.
* **`zkSync Era Processed, Ethereum Executed`** - Included in a block and executed on the Ethereum L1 network.
{% endtab %}

{% tab title="zkSync Lite" %}
### What do the statuses mean for a transaction on zkSync Lite?

* **`Initiated`**: the zkSync server has received and processed the transaction. Unless it is a withdrawal, it is ready for immediate use.
* **`Committed`**: the transaction appears in a block that is committed to the L1 smart contract.
* **`Verified`**: the transaction’s block has been proven and verified on the L1 smart contract.
{% endtab %}
{% endtabs %}

## How long does a deposit take?

A deposit to zkSync is a transaction from Ethereum to zkSync, and it typically takes about 5 minutes or about 10 block confirmations on Ethereum L1. The time can vary based on the congestion of the Ethereum network and the L1 gas fee set for the transaction.

## Is there a token for zkSync?

No

## Can I run a validator or a node for zkSync?

{% tabs %}
{% tab title="zkSync Era" %}
### Can I run a validator or a node for zkSync Era?

Not at the moment, but the network is expected to move towards a more decentralized model, allowing users to run their own validators or nodes in the future.
{% endtab %}

{% tab title="zkSync Lite" %}
### Can I run a validator or a node for zkSync Lite?

No
{% endtab %}
{% endtabs %}

## Is there a list of projects in the zkSync Ecosystem?

Yes, [https://ecosystem.zksync.io/](https://ecosystem.zksync.io/)

## Why don't I see my funds on my wallet?

{% tabs %}
{% tab title="zkSync Era" %}
### Why don't I see my funds on my wallet for zkSync Era?

For zkSync Era make sure you are connected to the zkSync Era mainnet. If you still don't see your funds, you might need to change display settings to either show or add custom tokens on your wallet interface. You can check MetaMask's ["How to display tokens in MetaMask"](https://support.metamask.io/hc/en-us/articles/360015489031-How-to-display-tokens-in-MetaMask) for more details.
{% endtab %}

{% tab title="zkSync Lite" %}
### Why don't I see my funds on my wallet for zkSync Lite?

You will not see your zkSync Lite funds on your wallet unless it is integrated with zkSync Lite like [Argent](https://www.argent.xyz/).\
\
Since you connect to zkSync Lite via Ethereum mainnet your wallet will show you your funds on Ethereum and you can check your zkSync Lite funds on [the zkSync Lite wallet](https://lite.zksync.io/) or [the zkSync Lite block explorer](https://zkscan.io/).
{% endtab %}
{% endtabs %}
