# Token Swaps Explained

## What Is a Swap?

A swap is exchanging one cryptocurrency for another. Instead of selling your token on an exchange and buying another, you can swap directly within the wallet.

## DEX vs CEX

### DEX (Decentralized Exchange)
A DEX is a smart contract on the blockchain that lets people trade tokens directly with each other — no middleman. When you swap tokens on the same chain (e.g., TON → USDT on TON), the trade happens through a DEX.

**Pros**: No registration, no KYC, your funds never leave your wallet
**Cons**: Only works within the same blockchain, prices depend on available liquidity

### CEX (Centralized Exchange)
A CEX is a company that holds funds and matches buyers with sellers (like Binance or Coinbase). MyTonWallet uses Changelly for cross-chain swaps — when you swap between different blockchains (e.g., TON → TRX).

**Pros**: Can swap between any supported chains
**Cons**: May require minimum amounts, takes longer, involves a third party

## Slippage

When you submit a swap, the price can change between the moment you click "Swap" and the moment the transaction executes. This difference is called **slippage**.

You set a **slippage tolerance** (default 5%) which means:
- If the price moves less than 5%, the swap executes.
- If it moves more than 5%, the swap fails and your tokens are returned.

Lower tolerance = you get a price closer to what you expected, but the swap may fail more often.

## Price Impact

If you're swapping a large amount relative to the available liquidity, your trade itself moves the price. This is **price impact**. The app shows it before you confirm.

- Small trades: negligible impact
- Large trades: can significantly worsen your rate

## Fees in Swaps

A swap typically involves:
- **Network fee** — paid to the blockchain (in native tokens)
- **DEX fee** — a percentage taken by the decentralized exchange (usually 0.1-0.3%)
- **Our fee** — a small service fee (shown on the confirmation screen)

All fees are displayed before you confirm.
