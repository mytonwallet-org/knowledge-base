# Desktop App (Electron)

A standalone desktop application for Windows, macOS, and Linux.

## Installation

Download from the official MyTonWallet website. Available for:
- **macOS**: `.dmg` installer
- **Windows**: `.exe` installer
- **Linux**: `.AppImage` or `.deb`

## Features

All core features are available. The desktop app provides a wider screen layout optimized for larger displays.

The desktop app also supports:

- Right-click shortcuts in some desktop flows, such as access to `Multisend`
- Layout switching improvements for larger screens

## Biometrics

- **macOS**: Touch ID (on supported MacBooks)
- Other platforms: password/PIN only

## OS Keychain Integration

On desktop, sensitive secrets (like biometric-protected passwords) are stored in the operating system's secure storage:
- **macOS**: Keychain
- **Windows**: Credential Manager
- **Linux**: Secret Service / password store

This provides OS-level encryption independent of the app.

## Ledger

Connects via **USB** (HID). Plug in your Ledger and open the TON app.

## Deep Links

The desktop app registers as a handler for `ton://`, `tc://`, and `mtw://` URL schemes. Clicking these links in your browser opens them in the wallet.

## Auto-Updates

The app checks for updates automatically and notifies you when a new version is available. Updates are downloaded and installed with one click.

## dApps

dApps open in your regular browser. They connect via TON Connect (if the browser extension is also installed) or via QR code / link.

There is no in-app browser on desktop.

## Limitations

- No push notifications
- No home screen widgets

## Troubleshooting

- **macOS "unidentified developer" warning**: Right-click → Open, then click Open in the dialog.
- **Linux missing dependencies**: Some distributions may need GTK libraries.
- **Update stuck**: Download the latest version manually from the official website.
