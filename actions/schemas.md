# Action Deeplinks

When the user wants to perform an action, you can return a **deeplink** that the client app displays as a tappable button below your message. The deeplink triggers the appropriate screen or operation with pre-filled parameters.

Use the `mtw://` protocol for all deeplinks.

Format deeplinks as a Markdown link. The client renders them as buttons:

```
[Button Label](mtw://command?param=value)
```

Always confirm details with the user before returning a transaction deeplink.

---

## Available Deeplinks

### Send (Multi-Chain)

**Preferred for all send actions.** Supports any chain. But use Transfer deeplink for ton chain

```
mtw://send/<chain>:<address>?amount=<smallest_units>&text=<comment>&token=<slug>
```

Parameters:
- `<chain>` — blockchain identifier: `ton`, `tron`, or `solana` (required in URL path)
- `<address>` — recipient address or DNS domain (required in URL path)
- `amount` — amount in **smallest units** (nanotons for TON, sun for TRON, lamports for Solana)
- `text` — comment/memo (optional)
- `token` — token slug, to send a specific token instead of the chain's native coin (optional)
- `bin` — binary payload in base64 (mutually exclusive with `text`)
- `init` / `stateInit` — state init for TON (optional)
- `exp` — expiry timestamp in seconds (optional)

If `token` is omitted, the chain's native token is used (TON, TRX, or SOL).

Examples:
- `[Send 10 TON to alice.ton](mtw://send/ton:alice.ton?amount=10000000000)`
- `[Send TON](mtw://send/ton:alice.ton)` — opens with address pre-filled, user enters amount
- `[Send USDT on TON](mtw://send/ton:EQ...?token=ton-usdt&amount=1000000)` — send a token on TON
- `[Send USDT on TRON](mtw://send/tron:T...?token=tron-usdt&amount=1000000)` — send USDT on TRON
- `[Send SOL](mtw://send/solana:...?amount=1000000000)` — send SOL

### Transfer (TON only, legacy)

Still supported, but prefer `send` for new actions. Only works for TON chain.

```
mtw://transfer/<address>?amount=<nanotons>&text=<comment>
```

Parameters:
- `<address>` — TON recipient address or DNS domain (required in URL path)
- `amount` — amount in **nanotons** (1 TON = 1,000,000,000 nanotons)
- `text` — comment/memo (optional)
- `jetton` — jetton minter address, to send a specific token instead of TON (optional)
- `nft` — NFT address, to send an NFT (optional)
- `bin` — binary payload in base64 (mutually exclusive with `text`)

### Swap

```
mtw://swap?in=<tokenSlug>&out=<tokenSlug>&amountIn=<number>
```

Parameters (all optional):
- `in` — token slug to swap from (default: `toncoin`)
- `out` — token slug to swap to
- `amountIn` — amount of the input token (as a regular number, not nanotons)

Examples:
- `[Swap 100 TON to USDT](mtw://swap?in=toncoin&out=ton-usdt&amount=100)`
- `[Open Swap](mtw://swap)` — opens swap screen with defaults

### Buy with Crypto

```
mtw://buy-with-crypto?in=<tokenSlug>&out=<tokenSlug>&amount=<number>
```

Similar to swap but pre-selects buy-oriented token pairs.

### Buy with Card

```
mtw://buy-with-card
```

Opens the Moonpay on-ramp widget.

### Stake

```
mtw://stake
```

Opens the staking screen.

### Receive

```
mtw://receive
```

Opens the receive screen with address and QR code.

### Explore (dApps)

```
mtw://explore
mtw://explore/<hostname>
```

Opens the Explore tab. If a hostname is provided, opens that specific dApp.

Example:
- `[Open Getgems](mtw://explore/getgems.io)`

### View Token

```
mtw://token/<slug>
mtw://token/<chain>/<tokenAddress>
```

Opens the token detail screen (price chart + activity).

Examples:
- `[View TON](mtw://token/toncoin)`
- `[View Token](mtw://token/ton/EQ...)`

### View Transaction

```
mtw://tx/<chain>/<txId>
```

Opens a specific transaction's detail view.

### View NFT

```
mtw://nft/<nftAddress>
```

Opens an NFT detail view.

---

## Common Token Slugs

Use these in `token` parameter for send deeplinks and `in`/`out` for swap deeplinks:

| Slug | Token |
|------|-------|
| `toncoin` | TON |
| `ton-usdt` | USDT on TON |
| `tron` | TRX |
| `tron-usdt` | USDT on TRON |
| `sol` | SOL |
| `sol-usdt` | USDT on Solana |

---

## Rules for Returning Deeplinks

1. **Always confirm with the user first.** Never return a transfer deeplink without the user explicitly agreeing to the destination and amount.
2. **Pre-fill what you know, leave the rest.** If the user says "send some TON to alice.ton" without specifying an amount, return the deeplink without the `amount` parameter — the app lets them fill it in.
3. **One deeplink per message.** Don't return multiple action deeplinks in a single response.
4. **Validate before returning.** If an address looks wrong or a token isn't supported, tell the user instead of returning a broken deeplink.
5. **Deeplinks open screens, not execute transactions.** The app shows the pre-filled screen — the user still reviews and confirms manually. No deeplink sends funds directly.
6. **Use smallest units for amounts in send deeplinks.** 1 TON = 1,000,000,000 nanotons; 1 TRX = 1,000,000 sun; 1 SOL = 1,000,000,000 lamports. For swap amounts, use regular numbers.
7. **Use clear button labels.** The label should describe the action: "Send 10 TON to alice.ton", "Open Swap", "View Staking".
