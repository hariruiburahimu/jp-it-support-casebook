# 🧾 Ticket 008 - USB Device Not Recognized / USBデバイスが認識されない

**Date:** 2025-07-18  
**User:** kobayashi.a  
**Department:** Design  
**Device:** Windows 11 Desktop  
**Location:** Osaka Branch – 1st Floor  

---

## 🛠️ Problem Description / 問題の説明

**EN:**  
User plugs in a USB device (flash drive) and receives the error:  
**"USB device not recognized. The last USB device you connected to this computer malfunctioned."**

**JP:**  
ユーザーがUSBフラッシュメモリを接続すると、  
「USBデバイスが認識されません。接続した最後のUSBデバイスが正常に動作しませんでした。」というエラーが表示されます。

---

## 🔍 Troubleshooting Steps / トラブルシューティング手順

1. Plugged the USB device into another port → Same error  
2. Tried USB device on another PC → Worked normally  
3. Checked Device Manager → Unknown USB Device with yellow triangle  
4. Right-clicked → Uninstalled device  
5. Disconnected USB device → Rebooted PC  
6. Plugged USB back in → Device installed and recognized  

**EN Result:**  
Faulty cached driver removed. USB device now works normally.

**JP 結果:**  
破損したドライバーキャッシュを削除し、USBデバイスは正常に認識されました。

---

## 📸 Screenshot

- [ ] Screenshot of Device Manager with error before fix  
  *(save as `usb_not_recognized.png` in `/screenshots/`)*

---

## ✅ Resolution Summary / 解決の要約

**EN:**  
Problem caused by corrupted cached USB driver. Resolved by uninstalling device and rebooting.

**JP:**  
破損したUSBドライバーが原因でした。デバイスをアンインストールし、再起動することで解決しました。

---

## 🗂️ Tags  
`#USB` `#DeviceManager` `#DriverIssue` `#Windows11`
