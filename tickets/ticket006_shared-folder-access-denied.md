# 🧾 Ticket 006 - Cannot Access Shared Folder / 共有フォルダーにアクセスできない

**Date:** 2025-07-18  
**User:** takahashi.y  
**Department:** Legal  
**Device:** Windows 11 Desktop  
**Location:** Tokyo Office – 6th Floor  

---

## 🛠️ Problem Description / 問題の説明

**EN:**  
User reports being unable to access a shared folder located at `\\fileserver01\legal`. Error message: **"Access is denied"** or **"Network path not found"**.

**JP:**  
ユーザーは `\\fileserver01\legal` にある共有フォルダーにアクセスできず、「アクセスが拒否されました」または「ネットワークパスが見つかりません」というエラーが表示されます。

---

## 🔍 Troubleshooting Steps / トラブルシューティング手順

1. Verified network connectivity to `fileserver01` via `ping`  
2. Confirmed folder path was typed correctly  
3. Checked user’s group membership → Not in `LegalShareAccess` group  
4. Added user to proper security group in Active Directory  
5. Ran `gpupdate /force`  
6. Restarted user’s PC  
7. Access to folder was successful

**EN Result:**  
User lacked proper group membership. Added to correct AD group and issue resolved.

**JP 結果:**  
ユーザーは正しいセキュリティグループに所属していなかったため、Active Directoryで追加し、問題を解決しました。

---

## 📸 Screenshot

- [ ] Add screenshot of **"Access is denied"** error window OR  
- [ ] Screenshot of group membership settings  
  *(save as `shared_folder_access_issue.png` in `/screenshots/`)*

---

## ✅ Resolution Summary / 解決の要約

**EN:**  
Access denied error was due to missing group membership. Resolved via AD group assignment and GP update.

**JP:**  
アクセス拒否の原因はセキュリティグループ未所属でした。ADで追加し、グループポリシーを更新して解決しました。

---

## 🗂️ Tags  
`#SharedFolder` `#AccessDenied` `#ActiveDirectory` `#GroupPolicy`
