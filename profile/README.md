# PairOnce

**PairOnce — browser-to-browser file transfer between your devices. No app, no account, files never stored on a server.**

[paironce.com](https://paironce.com) · 13 languages

Pair two devices once: scan a QR code or type a six-digit code, and compare the safety code on both screens. After that
they reconnect with one tap. Files, text and links go straight from one browser to the other, end-to-end encrypted; when a
network blocks a direct connection, an encrypted relay passes the data on without being able to read it.

## At a glance

| | |
| --- | --- |
| Install | Nothing to install: it runs in Chrome, Edge and Safari, and can be added to the home screen |
| Account | None |
| File size | Up to 2 GB per file when the receiving browser saves straight to disk (Chrome, Edge), or 10 GB with PairOnce Pro on one of the two devices; otherwise 50 MB per file |
| Across networks | Yes: direct when possible, otherwise through a relay (200 MB per device each month free) |
| Encryption | End to end: AES-256-GCM with keys from the two devices' ECDH keys; a 13-digit safety code to compare |
| Stored on our servers | Nothing: no files, no file names, no messages |
| Price | Free, no ads; optional [Pro](https://paironce.com/pro) for 5 GB of relay a month |

## Guides

[All guides](https://paironce.com/guides/) — for example
[sending iPhone photos to a computer without compression](https://paironce.com/guides/iphone-photos-to-computer-original),
[a work computer where you cannot install apps](https://paironce.com/guides/work-computer-no-install), and
[phone and computer on different Wi-Fi](https://paironce.com/guides/phone-pc-different-wifi).

## Open source

The part that decides whether your files stay private is open, so it can be checked rather than believed
(version 2.1.0, the same code paironce.com runs):

| Repository | What | License |
| --- | --- | --- |
| [protocol](https://github.com/paironce/protocol) | How pairing, key exchange, the safety code and transfers work; the threat model | CC BY 4.0 |
| [core](https://github.com/paironce/core) | `@paironce/core`: frame encryption, pairing cryptography, file-transfer framing | Apache-2.0 |
| [locales](https://github.com/paironce/locales) | The interface in 13 languages: translation fixes welcome | Apache-2.0 |
| [security](https://github.com/paironce/security) | How to report a vulnerability; every production release and the core version it runs | CC BY 4.0 |

The web app, the signaling service and the relay are not open source.

## Security and contact

Found a vulnerability? Email support@paironce.com with a subject starting "SECURITY". Questions and feedback are welcome
at the same address.

PairOnce™ and the PairOnce logo are not covered by the open-source licenses; a fork needs its own name.
