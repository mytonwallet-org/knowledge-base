# Privacy Features

## Hiding Sensitive Data

When you're in a public place or sharing your screen, you can hide your balance from the Home screen.

## Clipboard Safety

On mobile, when you copy an address or other sensitive data:
- The clipboard content **expires** after a short period (180 seconds).
- The data is marked as **local-only** — it won't sync to other devices via cloud clipboard services.

## What Data Stays on Your Device

- Recovery phrase and private keys — encrypted, never sent anywhere
- Password/PIN — stored locally, used only to decrypt keys
- Transaction history — cached locally for display
- Token balances — cached locally

## What Data Is Sent to Servers

- Your **public address** — to fetch balances, transactions, and NFTs (this is public information on the blockchain anyway)
- **Token prices** — fetched from price APIs
- **Push notification tokens** — if you enable push notifications, your device token and account address are sent to our server

## Non-Custodial

MyTonWallet never has access to your private keys or recovery phrase. We cannot:
- Access your funds
- Make transactions on your behalf
- Recover your wallet if you lose your phrase
- Freeze or block your account
