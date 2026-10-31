# PairOnce

**PairOnce — browser-to-browser file transfer between your devices. No app, no account, files never stored on a server.**

[paironce.com](https://paironce.com) · free · 13 languages · Windows, Mac, Linux, ChromeOS, Android, iPhone, iPad

PairOnce is a free web app for sending files, photos, text and links between your own devices, for example from an
iPhone to a Windows PC or from an Android phone to a Mac, without installing an app or creating an account. It works
like AirDrop across brands and across networks: the two browsers connect directly and end-to-end encrypted, and when a
network blocks a direct connection, an encrypted relay passes the data on without being able to read it. PairOnce keeps
no copy of what you send.

## What people use it for

- [Send photos from an iPhone to a Windows PC](https://paironce.com/guides/iphone-to-pc) at full quality, with no app
  and no cable
- [Move files from an Android phone to a Mac](https://paironce.com/guides/android-to-mac) or
  [to a Windows PC](https://paironce.com/guides/android-to-pc) without a USB cable
- [Send files when the phone and the computer are on different Wi-Fi](https://paironce.com/guides/phone-pc-different-wifi)
  or on mobile data
- [Get files onto a work computer where you cannot install software](https://paironce.com/guides/work-computer-no-install)
- [Copy on the phone and paste on the computer](https://paironce.com/guides/copy-paste-phone-to-pc), and the other way
- [Scan a paper document with the phone and receive the PDF on the computer](https://paironce.com/guides/scan-document-phone-to-computer)
- See the phone's camera on the computer and take a full-resolution photo from there (live picture)
- Hand the same files to a whole class or meeting on one Wi-Fi (distribution room: 10 devices, 30 with Pro)

## How it works

1. Open [paironce.com](https://paironce.com) on both devices.
2. Scan the QR code, or type the six-digit code.
3. Check that both screens show the same safety code, and approve.
4. Send. Next time, paired devices reconnect with one tap.

## Key facts

| | |
| --- | --- |
| Price | Free, no ads. Optional [PairOnce Pro](https://paironce.com/pro): US$3.99 a month or US$29.99 a year |
| Install | Nothing to install. It runs in Chrome, Edge and Safari and can be added to the home screen |
| Account | None |
| File size | Up to 2 GB per file over a direct connection when the receiving browser saves straight to disk (Chrome, Edge), up to 10 GB when one of the two devices has Pro; otherwise 50 MB per file |
| Across networks | Yes. Direct when possible, otherwise through an encrypted relay: 200 MB a month per device free, 5 GB with Pro |
| Encryption | End to end: AES-256-GCM, keys from the two devices' P-256 (ECDH) keys, a 13-digit safety code to compare on both screens |
| Stored on PairOnce servers | No files, no file names, no messages. The servers see addresses, timing and amounts of data ([data notice](https://paironce.com/realtime-beta-data-notice)) |
| Languages | English, Deutsch, Español, Français, हिन्दी, Bahasa Indonesia, Italiano, 日本語, 한국어, Português, 简体中文, 繁體中文 |
| Open source | The encryption, pairing and transfer code and the protocol (below); the web app and its services are not |

## When something else fits better

- **The receiver is offline, or the file should stay available later, or it goes to many people over weeks:** a cloud
  drive. PairOnce needs both devices online at the same time and keeps no copy
  ([which one fits](https://paironce.com/guides/direct-transfer-or-cloud-drive)).
- **Two Apple devices next to each other:** AirDrop is already there and needs no browser.
- **Very large files often over the relay:** the free relay allowance is 200 MB a month per device; on the same Wi-Fi
  there is no such limit.

## Questions

**Is PairOnce free?** Yes. Sending, receiving, pairing and saving devices are free with no ads. Pro adds relay data,
10 GB files and higher limits in the tools.

**Can PairOnce see my files?** No. Files and messages are encrypted in the sending browser and decrypted only in the
receiving one; the relay, when used, passes on data it cannot read.

**Does it work when the devices are not on the same Wi-Fi?** Yes. The devices connect directly over the internet when the
networks allow it, and through the encrypted relay when they do not.

**Do I need to install anything?** No. Open the website on both devices. Adding it to the home screen is optional.

**Is PairOnce open source?** The part that decides whether your files stay private is: the encryption and pairing code
and the protocol, so the privacy claims can be checked rather than believed.

## Open source

The same version that paironce.com runs ([release record](https://github.com/paironce/security/blob/main/RELEASES.md)):

| Repository | What | License |
| --- | --- | --- |
| [protocol](https://github.com/paironce/protocol) | How pairing, key exchange, the safety code and transfers work; the threat model | CC BY 4.0 |
| [core](https://github.com/paironce/core) | `@paironce/core`: frame encryption, pairing cryptography, file-transfer framing | Apache-2.0 |
| [locales](https://github.com/paironce/locales) | The interface in 13 languages: translation fixes welcome | Apache-2.0 |
| [security](https://github.com/paironce/security) | How to report a vulnerability; every production release and the core version it runs | CC BY 4.0 |

Questions, ideas and problem reports: [paironce/community discussions](https://github.com/paironce/community/discussions).

## More guides

[All guides](https://paironce.com/guides/), one question per page with the limits stated plainly, for example
[an AirDrop alternative for Windows, Android and iPhone](https://paironce.com/guides/airdrop-alternative),
[iPhone photos to a computer without losing quality](https://paironce.com/guides/iphone-photos-to-computer-original) and
[sending photos and videos without compression](https://paironce.com/guides/send-photos-without-compression).

## Security and contact

Found a vulnerability? Email support@paironce.com with a subject starting "SECURITY"; see
[SECURITY.md](https://github.com/paironce/security/blob/main/SECURITY.md). Questions and feedback are welcome at the same
address.

PairOnce™ and the PairOnce logo are not covered by the open-source licenses; a fork needs its own name.
