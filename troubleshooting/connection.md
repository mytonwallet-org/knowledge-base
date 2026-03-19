# Connection Troubleshooting

## App Won't Load or Sync

- Check your **internet connection**. The app needs internet to fetch balances and submit transactions.
- Try switching between Wi-Fi and mobile data.
- On mobile, check if the app has network permissions.
- Try closing and reopening the app.

## dApp Won't Connect

### On Mobile (In-App Browser)
- Make sure the dApp supports **TON Connect** (for TON dApps) or **WalletConnect** (for other chains).
- Try closing the in-app browser and reopening the dApp.
- Clear the in-app browser cache if available.

### On Browser Extension
- Make sure the extension is enabled and unlocked.
- Refresh the dApp page.
- Check that the dApp is looking for MyTonWallet (some dApps only support specific wallets).

### On Desktop / Web
- If connecting via QR code, make sure to scan it with MyTonWallet (not your phone camera).
- Check that the dApp and wallet are on the same network (mainnet vs testnet).

## dApp Shows "Disconnected"

dApp connections can expire. To reconnect:
1. Go to Settings → dApps.
2. Find the dApp and disconnect it.
3. Go back to the dApp and connect again.

## Balances Not Updating

- Pull down to refresh on mobile, or reload on web.
- Balances are fetched from the blockchain — if the network is slow, there may be a delay.
- If a specific token shows zero but you know you have it, the token's API endpoint may be temporarily unavailable.

## Push Notifications Not Working

- Check that notifications are enabled both in the app (Settings → Notifications) and in your device's system settings.
- Push notifications are limited to **3 accounts**. If you have more, only the selected accounts receive notifications.
- On Android, battery optimization can block background notifications — exclude MyTonWallet from battery optimization.
