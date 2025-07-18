# 🧾 Ticket 004 - Low Disk Space / ディスク容量が不足しています

**Date:** 2025-07-18  
**User:** watanabe.k  
**Department:** HR  
**Device:** Windows 11 Laptop  
**Location:** Sapporo Branch – 2nd Floor  

---

## 🛠️ Problem Description / 問題の説明

**EN:**  
User received a warning: “You are running out of disk space on Local Disk (C:)”.  
System has become slow and unresponsive.

**JP:**  
ユーザーは「ローカルディスク（C:）の空き容量が不足しています」という警告を受け取り、システムの動作が遅くなっています。

---

## 🔍 Troubleshooting Steps / トラブルシューティング手順

1. Verified available space via **Settings → Storage**  
2. Opened **Disk Cleanup (cleanmgr)**  
3. Selected temporary files, system error dumps, recycle bin  
4. Deleted unnecessary files  
5. Emptied **Downloads** folder (after user confirmation)  
6. Suggested moving media files to external USB drive  
7. Gained ~12 GB of free space

**EN Result:**  
Disk space recovered. Performance improved and warning disappeared.

**JP 結果:**  
ディスク容量が回復し、システムのパフォーマンスが改善され、警告が消えました。

---

## 📸 Screenshot

- [ ] Add screenshot of **Storage Settings** or **Disk Cleanup** results  
  *(save as `disk_cleanup_result.png` in `/screenshots/`)*

---

## ✅ Resolution Summary / 解決の要約

**EN:**  
Disk was full due to temp/system files and large downloads. Cleaned using Disk Cleanup and manual deletion.

**JP:**  
一時ファイルやダウンロードフォルダのファイルが原因でディスクが満杯になっていました。クリーンアップと手動削除により解決しました。

---

## 🗂️ Tags  
`#LowDiskSpace` `#Storage` `#DiskCleanup` `#Windows11`
