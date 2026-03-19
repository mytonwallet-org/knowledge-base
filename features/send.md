# Sending Crypto

## Basic Send

1. From the Home tab, tap **Send**.
2. Enter the **recipient address** — paste it, scan a **QR code**, or use a supported domain name.
3. Select the **token** you want to send.
4. Enter the amount.
5. Review the fee and confirmation details.
6. Confirm with your password, PIN, biometric, or hardware wallet if required.

The transaction appears in your Activity feed after submission. On TON, incoming and outgoing updates can appear almost immediately, though final blockchain confirmation can still take a little longer.

## Ways To Enter The Recipient

You can send using:

- A raw wallet address
- A scanned QR code
- A TON DNS domain such as `alice.ton`
- Other supported linked names such as `.t.me`, `.vip`, or `.gram`
- A saved address from your address book

If a linked domain or address looks suspicious, the app can show a warning before you continue.

## Amount Entry

You can enter the amount directly in crypto or use **fiat-denominated input** to type a value in your base currency and let the app convert it for you.

## Comments And Encrypted Messages

When sending on TON, you can attach a **comment** to the transaction. This is visible on-chain to anyone.

On TON, you can also use **encrypted comments** so that only the sender and recipient can read the message.

## Fees

Every blockchain charges a network fee:

- **TON**: typically very low
- **TRON**: depends on TRX, energy, and bandwidth rules
- **Solana**: very low fixed fees, plus possible rent for new token accounts

The app shows estimated fees before confirmation. In most cases, you pay the fee in the chain's native token. Some TON token transfers can use gasless mode instead. See `features/gasless.md`.

## Sending The Full Balance

On some chains, you can send your entire native-token balance and let the fee be deducted from the sent amount. The app shows a notice when that is possible.

## Multi-Send

`Multisend` lets you send multiple transfers in one action.

Ways to access it include:

- Open the Send flow and choose **Multi-Send**
- Long-press **Send** on mobile
- Right-click **Send** on desktop

It supports:

- Multiple recipients
- Different amounts
- Optional comments
- CSV upload

`Multisend` supports up to `255` transfers for `W5` wallets. Older wallet versions are limited to `4`.

## Instant Transfer Links

After sending, the app can generate a shareable transfer link right away, even before final confirmation. This is useful when you need to show that a payment was already initiated.

## Common Issues

- **Insufficient balance**: you may need more of the chain's native token, unless gasless sending is available
- **Invalid address**: make sure the address format matches the chain
- **Wrong chain**: sending to the wrong network can permanently lose funds
- **Transaction stuck or pending**: see `troubleshooting/transactions.md`
