# Mobile (iOS & Android)

The native mobile apps are the primary platform for MyTonWallet, used by the majority of users.

## Navigation

Core mobile navigation is centered around:

- **Home** for balances, tokens, activity, and main actions
- **Explore** for dApps and wallet-explorer tools
- **Settings** for account management and security

Mobile navigation includes:

- A bottom tab bar for Wallet, Explore, and Settings
- Quick account switching by long-pressing **Settings**
- Swipe-based wallet switching in Air

## In-App Browser

dApps open inside the wallet in an embedded browser. You can:
- **Minimize** — swipe down to collapse into a small pill at the bottom
- **Expand** — tap the pill to return to the dApp
- **Close** — fully exit the browser session

The browser supports TON Connect for TON dApps. dApps cannot access your keys — they request transactions that you approve individually.

## Biometrics

- **iOS**: Face ID, Touch ID
- **Android**: Fingerprint, Face Unlock (device-dependent)

Enable in Settings → Security → Biometric Unlock.

## Push Notifications

Native push notifications can alert you about incoming transactions and other wallet activity.

- Enable them in `Settings → Notifications`
- Notifications can be enabled for up to `3` wallets
- On Android, battery optimization can interfere with background delivery

## QR Code Scanner

Available when entering addresses (Send, dApp URLs, etc.). Tap the QR icon to open the camera scanner.

## Widgets

MyTonWallet supports several widget types on mobile:

- Home-screen widgets
- Token-price widgets
- Quick-action widgets such as add, send, swap, or earn
- iOS Lock Screen widgets that open token views in the app

## Ledger Connection

Mobile Ledger support includes Bluetooth and USB, depending on the platform. Make sure:

- The Ledger has the TON app open
- Bluetooth or USB access is available
- The devices are ready to pair

## Switching Between Air and Classic

The mobile app includes two interfaces: **Air** (native) and **Classic** (web-based). You can switch freely — your wallets and data carry over automatically.

- **Classic → Air**: Go to **Settings → Appearance** and tap the **MyTonWallet Air** toggle, or open the deep link `mtw://air`.
- **Air → Classic**: Go to **Settings → Appearance** and tap **Switch to Legacy Version**, or open the deep link `mtw://classic`.

See `platforms/air.md` for more details.

## Deep Links

The app handles `ton://`, `tc://`, `mtw://` URL schemes. Tapping a compatible link anywhere on your device opens it in MyTonWallet.

Notable `mtw://` deep links:
- `mtw://air` — Switch to Air interface
- `mtw://classic` — Switch to Classic interface

## Storage

- Encrypted keys stored in the device's secure storage (iOS Keychain / Android Encrypted SharedPreferences)
- App data stored locally — not backed up to iCloud or Google Drive

## iPad

MyTonWallet also includes a dedicated iPad-optimized layout with larger-screen navigation and settings improvements.
