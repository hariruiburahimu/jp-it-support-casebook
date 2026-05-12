# 🧾 Ticket 002 - Wi-Fi Connected But No Internet / Wi-Fiは接続されているがインターネットに接続できない

**Date:** 2025-07-18  
**User:** tanaka.k  
**Department:** Sales  
**Device:** Windows 11 Laptop  
**Location:** Osaka Branch – 2nd Floor  

---

## 🛠️ Problem Description / 問題の説明

**EN:**  
User reports that Wi-Fi is connected, but no websites open. Other employees can access the internet.

**JP:**  
ユーザーはWi-Fiに接続されているが、ウェブサイトが開けないと報告し、他の従業員端末は正常にインターネットを使用できています。

---

## 🔍 Troubleshooting Steps / トラブルシューティング手順

1. Checked Wi-Fi icon → No warning symbol  
2. Ran `ipconfig /all` → IP address assigned  
3. Pinged `192.168.1.1` → Success  
4. Pinged `8.8.8.8` → Success  
5. Pinged `www.google.com` → **Failed**  
6. Ran `ipconfig /flushdns`  
7. Ran `netsh winsock reset`  
8. Restarted laptop  
9. Tried again → Success  

**EN Result:**  
DNS cache caused resolution failure. Flushing DNS + Winsock reset resolved it.

**JP 結果:**  
DNSキャッシュが原因で名前解決に失敗していたため、DNSのフラッシュとWinsockのリセットで解決しました。

---

## 📸 Screenshot

- [ ] Add screenshot of command prompt running  
  `ipconfig /flushdns` and `netsh winsock reset`  
  *(save as `wifi_dns_reset.png` in `/screenshots/`)*

---

## ✅ Resolution Summary / 解決の要約

**EN:**  
Resolved by flushing DNS cache and resetting Winsock. Internet restored.

**JP:**  
DNSキャッシュをフラッシュし、Winsockをリセットすることで、インターネット接続が復旧しました。

---

## 🗂️ Tags  
`#WiFi` `#DNS` `#Windows11` `#Troubleshooting`
