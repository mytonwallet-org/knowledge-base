# Exploring dApps

## What Are dApps?

Decentralized applications are blockchain apps such as DEXes, games, NFT marketplaces, and utilities. Your wallet connects so the dApp can read your public address and request approvals.

## The Explore Tab

The **Explore** tab is the main discovery area for dApps. Categories include:

- Games
- Entertainment
- DeFi
- NFTs
- Utilities

Explore also surfaces connected dApps and quick access to recent services.

## Opening dApps

### On Mobile

dApps open in the built-in browser. The browser can be minimized into a small pill and reopened later.

### On Desktop, Web, And Extension

dApps usually open in your normal browser and connect through the wallet integration available on that platform.

## Connection Protocols

- **TON Connect** for TON dApps
- **WalletConnect** or similar flows for supported multichain dApps

MyTonWallet supports smoother TON Connect behavior and multi-device dApp sessions.

## Connecting Your Wallet

When a dApp requests a connection:

1. The wallet shows the dApp name and the request
2. You choose which account to connect
3. You approve or reject

The dApp can request actions, but it cannot access your private keys.

## Approving Transactions

When a connected dApp requests a transaction, the wallet shows a preview with the requested action and estimated fees. This preview is useful, but it is not an absolute guarantee:

- Some information comes from wallet-side checks and emulation
- Some preview content may come from the dApp itself
- Untrusted dApps can forge informational preview text

Always verify the recipient, asset, amount, and fee before approving.

## Managing Connected dApps

In `Settings → dApps`, you can:

- Review connected dApps
- Disconnect any dApp
- Check last activity

Explore also shows shortcuts for connected dApps.

## Data Signing

MyTonWallet also supports **signing data in dApps** through TON Connect, including messages, files, smart-contract payloads, and other structured requests.

## Safety Tips

- Only connect to dApps you trust
- Reject unexpected requests
- Treat dApp-provided descriptions as helpful, not authoritative
- Disconnect services you no longer use
