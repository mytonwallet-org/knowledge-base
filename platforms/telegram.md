# Telegram Mini App

MyTonWallet is available as a Telegram Mini App — you can open it directly inside Telegram without installing a separate app.

## How to Open

Search for the MyTonWallet bot in Telegram (or use a direct link) and launch the Mini App from the bot's menu.

## Features

Most core features are available:
- Send, receive, swap tokens
- View balances and activity
- Stake TON
- Browse and connect to dApps
- Manage NFTs
- Buy/sell crypto

The Mini App is designed as a quick-access wallet inside Telegram and supports faster transaction actions such as copying addresses, saving addresses, and opening items in a blockchain explorer.

## dApps

dApps connect directly through the Telegram Mini App environment. TON Connect is supported.

The broader Telegram ecosystem also includes `@push`, which is a separate Telegram bot and Mini App flow for chat-native transfers. See `features/push.md`.

## Limitations

The Telegram Mini App platform has inherent constraints:

- **No Ledger support** — hardware wallets cannot connect through Telegram
- **No deep links** — `ton://` and similar schemes are not handled
- **No push notifications** — Telegram handles its own notification system
- **No biometric unlock** — security depends on your Telegram app's own lock
- **Limited screen size** — the Mini App runs inside Telegram's webview, which may be smaller than a full-screen app

## When to Use

The Telegram Mini App is convenient for quick operations when you're already in Telegram. For full functionality and the best experience, use the native mobile app or desktop app.

## Help Center

The app also includes a Help Center entry point from Settings, alongside the public help site at `https://help.mytonwallet.io/`.

## Security Notes

- Your wallet keys are encrypted and stored within the Mini App's storage, separate from Telegram's own data.
- The Mini App runs in an isolated webview — Telegram cannot access your keys.
- For maximum security, consider using the native app for large transactions.
