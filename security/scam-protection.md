# Scam Protection

## Built-In Protections

### Scam Address Detection
MyTonWallet maintains a database of known scam addresses. When you enter a recipient address that matches a flagged address, the app shows a **warning**. You can still proceed, but you should carefully verify the address.

### Domain Similarity Warnings
When interacting with TON DNS domains, the app warns you about **lookalike domains** — names that are visually similar to well-known domains but are controlled by scammers (e.g., using letter substitution).

### Suspicious Action Alerts
The app can warn you about potentially dangerous actions. You can toggle this in Settings → Security → Allow Suspicious Actions.

### Anti-Poisoning Labels

MyTonWallet includes built-in **anti-poisoning** protection that marks lookalike or scam-history addresses with a visible **Scam** label in transaction history.

### Import And Send Warnings

MyTonWallet shows warnings for:

- Suspicious multisig wallet imports
- Suspicious `.ton` destinations before sending

## Common Scams to Watch For

### Fake Airdrops
You receive unexpected tokens or NFTs with instructions to visit a website. **Never** visit links from unexpected airdrops — they typically try to steal your recovery phrase.

### Phishing Sites
Websites that look like MyTonWallet or popular dApps, asking for your recovery phrase. **MyTonWallet will never ask for your recovery phrase** except during wallet import, and only in the app itself.

### Address Poisoning
Scammers send tiny transactions from addresses that look similar to your real contacts, hoping you'll copy the wrong address from your history. Always verify the full address, not just the first and last characters.

### Fake dApp Previews
Some dApps can show misleading descriptions or forged preview text. Even if a wallet preview looks familiar, verify the real recipient, asset, and amount before approving.

### Too-Good-To-Be-True Offers
Any dApp or service promising guaranteed returns, free tokens for connecting your wallet, or other unrealistic offers is almost certainly a scam.

## What to Do If You Suspect a Scam

- **Do not** approve any transactions.
- **Disconnect** the dApp (Settings → dApps).
- If you shared your recovery phrase: **immediately create a new wallet** and transfer all funds to it.
- If you approved a suspicious transaction: check your activity for unexpected outgoing transfers.
