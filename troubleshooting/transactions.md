# Transaction Troubleshooting

## Transaction Is "Pending" for a Long Time

Transactions typically confirm within seconds (TON) to a few minutes (TRON, Solana). If it stays pending:

- **TON**: Almost always confirms quickly. If stuck, the network may be congested — wait a few minutes.
- **TRON**: Can take longer if the network is busy. Wait up to 5-10 minutes.
- **Solana**: Usually fast. If pending, the transaction may have been dropped — check your activity for an updated status.

If a transaction has been pending for over 15 minutes, it likely failed silently. Check a blockchain explorer for the transaction hash (tap the transaction in your activity to find it).

## Transaction Failed

Common reasons:
- **Insufficient balance for fee** — you need the native token (TON/TRX/SOL) to cover the network fee, even when sending other tokens.
- **Insufficient energy/bandwidth (TRON)** — TRC-20 transfers require energy. If you don't have enough, the fee is paid in TRX. Make sure you have enough TRX.
- **Slippage exceeded (swaps)** — the price moved beyond your slippage tolerance. Try again or increase slippage.
- **Smart contract error** — the receiving contract rejected the transaction. This can happen with dApp interactions.

## Sent to the Wrong Address

Blockchain transactions are **irreversible**. If you sent to the wrong address:
- If you know the recipient, contact them to request a return.
- If you sent to a non-existent or uncontrolled address, the funds are lost.
- If you sent on the wrong chain (e.g., sent to a TRON address on TON), the funds are lost.

**Always double-check the address and chain before confirming.**

## Transaction Not Showing in Activity

- Refresh the Home tab (pull down to refresh on mobile).
- The transaction may not have been broadcast. Check if your balance changed.
- If you made the transaction on another device/wallet, it may take a moment to sync.

## Fee Was Higher Than Expected

Network fees vary based on:
- **Network congestion** at the time of the transaction
- **Transaction complexity** (token transfers cost more than native transfers on TRON)
- **Token account creation** (Solana charges rent for new token accounts)

The fee shown during confirmation is an estimate. The actual fee may differ slightly.
