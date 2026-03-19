# Browser Extension

Available for Chrome, Firefox, and Opera. The extension provides a popup wallet and enables dApp connections directly in your browser.

## Installation

Install from your browser's extension store:
- **Chrome**: Chrome Web Store
- **Firefox**: Firefox Add-ons
- **Opera**: Opera Add-ons

## Using the Extension

Click the MyTonWallet icon in your browser toolbar to open the wallet popup. All core features are available: send, receive, swap, stake, view NFTs, check activity.

## dApp Connection

The extension **injects** a wallet provider into web pages. When you visit a TON dApp:
1. The dApp detects MyTonWallet automatically.
2. It requests to connect — you see an approval popup.
3. Once connected, the dApp can request transactions which you approve individually.

For this to work:
- The extension must be **enabled** and **unlocked**.
- Some dApps require a page refresh after installing the extension.

## Biometrics

WebAuthn-based biometric unlock is available if your device supports it. Enable in Settings → Security.

## Ledger

Connects via **USB**. Plug in your Ledger, open the TON app on it, and the extension communicates directly.

## Limitations

- No in-app browser — dApps run in regular browser tabs
- No deep links
- No push notifications
- Extension popup has limited screen space — some features may feel compact

## Security Notes

- The extension stores encrypted keys in browser extension storage (separate from regular website storage).
- Pin the extension to your toolbar for quick access.
- Be cautious of phishing sites that mimic dApps — always check the URL.
