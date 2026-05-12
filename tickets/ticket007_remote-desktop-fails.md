# 🧾 Ticket 007 - Remote Desktop Fails / リモートデスクトップ接続できない

**Date:** 2025-07-18  
**User:** mori.s  
**Department:** IT  
**Device:** Windows 11 Pro Laptop  
**Location:** Fukuoka Office – 1st Floor  

---

## 🛠️ Problem Description / 問題の説明

**EN:**  
User is unable to connect via Remote Desktop to `192.168.1.87`.  
Error message: **“Remote Desktop can’t connect to the remote computer.”**

**JP:**  
ユーザーは `192.168.1.87` にリモートデスクトップで接続できず、「リモートコンピューターに接続できません」というエラーが表示されます。

---

## 🔍 Troubleshooting Steps / トラブルシューティング手順

1. Verified both devices are on same subnet (via `ipconfig`)  
2. Pinged target IP → Successful  
3. On remote PC, checked:  
   - **Settings → System → Remote Desktop** → Enabled  
   - **Firewall > Allow apps** → Remote Desktop allowed  
4. Verified user is in **Remote Desktop Users** group  
5. Restarted **Remote Desktop Services** from `services.msc`  
6. Re-attempted connection → Successful  

**EN Result:**  
Remote Desktop was disabled in settings. Enabled feature and user gained access.

**JP 結果:**  
リモートデスクトップが無効になっていたため、有効化して接続に成功しました。

---

## 📸 Screenshot

- [ ] Screenshot of Remote Desktop settings window  
  *(save as `remote_desktop_enabled.png` in `/screenshots/`)*

---

## ✅ Resolution Summary / 解決の要約

**EN:**  
Remote Desktop was disabled. Enabled RDP in settings and firewall, and ensured group permissions were correct.

**JP:**  
リモートデスクトップが無効になっていたため、設定とファイアウォールを調整し、グループ権限を確認して解決しました。

---

## 🗂️ Tags  
`#RemoteDesktop` `#RDP` `#Firewall` `#Windows11` `#Services`
