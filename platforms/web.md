# Web App

The web version runs in any modern browser at the official MyTonWallet URL.

## Features

All core features are available: send, receive, swap, stake, explore dApps, manage NFTs, and more.

## Biometrics

WebAuthn-based biometric unlock is available on devices that support it (e.g., Touch ID on MacBooks, Windows Hello). Enable in Settings → Security.

## Ledger

Connects via **WebHID**. Requires a Chromium-based browser (Chrome, Edge, Brave). Not supported in Firefox or Safari.

## dApps

dApps open in a new browser tab. They connect to your wallet if you have the MyTonWallet browser extension installed, or via QR code / link.

There is no in-app browser on web — dApps run in their own tabs.

## Limitations

- No push notifications (browser notifications may be available but are less reliable than native)
- No deep link handling
- No home screen widgets
- Session depends on browser storage — clearing browser data may require re-importing your wallet

## Security Notes

- Keys are encrypted and stored in browser localStorage
- Use a private/dedicated browser profile for extra security
- Be cautious of browser extensions that could access page content
- Always verify you're on the official URL
