# Gasless (Diesel) Transactions

## What Are Gasless Transactions?

Normally, you need the chain's native token (TON) to pay network fees — even when sending other tokens like USDT. Gasless transactions let you **pay the fee in the token you're sending** instead, so you don't need to hold any TON at all.

## How It Works

When you send a token on TON (like USDT) and your wallet supports gasless mode, the app automatically checks if a gasless transaction is available. If it is, the fee is deducted from the token amount you're sending rather than from your TON balance.

This is powered by the **W5 wallet version** — the latest TON wallet contract that supports sponsored transactions. If your wallet uses an older version, you can upgrade to W5 in Settings → Wallet Version.

## When Is It Available?

Gasless transactions are available when:
- Your wallet uses the **W5** contract version
- You're sending a supported token (like USDT on TON)
- The gasless service is online and has capacity

The app detects availability automatically and shows the fee in the token you're sending on the confirmation screen. If gasless is unavailable, the fee falls back to TON as usual.

Gasless or mintless TON token transfers activate automatically when your TON balance falls below `0.3 TON`.

## Why Use It?

- **Convenience** — no need to keep a TON balance just for fees
- **Simpler onboarding** — new users who receive USDT can send it immediately without first acquiring TON
- The fee amount is comparable to a regular TON fee, just paid in a different token
