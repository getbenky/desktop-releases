# Benky for Mac

[Download for Apple Silicon](https://github.com/getbenky/desktop-releases/releases/latest/download/Benky-macOS-arm64.dmg) · [Release history](https://github.com/getbenky/desktop-releases/releases) · [Benky website](https://benky.space)

This repository contains desktop beta installers and checksums only. The development repository is private. A Benky account is required to use the app.

## Install

1. Download the DMG. It supports Apple Silicon Macs (M1 and newer), not Intel Macs.
2. Open it and drag Benky into Applications.
3. Open Benky from Applications.

**Unsigned beta:** builds have an ad-hoc signature, but are not Developer ID signed or Apple-notarized. If macOS blocks the first launch, attempt to open the app, then use System Settings → Privacy & Security → Open Anyway if you trust this download. [Apple installation guidance](https://support.apple.com/en-us/102445).

Updates are manual: download the newest release and replace the app in Applications. There is no automatic updater yet.

## Verify a download

Download the DMG and its `.sha256` file from the same release into one directory, then run:

```sh
shasum -a 256 -c Benky-macOS-arm64.dmg.sha256
```

The checksum detects an incomplete or changed download; it does not replace Developer ID signing or notarization.
