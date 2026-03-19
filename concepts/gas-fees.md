# Network Fees (Gas) Explained

## Why Do Fees Exist?

Every blockchain transaction needs to be processed and confirmed by the network. Fees compensate the validators (computers) that do this work, and they prevent spam — without fees, anyone could flood the network with millions of transactions.

## How Fees Work

When you send crypto, a small fee is deducted and paid to the network. You always pay the fee in the blockchain's **native token**:
- TON transactions → fee paid in **TON**
- TRON transactions → fee paid in **TRX** (or energy/bandwidth)
- Solana transactions → fee paid in **SOL**

This means you need some native tokens even if you only want to send other tokens (like USDT).

## Fee Amounts by Chain

### TON
- Very low — typically fractions of a TON
- Consistent and predictable
- Almost negligible for most users

### TRON
- Uses an **energy/bandwidth** model
- Simple TRX transfers: very cheap
- TRC-20 token transfers (like USDT): more expensive because they require "energy"
- If you don't have enough energy, extra TRX is burned to cover the cost

### Solana
- Extremely low — fractions of a cent
- Plus a one-time "rent" when creating a new token account (when you receive a token type for the first time)

## When Are Fees Charged?

Fees are charged for any on-chain action:
- Sending tokens
- Swapping tokens
- Staking / unstaking
- Minting or transferring NFTs
- Interacting with dApps

The app shows the estimated fee **before you confirm** every transaction. The actual fee may vary slightly from the estimate.

## "Insufficient Balance for Fee"

This common error means you don't have enough of the native token to pay the transaction fee. For example, if you want to send all your USDT on TON, you still need a small amount of TON for the fee. Solution: keep a small native token balance at all times.
