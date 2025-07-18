# 🧾 Ticket 001 - Printer Not Working / プリンタが印刷しない

**Date:** 2025-07-18  
**User:** yamada.t  
**Department:** General Affairs  
**Device:** Windows 11 Pro Desktop  
**Location:** Tokyo Office – 3rd Floor  

---

## 🛠️ Problem Description / 問題の説明

**EN:**  
User reports that the printer is powered on, connected, but does not print any document.  

**JP:**  
ユーザーはプリンターの電源が入り、接続されているにもかかわらず、印刷できないと報告しました。

---

## 🔍 Troubleshooting Steps / トラブルシューティング手順

1. Checked printer's LED status → No error lights.  
2. Verified USB connection → Replugged cable.  
3. Opened **Control Panel > Devices and Printers** → Printer was **offline**.  
4. Right-clicked printer → Selected "Use Printer Online".  
5. Cleared print queue.  
6. Performed test print.

**EN Result:**  
Printer resumed normal function after setting it online.

**JP 結果:**  
プリンターをオンラインに設定した後、通常通り印刷できるようになりました。

---

## 📸 Screenshot

- [ ] Add screenshot of "Devices and Printers" showing printer status  
  *(save as `printer_offline_fix.png` in `/screenshots/`)*

---

## ✅ Resolution Summary / 解決の要約

**EN:** Printer was offline. Manually set online via Control Panel. Print queue cleared. Resolved.  
**JP:** プリンターがオフライン状態だったため、手動でオンラインに設定し、印刷キューをクリアして解決しました。

---

## 🗂️ Tags  
`#Printer` `#Offline` `#Windows11` `#ControlPanel`

