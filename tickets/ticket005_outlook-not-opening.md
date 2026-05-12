# 🧾 Ticket 005 - Outlook Not Opening / Outlookが起動しない

**Date:** 2025-07-18  
**User:** nakamura.r  
**Department:** Sales  
**Device:** Windows 11 Laptop  
**Location:** Nagoya Branch – 4th Floor  

---

## 🛠️ Problem Description / 問題の説明

**EN:**  
User reports that Microsoft Outlook does not open. Clicking the icon does nothing, or it freezes on splash screen.

**JP:**  
ユーザーはOutlookを起動しようとすると、何も反応しないか、起動画面で止まってしまうと報告しました。

---

## 🔍 Troubleshooting Steps / トラブルシューティング手順

1. Ran `outlook.exe /safe` from Run dialog  
   → Outlook opened in Safe Mode  
2. Disabled all COM Add-ins via **File → Options → Add-ins**  
3. Restarted Outlook normally → Opened successfully  
4. Re-enabled add-ins one by one → Identified faulty one (PDF plugin)  
5. Permanently disabled faulty add-in  
6. Performed `Quick Repair` from Control Panel → Programs and Features

**EN Result:**  
Outlook opened normally after removing problematic add-in and repairing Office.

**JP 結果:**  
問題のあるアドインを無効化し、Officeを修復したことで、Outlookは正常に起動するようになりました。

---

## 📸 Screenshot

- [ ] Add screenshot of **Outlook in Safe Mode** or **Add-ins window**  
  *(save as `outlook_safe_mode.png` in `/screenshots/`)*

---

## ✅ Resolution Summary / 解決の要約

**EN:**  
Issue was caused by faulty add-in. Outlook opened in Safe Mode. Add-in disabled and Office repaired.

**JP:**  
原因は不良アドインでした。Outlookをセーフモードで起動し、アドインを無効化し、Officeを修復して解決しました。

---

## 🗂️ Tags  
`#Outlook` `#SafeMode` `#Add-ins` `#OfficeRepair`
