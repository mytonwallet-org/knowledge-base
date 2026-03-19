# Creating a New Wallet

## Steps

1. Open MyTonWallet and tap **Create Wallet**.
2. The app generates a **24-word recovery phrase** (also called a "seed phrase" or "secret words").
3. Write down all 24 words **on paper**, in order. Do not screenshot or copy to clipboard.
4. The app asks you to verify a few words to confirm you saved them correctly.
5. Set a **password** (or 4-digit **PIN** on mobile) to protect daily access.
6. Optionally enable **biometric unlock** (Face ID, Touch ID, fingerprint).

Your wallet is now ready. You'll have addresses for TON, TRON, and Solana automatically.

## About the Recovery Phrase

- It is the **master key** to your wallet. Anyone with these words can access all your funds across all chains.
- MyTonWallet is **non-custodial** — we do not store your phrase. If you lose it, nobody can help you recover it.
- Never enter your recovery phrase on any website or share it with anyone. MyTonWallet will never ask for it except during wallet import.
- Store it in a safe, offline location. Consider multiple copies in different physical locations.

## What Happens Technically

When you create a wallet, the app derives private keys for each supported blockchain from your recovery phrase using standard cryptographic algorithms (BIP-39). The phrase and keys are encrypted with your password and stored locally on your device. They never leave your device.

## After Creation

- Your wallet starts with zero balance on all chains.
- To add funds, go to Receive to get your address, or use Buy to purchase crypto with a card.
- Consider completing the security setup (Settings → Security): enable biometrics and set an auto-lock timeout.

## Onboarding Experience

The onboarding flow includes:

- More guided backup and verification steps
- Security alerts during setup
- Faster onboarding screens

If your app looks different from an older guide, the main process is still the same: create wallet, secure the recovery phrase, verify it, and protect the app with a password or PIN.
