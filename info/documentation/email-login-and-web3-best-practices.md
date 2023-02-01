---
description: Login with Email
---

# Email Login and Web3 Best Practices

New to Web3? Don't have an Ethereum wallet? No problem! You can log into Coordinape with any email address, and our partners at MagicLink will create a wallet for you behind the scenes. Here's what you need to know about that...

## How it works

* When you log in via email, MagicLink creates a free Ethereum wallet for you and associates it with your email address.
* When authenticated via your email, you can control the wallet through MagicLink's API.
* You can use your MagicLink wallet to perform actions in Coordinape, such as sending GIVE, allowing you to use most functions in the app and even recieve tokens from your DAO.
* You cannot use your MagicLink wallet to manage CoVaults.  If you are a Coordinape Admin, it might make sense to use Metamask instead.
* You can also use the MagicLink wallet and interface for other dApps in web3.
* In the future, you can export your wallet's private key (like a password) to use with a more standard, browser based-application like Metamask.
* Taking this step means you are now the sole owner of your wallet's private key, and it will be a more flexible and secure way to manage your tokens.&#x20;

## What is a wallet?

A wallet is a piece of software that holds the private keys (or seed phrase) for your address and makes it simple for you to interact with a blockchain.&#x20;

* Private Keys are the 12 to 24 words that you use to prove your ownership of an Ethereum address.

There are a ton of great wallets out there and most of them will let you use the same passkey to access the funds held in your address.

There are 4 ways to log into Coordinape:

* [Metamask ](https://metamask.io)(A browser extension you can download) or a wallet that can emulate MM like [0xFrame](https://frame.sh)
* [Coinbase Wallet](https://www.coinbase.com/wallet) (A browser extension you can download)
* [Wallet Connect](https://walletconnect.com) (A QR code that you can scan with a wallet on your phone)
  * This supports a ton of cool wallets like [Argent ](https://www.argent.xyz)and [Rainbow](https://rainbow.me)
* Email Login (MagicLink creates a wallet for you and holds your private keys, allowing you to log in and manage it with your email address)&#x20;

For more information on wallets click [here](https://ethereum.org/en/wallets/)

<details>

<summary>Wallets Recommeded by Coordinape</summary>

#### [0xFrame](https://frame.sh)

Feature rich software wallet that lives on your local machine and can emulate Metamask when signing transactions.

➕ Does a great job of displaying what your signing

➕ Compatible with all EVM Chains

➕ Excellent hardware wallet support

➖ Not natively supported everwhere

#### [Argent](https://www.argent.xyz)

A mobile wallet that doesn't require you to know your private keys and supports Social Recovery if you forget your password

➕ Never been hacked

➕ All Transactions must be approved by guardians (3 factor Authentication)

➖ Only compatible with ETH, and ZKsynchas

➖ Can be more expensive to perform transactions due to additional security of the guardians

#### [Coinbase Wallet](https://www.coinbase.com/wallet)

Mobile wallet and Browser Extension that supports EVM chains and additional chains

➕ Built in browser

➕ Integration with Coinbase&#x20;

➖ Not as widely supported as Metamask

#### [MetaMask](https://metamask.io)

Mobile wallet and browser extension that supports all EVM chains, this is the standard wallet for Crypto.

➕ Built in browser

➖ UX&#x20;

Even More wallets can be found here [https://ethereum.org/en/wallets/find-wallet/](https://ethereum.org/en/wallets/find-wallet/)

</details>

## Taking full ownership of your wallet

* MagicLink provides a wallet, and an option to export your private key so you can decide to manage it on your own.
* This feature requires some provisioning from Coordinape, which we will be adding in coming months.

## Best practices for Wallets

{% hint style="warning" %}
Never under any circumstances share your private key with someone. If they have this key they can take everything in your wallet.

\
There are no refunds in web3
{% endhint %}

The current web3/crypto landscape looks different than the web that you may be used to. There are a number of reasons for this.&#x20;

One of those reasons is users own their assets, not a bank, or Google, or Amazon, or Microsoft. This means that users need to take an abundance of caution when interacting with apps.&#x20;

Anything that you'll want to do in web3 will involve you connecting to an app and giving it permission to connect to your wallet before doing a transaction.&#x20;

This will require you to "sign" things with your wallet.&#x20;

\`To do those transactions you'll typically need to do 3 signatures: (Pop ups that will prompt you to approve something)&#x20;

1. Sign to allow the app to connect to your wallet ⛽🚫
2. Sign to approve the app to spend your assets ⛽
3. Sign to approve that app to complete the transaction. ⛽

`⛽ = Transaction requires gas`

`⛽🚫 = Signature only`

{% hint style="info" %}
Some wallets will give you an option to set the "gas" fee and the "tip" for each transaction. You should only change these if you have an idea of what your doing, but in general a lower gas fee means you will wait longer to have the transaction confirmed, and a higher one means it will go through faster.&#x20;
{% endhint %}

If you want to see a transactions progress before it's finalized every transaction creates a "Hash" that can be looked up on [Etherscan](https://etherscan.io). (Or it's equivalent if your on another chain) Etherscan can tell you all about your transaction, but you'll need to have a pretty good understanding of the code to make much sense of it

It's important not to blindly sign any popup that comes up on your web3 journey. Only sign transactions from sites that you trust. [0xFrame ](https://frame.sh)does an excellent job of letting you read what you're signing.&#x20;

You are the master of your own fate in web3. It can be scary, but it's worth it. If you have any questions we're always happy to answer them in our discord... Just don't give us your private keys.

## What's special about web3?

Web3 (or Crypto) is a version of the internet with a focus on decentralization and user ownership.&#x20;

To appreciate this ownership focus you should [give this a look](https://ethereum.org/en/web3/), but if you want a super short TLDR of what web1 and web2 are you can check this out below.

* Web1 - Read Only
  * The early internet, mostly static sites run by businesses.
* Web2 - Read/Write
  * Social media and advertisement driven user flows, the users attention is usually what companies are selling.
* Web3 - Read/Write/Own
  * Decentralized, permissionless, native payments, and trustless. Users can now own their data, payments methods, and not be forced to choose between tech giants for the services they rely on.&#x20;

{% hint style="info" %}
_Most of the Web3 tools and apps exist on a spectrum of the highlights above, some apps are fully on chain with IPFS hosted front ends, and others only interact with the blockchain for payments. As the infrastructure for truly decentralized apps is built out the ideal outcome is more decentralization to return to the initial promise of the early internet where people could freely exchange ideas, values, and data._


{% endhint %}

To put a cherry on top of this the teams building in web3/crypto today are doing so because they've caught a glimpse of the future.&#x20;

* A future where a teen living in Somalia can make the same investments as an Elizabeth Warren.
* A future where a woman in Iran can design an amazing website and get paid for their work regardless of her gender, or location
* A future where a whistleblower can post uncensorable articles about their repressive government without fear of their data being deleted.&#x20;
* A future where a refugee can protect their hard earned money from being stolen by a corrupt government.

If those things sound valuable, you're in the right place, if they don't, give it time.
