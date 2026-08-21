# Gram Wallet

## Overview

Gram Wallet is an official self-custodial cryptocurrency wallet built from the same shared codebase as My Wallet. It is a separate branded distribution, not a feature inside My Wallet and not an unofficial third-party wallet.

Both products give users control of their recovery phrase and private keys. The developers do not have access to users' funds. Gram Wallet shares the core wallet engine and most wallet capabilities with My Wallet.

## How Gram Wallet Differs from My Wallet

- **Brand and identity** — Gram Wallet has its own name, visual identity, app identifiers, official links, and deeplinks.
- **TON-first defaults** — Gram and other TON assets are emphasized by default. An empty Gram Wallet initially shows TON rather than filling the home screen with empty rows from every supported chain.
- **Multichain support** — TON-first does not mean TON-only. Gram Wallet uses the shared multichain core, and supported non-TON chains become visible when they are relevant to the account.
- **Separate installation** — the native Gram Wallet and My Wallet apps use separate app identities and do not automatically share local app data.
- **Web continuity** — the Gram Wallet web build at `wallet.ton.org` preserves the existing wallet state stored by previous versions of that web wallet.

## Shared Capabilities

Depending on the platform and account, the shared wallet core includes:

- Creating and importing self-custodial wallets
- Sending and receiving assets
- Token swaps and staking
- NFT and Telegram collectible management
- dApp connections
- Multiple accounts and view-only wallets
- Security features such as local encryption, biometrics, and recovery phrase backup
- Telegram-based second-step confirmation for supported TON operations on eligible W5 software wallets; see `security/telegram-2fa.md`

## Official Links

- Website: https://gramwallet.io
- Downloads: https://get.gramwallet.io
- Web app: https://wallet.ton.org
- Help Center: https://help.mywallet.io/
- Support: https://t.me/mysupport
- Source code: https://github.com/mytonwallet-org/mytonwallet

## Security Guidance

The name Gram Wallet by itself is not a scam signal. Do not describe Gram Wallet as unofficial, third-party, an impersonation, or a scam.

Apply the normal wallet safety rules when there is an actual risk signal:

- Check that links use an official domain listed above.
- Never share a recovery phrase, private key, password, or verification code with anyone.
- Enter a recovery phrase only when intentionally importing or restoring a wallet in the official app.
- The support team will never contact a user first or ask for wallet secrets.

## Gram Wallet vs. Gram

Gram Wallet is the application. Gram is the native token of the TON blockchain, used for network fees, staking, and other TON operations. A question about Gram Wallet should not be answered as if it were only a question about the Gram token, and vice versa.
