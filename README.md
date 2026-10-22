# Obol Wallet downloads

Public preview installers for the optional Obol Wallet companion.

[Download the current preview](https://github.com/tameioncs-acc/Obol-Wallet-Downloads/releases/tag/v0.1.0-preview.20261022)

# Obol Wallet companion preview · 2026-10-22

An installable visual preview of the optional Obol Wallet desktop companion.
This build uses sample balances and activity. Live account sign-in, inference,
payments, verified earning, automatic tool configuration and updates are not
connected. Installing it does not create an account or grant credits.

| Platform | Download |
| --- | --- |
| Windows x64 | `Obol-Wallet-0.1.0-preview-windows-x64.exe` |
| macOS, Apple Silicon and Intel | `Obol-Wallet-0.1.0-preview-macos-universal.dmg` |
| Linux x64 | `Obol-Wallet-0.1.0-preview-linux-x64.AppImage` |
| Debian-compatible Linux x64 | `Obol-Wallet-0.1.0-preview-linux-x64.deb` |

Windows has no publisher signature. The macOS app is ad-hoc signed, without
Developer ID signing or notarization. Your operating system may block these
preview builds. They are not a signed production release. Linux requires the
GTK/WebKitGTK runtime dependencies declared by the Debian package; AppImage
compatibility depends on the distribution.

All three native packaging jobs passed. The universal macOS app passed signature
verification and has recorded launch evidence. Windows and Linux runtime
validation remains limited. The native app's internal version is `0.1.0`.

Source revision: `6d88d281e0a60909159eeb426f4bfb66bd940c91`.
GitHub Actions build: `39718529040` (2026-10-22). These are the existing successful
CI artifacts, not binaries rebuilt from subsequent working-tree changes.

`SHA256SUMS.txt` records the hash of each installer; `release.json` records its
size, platform and source revision. Verify the downloaded bytes before use:

```sh
# macOS
shasum -a 256 Obol-Wallet-0.1.0-preview-macos-universal.dmg
# Linux
sha256sum Obol-Wallet-0.1.0-preview-linux-x64.AppImage
```

```powershell
# Windows PowerShell
Get-FileHash .\Obol-Wallet-0.1.0-preview-windows-x64.exe -Algorithm SHA256
```

Compare the result with the matching entry in `SHA256SUMS.txt`. The desktop
companion is optional; Wallet's web-first product direction is unchanged.
