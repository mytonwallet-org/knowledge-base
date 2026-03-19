# Wallets Explained

## What Is a Crypto Wallet?

A crypto wallet doesn't actually "store" your crypto — your tokens live on the blockchain. A wallet stores your **private keys**, which are like the passwords that let you access and send your tokens. Whoever has the private key controls the funds.

## Recovery Phrase (Seed Phrase)

When you create a wallet, you get a **recovery phrase** — a list of 12 or 24 ordinary words (like "apple" "river" "sunset"...) in a specific order. This phrase is a human-readable representation of your master private key.

From this single phrase, the wallet derives private keys for all supported blockchains. That's why one recovery phrase gives you addresses on TON, TRON, and Solana.

**Critical rules:**
- Write it on paper, never digitally
- Never share it with anyone
- Never enter it on any website
- If someone has your phrase, they have your funds
- If you lose your phrase and your device, your funds are gone forever

## Custodial vs Non-Custodial

### Custodial Wallet
A company holds your private keys for you (like a bank holding your money). Convenient, but you depend on them — they could get hacked, freeze your account, or go out of business.

### Non-Custodial Wallet (MyTonWallet)
**You** hold your private keys. Nobody else — not even MyTonWallet — can access your funds. You have full control, but you're also fully responsible for keeping your recovery phrase safe.

## What Happens When You "Create a Wallet"?

1. The app generates a random recovery phrase (24 words).
2. From the phrase, it derives private keys for each blockchain.
3. From each private key, it derives your public address.
4. The phrase and keys are encrypted with your password and stored on your device.

Your addresses are now "live" on the blockchain — anyone can send tokens to them. The private key lets you send tokens from them.

## Multiple Wallets / Accounts

You can have multiple wallets in one app. Each has its own recovery phrase (or private key) and its own set of addresses. Useful for separating funds or purposes.
