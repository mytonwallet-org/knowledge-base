# `@push` Technical Security Notes

## High-Level Model

`@push` is designed as a **non-custodial** Telegram transfer system:

- The sender signs with their wallet through TON Connect
- Funds are locked in a smart contract
- The backend coordinates messages and state updates
- The recipient proves eligibility with Telegram-signed data when claiming

The backend does **not** hold private keys and does not sign transactions on the user's behalf.

## How Claim Authorization Works

When a recipient claims a transfer, the system checks Telegram-signed data. Depending on how the sender created the transfer, the check can be bound to:

- A specific **chat instance**, so any eligible member of that chat can claim it
- A specific **Telegram username**, so only that username can claim it

This is how `@push` stays chat-native without asking the sender or recipient to trust a custodial service.

## Gas And Fees

The sender prepays the on-chain work needed for the transfer. The claim message itself carries no value, so the recipient does not need to pay gas just to receive the asset.

## Security Properties

- Private keys stay in the user's wallet
- Telegram signatures are checked before claim processing
- Stored bindings must match the signed username or chat instance
- Timestamp checks help prevent replay of stale Telegram signatures

## Trade-Offs And Limitations

- The design depends on Telegram signatures and Telegram account state
- Username-based transfers rely on whoever controls that username at claim time
- Chat-based transfers rely on the recipient still being eligible in that chat
- Operational status still depends on backend infrastructure for message orchestration and state polling

## What This Means For Users

- `@push` is safer than handing funds to a custodial bot
- It is still important to verify who you are sending to
- If you want strong recipient control, sending to a specific `@username` is more precise than sending to a whole chat
- For large transfers, use the same caution you would use with any blockchain payment
