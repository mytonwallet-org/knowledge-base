# Missing Tokens Troubleshooting

## Token Balance Shows Zero

- **Refresh** — pull down to refresh on mobile, or reload on web.
- **Correct chain?** — check that you're looking at the right blockchain. USDT exists on TON, TRON, and Solana separately. Your balance on one chain doesn't appear on another.
- **Correct account?** — if you have multiple accounts, make sure you're viewing the right one.
- **Token hidden?** — you or the app may have hidden the token. Go to Settings → Tokens → Hidden Tokens to check.
- **Tiny balance hidden?** — very small balances may be hidden. Enable "Show Tiny Transfers" in Settings → Tokens.

## Token Not Listed

If a token doesn't appear in your list at all:
- It may not be in the default token list. **Import it manually** by contract address: Settings → Tokens → Import Token. See `tokens/import-hide.md`.
- If you recently received the token, wait a moment for the balance to sync.

## Sent Tokens But They Didn't Arrive

- **Check the transaction status** in your activity feed. Is it confirmed or still pending?
- **Correct address and chain?** — tokens sent on the wrong chain are lost.
- **Recipient using the right wallet?** — the recipient needs a wallet that supports the token's chain.
- Use a **blockchain explorer** to verify: look up the transaction hash to see if it was confirmed on-chain.

## NFTs Not Showing

- NFTs may take a moment to load after a transfer.
- Check if the NFT's collection is hidden (Settings → NFTs or Hidden Collections).
- Telegram Gifts are auto-collected — they should appear automatically.
- Try refreshing the Assets section.

## Balance Doesn't Match Explorer

- The app caches balances and refreshes periodically. Pull down to force a refresh.
- Some tokens use non-standard display decimals. The raw on-chain balance may look different from the displayed amount.
- If the discrepancy persists after refreshing, it may be a temporary API issue.
