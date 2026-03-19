# Ledger Hardware Wallet

## What Is a Hardware Wallet?

A Ledger is a physical device that stores your private keys offline. Transactions are signed on the device itself — your keys never touch your phone or computer. This provides the highest level of security.

## Supported Platforms

| Platform | Connection |
|----------|-----------|
| Mobile (iOS/Android) | Bluetooth or USB, depending on platform support |
| Web | WebHID (browser must support it) |
| Browser Extension | USB |
| Desktop (Electron) | HID / USB |
| Telegram Mini App | Not supported |

## Setting Up Ledger

1. Install the **TON app** on your Ledger device (via Ledger Live).
2. Open MyTonWallet and go to **Settings → Hardware Wallet** (or choose Ledger during wallet import).
3. Connect:
   - **Mobile**: Use Bluetooth or USB, depending on platform support.
   - **Desktop/Extension**: Plug in your Ledger via USB.
   - **Web**: Your browser prompts for WebHID device access.
4. Select which wallet(s) to import from the Ledger.
5. The wallet appears in your account list.

## Using Ledger

When you need to sign a transaction (send, swap, stake, approve dApp):
1. The app prepares the transaction and shows you a preview.
2. You confirm in the app.
3. The transaction details appear on your **Ledger screen** — verify them.
4. **Physically approve** on the Ledger device by pressing the buttons.

If the details on your Ledger screen don't match what the app shows, **reject** the transaction.

## Limitations

- Ledger wallets are **TON-only** in MyTonWallet (no TRON or Solana via Ledger at this time).
- You cannot export the private key from a Ledger — that's by design.
- The Ledger must be connected and unlocked with the TON app open whenever you need to sign.

## Troubleshooting

- **Device not found**: Make sure Bluetooth is enabled on mobile, or try a different USB port or cable where USB is supported. Ensure the TON app is open on the Ledger.
- **Transaction rejected**: Verify the Ledger firmware and TON app are up to date via Ledger Live.
- **Browser won't connect (Web)**: WebHID requires a Chromium-based browser (Chrome, Edge, Brave). Firefox and Safari are not supported.
