# Platform-Specific Issues

## iOS

### App Crashes on Launch
- Make sure you're on iOS 16 or later.
- Try force-quitting and reopening.
- If persistent, uninstall and reinstall (you'll need your recovery phrase to re-import).

### Face ID Not Working
- Check that Face ID is enabled for MyTonWallet in device Settings → Face ID & Passcode.
- Re-enable biometric unlock in the app: Settings → Security → Biometric Unlock.

### Push Notifications Not Arriving
- Check iOS Settings → Notifications → MyTonWallet is enabled.
- Check that Focus/Do Not Disturb isn't blocking notifications.

## Android

### App Not Receiving Notifications in Background
- Exclude MyTonWallet from **battery optimization** (Settings → Apps → MyTonWallet → Battery → Unrestricted).
- Different manufacturers have different battery management — search for your device brand + "allow background apps."

### WebView Issues
- The app uses an embedded WebView for its SDK layer. If something behaves unexpectedly, make sure **Android System WebView** is updated from the Play Store.

### Camera Not Working for QR Scan
- Check that camera permission is granted: device Settings → Apps → MyTonWallet → Permissions.

## Web

### Extension Not Detected by dApps
- Make sure the extension is **enabled** in your browser's extension settings.
- Some dApps require a page refresh after installing the extension.
- The extension must be **unlocked** (not in locked state) for dApps to detect it.

### WebHID Not Working (Ledger)
- WebHID requires a Chromium-based browser (Chrome, Edge, Brave). Not supported in Firefox or Safari.
- Try a different USB port or cable.

## Desktop (Electron)

### App Not Starting
- Try deleting the app cache and restarting.
- On macOS, check System Settings → Privacy & Security if the app is blocked.
- On Linux, some distributions may need additional GTK dependencies.

### Auto-Update Stuck
- Check your internet connection.
- You can always download the latest version manually from the official website.

## Telegram Mini App

### Limited Features
The Telegram Mini App does not support:
- Ledger hardware wallet
- Deep links
- Push notifications (Telegram handles its own notifications)

These limitations are inherent to the Telegram Mini App platform.
