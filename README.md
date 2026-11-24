# Sapherbox downloads

Installers of the Sapherbox desktop clients. This repository holds released
files only; it contains no source code.

| Client | Platform | Download |
|---|---|---|
| Sapherbox Sync | Windows | [SapherboxSync-windows-installer.exe](https://github.com/jetned/sapherbox-downloads/releases/download/sync-latest/SapherboxSync-windows-installer.exe) |
| Sapherbox Sync | macOS | [SapherboxSync-macOS.zip](https://github.com/jetned/sapherbox-downloads/releases/download/sync-latest/SapherboxSync-macOS.zip) |
| Sapherbox Sync | Linux (Debian/Ubuntu, amd64) | [SapherboxSync-linux-amd64.deb](https://github.com/jetned/sapherbox-downloads/releases/download/sync-latest/SapherboxSync-linux-amd64.deb) |
| Sapherbox for Mac | macOS | [Sapherbox-macOS.dmg](https://github.com/jetned/sapherbox-downloads/releases/download/macos-latest/Sapherbox-macOS.dmg) |

The same files are linked from the Clients page of every Sapherbox
(Preferences → Clients) and from `https://www.sapherbox.com/download/…`.

## How this repository works

- Each client has one rolling release (`sync-latest`, `macos-latest`). It is
  replaced with every new version, and the file names stay the same, so the
  links above always deliver the newest version. The release title names the
  version.
- Each release carries a checksum file (`SHA256SUMS-sync.txt`,
  `SHA256SUMS-macos.txt`). To check a download:
  `sha256sum -c SHA256SUMS-sync.txt --ignore-missing` (macOS: `shasum -a 256 -c`).
- The files are published by the release pipelines of the clients.

## Help

Sapherbox help center: https://support.sapherbox.com/help
