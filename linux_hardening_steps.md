---
# Linux Endpoint Hardening Project

Below are the commands and steps used to harden a Linux system (Ubuntu):

---

## 1. System Updates
- Update and upgrade packages:
  ```bash
  sudo apt update && sudo apt upgrade -y
  ```

## 2. Enable and Configure UFW Firewall
- Enable firewall:
  ```bash
  sudo ufw enable
  sudo ufw default deny incoming
  sudo ufw default allow outgoing
  sudo ufw allow ssh
  ```

## 3. Secure SSH Configurations
- Edit SSH settings:
  ```bash
  sudo nano /etc/ssh/sshd_config
  ```
- Actions:
  - Disable root login.
  - Change default SSH port (optional).
  - Limit login access to specific users.

## 4. Install and Configure Fail2Ban
- Install Fail2Ban:
  ```bash
  sudo apt install fail2ban -y
  ```
- Enable and start service:
  ```bash
  sudo systemctl enable fail2ban
  sudo systemctl start fail2ban
  ```

## 5. Disable Unnecessary Services
- Example disabling services:
  ```bash
  sudo systemctl disable bluetooth
  sudo systemctl disable cups
  ```

## 6. Install and Run Rootkit Hunter
- Install:
  ```bash
  sudo apt install rkhunter -y
  ```
- Run scan:
  ```bash
  sudo rkhunter --check
  ```

## 7. Enforce Password Policies
- Edit login definitions:
  ```bash
  sudo nano /etc/login.defs
  ```
- Settings:
  - Minimum password length: 12
  - Password expiration: 90 days

## 8. Create Non-Root Administrative User
- Create user and add to sudo group:
  ```bash
  sudo adduser secureadmin
  sudo usermod -aG sudo secureadmin
  ```

## 9. Enable Automatic Security Updates
- Install unattended-upgrades:
  ```bash
  sudo apt install unattended-upgrades
  sudo dpkg-reconfigure --priority=low unattended-upgrades
  ```

## 10. Regular Log Auditing
- Check authentication logs:
  ```bash
  sudo less /var/log/auth.log
  ```

---

# Notes:
- Tested on Ubuntu 20.04 LTS.
- Always backup critical files before making major changes.

