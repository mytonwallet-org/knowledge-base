# `@push` in Telegram

## What It Is

`@push` is a Telegram bot and Mini App for sending TON-based assets inside Telegram chats without giving custody of your funds to a service. It supports:

- TON and Jettons
- TON NFTs
- On-chain Telegram Gifts
- Payment requests and invoices

The sender signs with a TON wallet through TON Connect. The transfer is then claimed by the recipient inside Telegram.

## Where It Works

`@push` can be used in:

- Private chats
- Group chats
- Channels

For channel transfers, the channel must have **Sign Messages** enabled. Some Telegram contexts may block sending, such as anonymous admin mode in discussion groups.

## What You Can Do

- Send crypto to a chat or a specific `@username`
- Request a payment instead of sending immediately
- Send TON NFTs and Telegram Gifts
- Enter amounts in fiat
- Use simple arithmetic like splitting a bill
- Add comments or emoji
- Mute status updates with `/mute`

## Basic Send Flow

1. In Telegram, start a message with `@push`.
2. Enter what you want to send, such as TON, a token amount, or a collectible command like `@push nft` or `@push gift`.
3. Connect a TON wallet when prompted.
4. Choose the asset and, if needed, the recipient.
5. Sign the transfer.

The bot posts the transfer in chat, and the recipient can claim it later.

## Receiving And Claiming

Recipients do not need to have a wallet at the moment the transfer is created.

- Funds or collectibles remain in a smart contract until claimed
- The recipient can claim by connecting a wallet
- Some collectible flows also allow forwarding to a wallet address instead of connecting in place

This makes `@push` useful for sending assets to people who are not yet crypto users.

## Gift And NFT Commands

- `@push gift` shows on-chain Telegram Gifts only
- `@push nft` shows TON NFTs available to send

You can send collectibles in private chats, groups, and channels. If a collectible is still unclaimed, the sender can cancel the transfer before the recipient claims it.

## Payment Requests

`@push` can also create payment requests instead of transfers. This is useful for collecting payments in a group or sending a direct request to a specific Telegram user.

## Wallet Compatibility

`@push` is designed to work with TON-compatible wallets through TON Connect, not just MyTonWallet.

## Important Notes

- `@push` is **non-custodial**: the service does not control your wallet keys
- Availability depends on Telegram chat context and wallet support
- Claims and notifications may take time to update because they depend on both Telegram and blockchain state
- If you need technical details about signatures, bindings, or security assumptions, see `security/push-technical.md`
