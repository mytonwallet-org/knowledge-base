# Security Setup

## Password

Required during wallet creation or import. Used to encrypt your keys on-device and to confirm sensitive operations (sending, exporting keys, connecting dApps).

- Must be set during initial setup.
- Can be changed later in Settings → Security → Change Password.
- If forgotten, you must re-import your wallet using the recovery phrase.

## PIN

On mobile, you can use a PIN instead of typing a full password for daily operations.

- Set during wallet creation or in Settings → Security
- Used for quick unlock and confirmations
- Your full password still protects the underlying encryption

## Biometric Unlock

Available on all platforms where the device supports it:
- **Mobile**: Face ID, Touch ID, fingerprint
- **Desktop (macOS)**: Touch ID
- **Web / Extension**: WebAuthn (if your device supports it)

Enable in Settings → Security → Biometric Unlock.

Biometrics provide a convenience layer — they unlock access to your encrypted password, which in turn decrypts your keys.

## Auto-Lock

The app locks automatically after inactivity. Configure the timeout in `Settings → Security → Auto-Lock`.

Auto-lock includes:

- Locking after inactivity
- A default `10 minute` lock
- Configurable timeout options

When locked, the app requires your password, PIN, or biometric to unlock.

## Remember Passcode

**Remember Passcode** mode keeps repeated confirmations unlocked for a short time, such as `5 minutes`, especially when biometrics are off.

## Password Recovery Safety

If you forget the password, you usually need to re-import the wallet with the recovery phrase. The lock screen also offers an option to **log out of all wallets** after a failed unlock attempt, which helps you reset access safely without keeping old encrypted wallets on the device.

## Recommendations

- Use the manual lock option if you want to lock the app immediately without waiting for auto-lock.
- Enable biometric unlock for convenience without compromising security.
- Set auto-lock to 10 minutes or less, especially on shared or mobile devices.
- Use a strong, unique password that you don't use elsewhere.
- Back up your recovery phrase before doing anything else (Settings → Security → Back Up Secret Words).
