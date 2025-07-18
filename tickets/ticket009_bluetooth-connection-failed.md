# 🧾 Ticket 009 - Bluetooth Device Not Connecting / Bluetoothデバイスが接続できない

**Date:** 2025-07-18  
**User:** fujimoto.h  
**Department:** Planning  
**Device:** Windows 11 Laptop  
**Location:** Yokohama Office – 3rd Floor  

---

## 🛠️ Problem Description / 問題の説明

**EN:**  
User is trying to connect a Bluetooth keyboard, but the device fails to pair.  
Error: **"Couldn't connect. Try again."**

**JP:**  
ユーザーがBluetoothキーボードを接続しようとすると、「接続できませんでした。もう一度お試しください。」というエラーが表示されます。

---

## 🔍 Troubleshooting Steps / トラブルシューティング手順

1. Ensured Bluetooth was enabled in **Settings → Devices → Bluetooth & devices**  
2. Verified airplane mode was **off**  
3. Restarted Bluetooth Support Service (`services.msc`)  
4. Removed previously paired version of the device  
5. Restarted PC  
6. Repaired device from scratch → Successfully connected  

**EN Result:**  
Repaired Bluetooth connection by resetting service and removing previous pairings.

**JP 結果:**  
Bluetoothサービスの再起動とペアリング履歴の削除により、デバイスが正常に接続できるようになりました。

---

## 📸 Screenshot

- [ ] Screenshot of **Bluetooth settings screen** or **pairing error**  
  *(save as `bluetooth_connection_issue.png` in `/screenshots/`)*

---

## ✅ Resolution Summary / 解決の要約

**EN:**  
Bluetooth device failed to pair due to cached connection. Resolved by resetting service and re-pairing.

**JP:**  
Bluetoothデバイスがペアリングキャッシュの影響で接続できませんでした。サービスを再起動し、再ペアリングすることで解決しました。

---

## 🗂️ Tags  
`#Bluetooth` `#PairingIssue` `#Windows11` `#Services` `#WirelessDevices`
