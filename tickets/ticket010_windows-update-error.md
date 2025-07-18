# 🧾 Ticket 010 - Windows Update Error 0x80070002 / Windowsアップデートエラー

**Date:** 2025-07-18  
**User:** yoshida.m  
**Department:** Operations  
**Device:** Windows 11 Desktop  
**Location:** Nagasaki Branch – 2nd Floor  

---

## 🛠️ Problem Description / 問題の説明

**EN:**  
User reports that Windows Update fails repeatedly.  
Error code shown: **0x80070002 – "Something went wrong."**

**JP:**  
ユーザーはWindowsアップデートが何度も失敗し、「0x80070002」というエラーコードが表示されます。

---

## 🔍 Troubleshooting Steps / トラブルシューティング手順

1. Opened **Settings → Windows Update** → Confirmed updates failing  
2. Stopped **Windows Update** and **Background Intelligent Transfer Service (BITS)** via `services.msc`  
3. Deleted contents of `C:\Windows\SoftwareDistribution\Download`  
4. Restarted the services  
5. Ran `sfc /scannow` → No integrity violations found  
6. Restarted PC  
7. Ran Windows Update again → Success  

**EN Result:**  
Corrupted update files removed. Update completed successfully after services reset.

**JP 結果:**  
破損したアップデートファイルを削除し、サービスを再起動することで正常にアップデートが完了しました。

---

## 📸 Screenshot

- [ ] Screenshot of Windows Update error  
  *(save as `windows_update_error.png` in `/screenshots/`)*

---

## ✅ Resolution Summary / 解決の要約

**EN:**  
Update failed due to corrupted cached files. Issue resolved by deleting cache and restarting update services.

**JP:**  
キャッシュされた破損ファイルが原因でアップデートが失敗していました。削除とサービス再起動により解決しました。

---

## 🗂️ Tags  
`#WindowsUpdate` `#Error0x80070002` `#SoftwareDistribution` `#SFC` `#Windows11`
