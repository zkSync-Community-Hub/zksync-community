# ❓ FAQ

## What is ZKsync?

ZKsync is a user-centric, Layer 2, zkRollup platform from [Matter Labs](https://matter-labs.io/). It is a scaling solution for Ethereum, with two different versions, ZKsync Era and ZKsync Lite.

{% tabs %}
{% tab title="ZKsync Era" %}
### What is ZKsync Era?

<table><thead><tr><th>Feature</th><th>ZKsync Era (formerly ZKsync 2.0)</th><th data-hidden>ZKsync Lite (formerly ZKsync 1.0)</th></tr></thead><tbody><tr><td><strong>Description</strong></td><td>ZKsync Era is a Zero Knowledge (ZK) rollup that supports generalized EVM compatibility for the Ethereum blockchain.</td><td>ZKsync Lite is a trustless protocol for scalable low-cost payments on Ethereum, powered by zkRollup technology.</td></tr><tr><td><strong>Mainnet</strong></td><td><a href="https://blog.matter-labs.io/gm-zkevm-171b12a26b36">March 24, 2023</a></td><td><a href="https://blog.matter-labs.io/zksync-is-live-bringing-trustless-scalable-payments-to-ethereum-9c634b3e6823">June 18, 2020</a></td></tr><tr><td><strong>Purpose</strong></td><td>Universal</td><td>Payments, NFTs, Atomic Swaps</td></tr><tr><td><strong>Smart Contracts</strong></td><td>✅</td><td>❌</td></tr></tbody></table>

You can learn more about both protocols on [L2beat.com](https://l2beat.com/scaling/projects/zksync-era).
{% endtab %}

{% tab title="ZKsync Lite" %}
### What is ZKsync Lite?

<table><thead><tr><th>Feature</th><th>ZKsync Lite (formerly ZKsync 1.0)</th><th data-hidden>ZKsync Era (formerly ZKsync 2.0)</th></tr></thead><tbody><tr><td><strong>Description</strong></td><td>ZKsync Lite is a trustless protocol for scalable low-cost payments on Ethereum, powered by zkRollup technology.</td><td>ZKsync Era is a Zero Knowledge (ZK) rollup that supports generalized EVM compatibility for the Ethereum blockchain.</td></tr><tr><td><strong>Mainnet</strong></td><td><a href="https://blog.matter-labs.io/zksync-is-live-bringing-trustless-scalable-payments-to-ethereum-9c634b3e6823">June 18, 2020</a></td><td><a href="https://blog.matter-labs.io/gm-zkevm-171b12a26b36">March 24, 2023</a></td></tr><tr><td><strong>Purpose</strong></td><td>Payments, NFTs, Atomic Swaps</td><td>Universal</td></tr><tr><td><strong>Smart Contracts</strong></td><td>❌</td><td>✅</td></tr></tbody></table>

You can learn more about ZKsync Lite on [L2beat.com](https://l2beat.com/scaling/projects/zksync-lite).
{% endtab %}
{% endtabs %}

## How Do Fees Work on ZKsync?

{% tabs %}
{% tab title="ZKsync Era" %}
#### How Do Fees Work on ZKsync Era?

In ZKsync Era, the way fees are calculated is similar to Ethereum. Fees are needed for:

1. The work done by the protocol (computational cost).
2. The cost to put data on-chain (publishing data).
3. The effects of storage.
4. Putting data on the L1 chain (publishing to L1).
5. Creating proofs (proof generation).

The fees for putting data on the L1 chain can change a lot due to volatile L1 gas prices. Because of this, the fees on a L2 will rise and fall with L1 fees.
{% endtab %}

{% tab title="ZKsync Lite" %}
#### How Do Fees Work on ZKsync Lite?

Fees depend on Ethereum Layer 1 (L1) gas prices because with every ZKsync Layer 2 (L2) transaction, we post related data on Layer 1 — this allows us to inherit the security of Ethereum.
{% endtab %}
{% endtabs %}

## How Long are Withdrawal Times?

{% tabs %}
{% tab title="ZKsync Era" %}
#### How Long are Withdrawal Times on ZKsync Era?

There is currently a 24 hour delay on withdrawals from ZKsync Era mainnet to Ethereum L1. You can learn more about the process and reason in our latest [blog post](https://blog.matter-labs.io/securing-zksync-era-execution-delay-ee32b11d6f9)

Once the transaction is ["Committed"](faq.md#what-do-the-statuses-mean-ofa-transaction) the 24 hour delay starts.

You can check our tutorial for ["How to Withrdraw"](tutorials.md#how-to-withdraw) for details on how to check if your transaction is past the withdrawal delay.
{% endtab %}

{% tab title="ZKsync Lite" %}
#### How Long are Withdrawal Times on ZKsync Lite?

At peak usage of ZKsync, the withdrawal time is about 15 minutes. During lower use, it can take up to 10 hours. Currently, withdrawal times depend on the activity on ZKsync, when we finalize blocks, and submit them to L1.
{% endtab %}
{% endtabs %}

## Where Can I See My Funds After a Withdrawal?

{% tabs %}
{% tab title="ZKsync Era" %}
#### Where Can I See My Funds After a Withdrawal from ZKsync Era?

You can find fully verified withdrawals on [Etherscan](https://etherscan.io/) in the "**Internal Transactions**" tab\*. You will have a transaction from the [`ZKsync Era:Diamond Proxy` contract](https://etherscan.io/address/0x32400084c286cf3e17e7b677ea9583e60a000324).

\* If you withdrew a token other than ETH then you would find the transaction in the "**Token Transfers(ERC-20)**" tab.
{% endtab %}

{% tab title="ZKsync Lite" %}
#### Where Can I See My Funds After a Withdrawal from ZKsync Lite?

You can find fully verified withdrawals on [Etherscan](https://etherscan.io/) in the "**Internal Transactions**" tab\*. You will have a transaction from the [`ZKsync` contract](https://etherscan.io/address/0xabea9132b05a70803a4e85094fd0e1800777fbef#tokentxns).

\* If you withdrew a token other than ETH then you would find the transaction in the "**Token Transfers(ERC-20)**" tab.
{% endtab %}
{% endtabs %}

## Can I Send Funds to or From a Centralized Exchange to ZKsync?

{% tabs %}
{% tab title="ZKsync Era" %}
#### Can I Send Funds to or From a Centralized Exchange to ZKsync Era?

No, you cannot send funds to or from a Centralized Exchange (CEX) until the network is supported by the exchange. To prevent loss of funds, please check with the specific exchange for their policies and support before sending funds to or from ZKsync Era to a CEX.

Until there is more CEX support for ZKsync Era you can use some third-party bridges to deposit funds from a CEX to ZKsync. See our [Ecosystem page](https://ecosystem.zksync.io/) for a list of bridges.
{% endtab %}

{% tab title="ZKsync Lite" %}
#### Can I Send Funds to or From a Centralized Exchange to ZKsync Lite?

Yes, you can send funds to and from a Centralized Exchange (CEX) to ZKsync as long as the CEX supports the ZKsync network. However, always ensure to check with the specific exchange for their policies and support. Some third-party bridges allow you to deposit funds from a CEX to ZKsync. See our [Ecosystem page](https://ecosystem.zksync.io/) for a list of bridges.
{% endtab %}
{% endtabs %}

## What is the Account Activation Fee on ZKsync Lite?

The account activation fee is a one-time fee to register your account with ZKsync. This fee only applies to your first ZKsync transaction on ZKsync Lite and **does not apply to ZKsync Era**.

On a deeper level, to be better suited for zero-knowledge proofs, ZKsync accounts are defined over a different elliptic curve than Ethereum's. Activating your account generates and publishes a new private-public key pair over this curve associated with your Ethereum address.

The registration process happens directly on the Ethereum smart contract and therefore it is an L1 transaction, so the activation fee is to pay the Ethereum miners and not ZKsync validators.

ERC-1271 compatible wallets (like Argent) increase this one-time fee because of higher interaction with the ZKsync smart contract. This operation is cheaper if you are using a CREATE2 smart-contract-based wallet.

## What Do the Statuses Mean for a Transaction?

{% tabs %}
{% tab title="ZKsync Era" %}
#### What Do the Statuses Mean for a Transaction on ZKsync Era?

* **`Indexing`** - In the mempool but not yet included in a block.
* **`Failed`** - Unverified/failed transaction.
* **`ZKsync Era Processed, Ethereum Sending`** - Included in a block but the batch containing the block has not yet been committed.
* **`ZKsync Era Processed, Ethereum Validating`** - Included in a block and committed on the Ethereum L1 network.
* **`ZKsync Era Processed, Ethereum Executing`** - Included in a block and proven on the Ethereum L1 network.
* **`ZKsync Era Processed, Ethereum Executed`** - Included in a block and executed on the Ethereum L1 network.
{% endtab %}

{% tab title="ZKsync Lite" %}
#### What Do the Statuses Mean for a Transaction on ZKsync Lite?

* **`Initiated`**: the ZKsync server has received and processed the transaction. Unless it is a withdrawal, it is ready for immediate use.
* **`Committed`**: the transaction appears in a block that is committed to the L1 smart contract.
* **`Verified`**: the transaction’s block has been proven and verified on the L1 smart contract.
{% endtab %}
{% endtabs %}

## How Long Does a Deposit Take?

A deposit to ZKsync is a transaction from Ethereum to ZKsync, and it typically takes about 5 minutes or about 10 block confirmations on Ethereum L1. The time can vary based on the congestion of the Ethereum network and the L1 gas fee set for the transaction.

## Is There a Token for ZKsync?

Yes, [https://docs.zknation.io/zk-token/zk-token](https://docs.zknation.io/zk-token/zk-token)

## Can I Run a Validator or a Node for ZKsync?

{% tabs %}
{% tab title="ZKsync Era" %}
#### Can I Run a Validator or a Node for ZKsync Era?

Not at the moment, but the network is expected to move towards a more decentralized model, allowing users to run their own validators or nodes in the future.
{% endtab %}

{% tab title="ZKsync Lite" %}
#### Can I Run a Validator or a Node for ZKsync Lite?

No
{% endtab %}
{% endtabs %}

## Is There a List of Projects in the ZKsync Ecosystem?

Yes, [https://ecosystem.zksync.io/](https://ecosystem.zksync.io/)

## Why Don't I See My Funds on My Wallet?

{% tabs %}
{% tab title="ZKsync Era" %}
#### Why Don't I See My Funds on My Wallet for ZKsync Era?

For ZKsync Era make sure you are connected to the ZKsync Era mainnet. If you still don't see your funds, you might need to change display settings to either show or add custom tokens on your wallet interface. You can check MetaMask's ["How to display tokens in MetaMask"](https://support.metamask.io/hc/en-us/articles/360015489031-How-to-display-tokens-in-MetaMask) for more details.
{% endtab %}

{% tab title="ZKsync Lite" %}
#### Why Don't I See My Funds on My Wallet for ZKsync Lite?

You will not see your ZKsync Lite funds on your wallet unless it is integrated with ZKsync Lite like [Argent](https://www.argent.xyz/).\
\
Since you connect to ZKsync Lite via Ethereum mainnet your wallet will show you your funds on Ethereum and you can check your ZKsync Lite funds on [the ZKsync Lite wallet](https://lite.zksync.io/) or [the ZKsync Lite block explorer](https://zkscan.io/).
{% endtab %}
{% endtabs %}
