# Swapping Tokens

## How Swaps Work

Swapping lets you exchange one token for another directly in the wallet.

1. Tap **Swap**
2. Choose the token you are swapping from
3. Choose the token you want to receive
4. Enter the amount
5. Review the route, rate, fees, and price impact
6. Confirm

The wallet compares available routes and tries to show the best option automatically.

## On-Chain Swaps

For assets on the same blockchain, the app routes through integrated DEX liquidity. The swap aggregator:

- Compares routes across multiple DEXes
- Marks the strongest route with a **Best Rate** badge
- Lets you inspect alternative routes
- Separates exchange rate and fee information more clearly
- Uses broader routing and multi-path routing to reduce slippage

Some swap flows have included a `0.875%` service fee.

## Cross-Chain Swaps

For swaps between different chains, the wallet uses integrated exchange providers. This includes:

- Automatic swaps between supported chains like TON, TRON, and Solana
- Swaps to or from external chains such as BTC or ETH, where you provide an external wallet address or send funds to a deposit address

These swaps take longer than same-chain swaps.

## Solana Support

The multichain swap experience also includes cross-chain swaps between Solana and the wallet's other supported chains.

## Slippage

Slippage is the difference between the quoted rate and the executed rate.

- Lower slippage means tighter protection but a higher chance of failure
- Higher slippage means more tolerance for price movement
- Large or illiquid trades can have higher price impact

## Fees

Swap costs can include:

- **Network fee**
- **DEX or route fee**
- **Exchange-provider fee** for cross-chain or external-chain swaps
- **Price impact**

The confirmation screen also shows clearer fee and change breakdowns.

## Common Issues

- **Insufficient balance for fee**: you need enough of the native token unless the flow explicitly supports another fee model
- **Price moved too much**: the swap may fail if the market moves outside your slippage tolerance
- **Minimum amount not met**: common in cross-chain swaps
- **Wrong external address**: external-chain swaps depend on the destination address being correct
