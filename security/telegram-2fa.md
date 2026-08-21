# 2FA with Telegram

## What It Is

Gram Wallet supports Telegram-based two-factor confirmation for eligible TON wallets. It adds a second approval step to supported TON operations:

1. The user authorizes the operation in Gram Wallet with the wallet passcode or password.
2. The user reviews and confirms the pending operation in Telegram.
3. Only after the Telegram confirmation is the operation broadcast to TON.

This is transaction-level protection. It is not SMS or authenticator-app 2FA, it does not protect login or unlock of the app, and it is unrelated to Telegram's own Two-Step Verification setting.

2FA with Telegram applies only to supported operations involving TON assets. It does not add Telegram confirmation to operations on other blockchains.

## Requirements

New connections are made in Gram Wallet. The active account must:

- Be a software wallet created or imported from a recovery phrase
- Support TON
- Use the W5 TON wallet version
- Have at least `0.15 Gram` for the connection fee

Ledger and view-only accounts cannot connect Telegram 2FA. Availability is also controlled per account and platform during rollout, so the setting may not appear for every otherwise eligible account immediately.

2FA is configured separately for each eligible TON wallet. It is not a global setting shared by all accounts in the app.

## Connect Telegram

1. Select the TON wallet you want to protect.
2. Open **Settings → Security → 2FA with Telegram**.
3. Tap **Connect Telegram**.
4. Gram Wallet opens the official Telegram bot and Mini App. Review the Telegram account and TON wallet being linked, then confirm.
5. Return to Gram Wallet and confirm the connection with the wallet passcode or password.
6. Review and pay the displayed `0.15 Gram` connection fee. Wait for the connection to complete before leaving the flow.

The first connection requires the wallet passcode or password; do not tell users that biometrics alone are sufficient for this step.

## Confirm an Operation

When a supported TON operation requires 2FA:

1. Review and authorize it in Gram Wallet.
2. Open Telegram from the confirmation screen.
3. Verify the wallet, action, recipient, asset, amount, and fee shown in Telegram.
4. Confirm only if every detail is correct.
5. Return to Gram Wallet and wait for completion.

The TON operation remains pending and is not broadcast until the Telegram confirmation succeeds. Reject the request if its purpose or details are unclear.

## Unlink or Change the Telegram Account

To disable 2FA:

1. Open **Settings → Security → 2FA with Telegram**.
2. Tap **Unlink Account**.
3. Authorize the disconnection in Gram Wallet.
4. Confirm the removal in Telegram and wait for it to complete.

There is no direct account-switch action. To use a different Telegram account, unlink the current account, switch to the intended account in Telegram, and connect Telegram again from Gram Wallet.

## Troubleshooting

- **The 2FA setting is missing** — make sure the user is in Gram Wallet and has selected an eligible recovery-phrase TON wallet using W5. Update the app. If all requirements are met, the feature may not yet be enabled for that account or platform.
- **Unsupported Wallet Version** — Telegram 2FA requires W5. The version can be checked under **Settings → Wallet Version**. Changing the TON wallet version changes the TON address and requires moving assets, so the user should review `features/wallet-version.md` before upgrading.
- **Insufficient Balance** — add enough Gram to the selected TON wallet to cover the displayed `0.15 Gram` connection fee.
- **Telegram did not open or the connection is still pending** — return to the 2FA screen and tap **Open Telegram** or **Connect Telegram** again, complete the confirmation, then return to Gram Wallet.
- **The user lost access to the linked Telegram account** — do not invent a bypass. Removal normally requires Telegram confirmation. Direct the user to official support for the currently available recovery options.

## Security Guidance

Start the connection and every confirmation from inside Gram Wallet. The official flow opens `@tgmfabot`; never follow an unexpected confirmation link sent by another account.

Neither the Telegram bot nor support needs the recovery phrase, private key, wallet password, or passcode. Telegram 2FA is an additional protection layer, not a replacement for a secure recovery-phrase backup. If a recovery phrase or private key may be compromised, follow the compromised-wallet guidance instead of relying on 2FA alone.
