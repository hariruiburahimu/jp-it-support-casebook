# 🧾 Ticket 003 - Windows Account Locked / Windowsアカウントがロックされている

**Date:** 2025-07-18  
**User:** suzuki.m  
**Department:** Accounting  
**Device:** Windows 11 Desktop  
**Location:** Kyoto HQ – 5th Floor  

---

## 🛠️ Problem Description / 問題の説明

**EN:**  
User reports being unable to log into their Windows account.  
A message appears: “The referenced account is currently locked out and may not be logged on to.”

**JP:**  
ユーザーはWindowsアカウントにログインできず、「現在参照されているアカウントはロックされており、ログオンできません」というメッセージが表示されています。

---

## 🔍 Troubleshooting Steps / トラブルシューティング手順

1. Confirmed user had entered incorrect password 5+ times.  
2. Accessed another admin account on same PC.  
3. Opened **Computer Management → Local Users and Groups → Users**  
4. Located `suzuki.m` account  
5. Right-click → Properties  
6. Unchecked **"Account is locked out"** checkbox  
7. Instructed user to reset password at next login

**EN Result:**  
Account lockout was cleared. User was able to log in after resetting password.

**JP 結果:**  
アカウントのロックを解除し、ユーザーはパスワードをリセット後に正常にログインできました。

---

## 📸 Screenshot

- [ ] Add screenshot of “User Properties” window showing the unchecked “Account is locked out” option  
  *(save as `account_unlock_screenshot.png` in `/screenshots/`)*

---

## ✅ Resolution Summary / 解決の要約

**EN:** Account was locked due to multiple failed login attempts. Admin manually unlocked the account.  
**JP:** 複数回のログイン失敗によりアカウントがロックされていました。管理者が手動でロックを解除しました。

---

## 🗂️ Tags  
`#WindowsAccount` `#LockedOut` `#ComputerManagement` `#UserSupport`
