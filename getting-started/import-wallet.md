# Importing an Existing Wallet

You can import a wallet you created elsewhere or restore a wallet from a backup.

## Import Methods

### Recovery Phrase (Mnemonic)
1. Tap **Import Wallet** on the start screen (or go to Settings → Add Account → Import).
2. Enter your 12 or 24 words in order.
3. Set a password or PIN.
4. The app derives your addresses for all supported chains (TON, TRON, Solana).

Both standard BIP-39 mnemonics and TON-specific 24-word mnemonics are supported. The app detects the format automatically.

Import includes easier flows such as one-click seed-phrase pasting and more guided verification.

### Private Key
1. Choose **Import from Private Key**.
2. Paste your private key.
3. Set a password or PIN.

This imports a single-chain wallet. The chain is detected from the key format.

### Ledger Hardware Wallet
1. Choose **Connect Ledger**.
2. On mobile, use Bluetooth or USB depending on platform support.
3. On desktop, connect via USB.
4. On web, the app uses WebHID — your browser may prompt for device access.
5. Select which wallet(s) to import from the Ledger.

Ledger wallets are view-and-sign only — the private key stays on the hardware device.

### View-Only (Watch) Account
1. Choose **Add Account** → **Watch Account**.
2. Enter any wallet address.
3. You can view balances and activity but cannot send or sign transactions.

Useful for monitoring addresses you don't control.

## After Import

- Balances and transaction history load automatically.
- If you imported via mnemonic, you have full access to all chains.
- You can add more accounts later from Settings without losing the current one.
