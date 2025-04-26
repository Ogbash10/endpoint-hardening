---
# Windows Endpoint Hardening Project

Below are the actions taken to harden a Windows system:

---

## 1. System Updates
- Enable automatic Windows Updates.
- Install the latest patches.

## 2. Windows Defender
- Enable real-time protection.
- Enable cloud-delivered protection.
- Schedule quick and full system scans.

## 3. Windows Firewall
- Ensure firewall is enabled.
- Block all incoming connections (unless needed).
- Allow only critical outbound connections.

## 4. User Account Management
- Remove unnecessary users.
- Enforce strong passwords.
- Enable account lockout policies.
- Use standard accounts (not admin) for daily use.

## 5. BitLocker Encryption
- Enable BitLocker on system drives.
- Secure recovery keys properly.

## 6. Disable Unnecessary Services
- Disable services like:
  - Remote Desktop (unless needed)
  - SMBv1
  - Bluetooth (if unused)

## 7. Enable Audit Policies
- Logon events, object access, policy changes.

## 8. Application Whitelisting
- Configure WDAC (Windows Defender Application Control) or AppLocker.

## 9. Browser Hardening
- Enable safe browsing.
- Use security extensions.

## 10. Disable AutoRun/AutoPlay
- Prevent automatic execution from USB devices.

---

# Notes:
- Tested on Windows 10 Pro.
- Always backup important data before making critical changes.
