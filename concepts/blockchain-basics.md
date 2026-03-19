# Blockchain Basics

## What Is a Blockchain?

A blockchain is a public digital ledger — think of it as a shared notebook that records every transaction, and once something is written, it can't be erased. Thousands of computers around the world maintain copies of this notebook, so no single person or company controls it.

## Key Concepts

### Address
Your wallet address is like a bank account number. It's a long string of characters (letters and numbers) that uniquely identifies your wallet on a specific blockchain. You share it with others so they can send you crypto.

Each blockchain has its own address format:
- **TON**: starts with `UQ` or `EQ` (or `0:` in raw format)
- **TRON**: starts with `T`
- **Solana**: a base58-encoded string

### Transaction
A transaction is a transfer of value from one address to another. When you send crypto, you create a transaction that gets recorded on the blockchain. Once confirmed, it's permanent and irreversible.

### Block
Transactions are grouped into "blocks" and added to the chain one at a time. Each block references the previous one — that's what makes it a chain. When your transaction is included in a block, it's "confirmed."

### Network Fee (Gas)
Every transaction requires a small fee paid to the network. This fee compensates the computers (validators) that process and confirm transactions. Fees vary by blockchain and network congestion.

## Why Multiple Blockchains?

Different blockchains have different strengths:
- **TON**: Very fast, low fees, designed by the team behind Telegram
- **TRON**: Popular for USDT transfers, relatively low fees
- **Solana**: Very fast, very low fees, popular for DeFi and NFTs

The same token (like USDT) can exist on multiple blockchains, but they're separate — you can't send USDT from one chain directly to an address on another chain without a cross-chain swap.

## Irreversibility

Unlike bank transfers, blockchain transactions **cannot be reversed**. There's no customer support to call, no chargebacks. Once you confirm a send, the tokens are gone. This is why it's crucial to double-check addresses and amounts before confirming.
