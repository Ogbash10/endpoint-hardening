---
# Endpoint Hardening (Linux & Windows)

## Overview
This project demonstrates the application of essential endpoint hardening techniques to secure both Linux and Windows systems against cyber threats. It is designed to help businesses and organizations strengthen their endpoints by reducing vulnerabilities, enforcing security policies, and protecting sensitive data.

The configurations and steps outlined here follow industry best practices for securing systems in a corporate environment.

---

## Project Goals
- Reduce the attack surface on Linux and Windows endpoints.
- Strengthen authentication and authorization policies.
- Enable encryption, firewalls, and system monitoring.
- Protect sensitive files and critical services.
- Document clear, repeatable steps for real-world business use.

---

## Project Structure
```bash
endpoint-hardening/
├── linux_hardening_steps.md
├── windows_hardening_steps.md
├── README.md
```

---

## Linux Hardening Highlights
- Enabled UFW firewall with strict rules.
- Hardened SSH configurations to prevent unauthorized access.
- Installed Fail2Ban for intrusion prevention.
- Disabled unused services to minimize exposure.
- Configured password and account policies.
- Implemented Rootkit Hunter scanning.

(Details are available in `linux_hardening_steps.md`)

---

## Windows Hardening Highlights
- Enabled BitLocker drive encryption.
- Hardened Windows Firewall with strict inbound/outbound rules.
- Strengthened password and account lockout policies.
- Disabled unnecessary services like SMBv1 and RDP (if not required).
- Enabled system auditing and regular security patching.

(Details are available in `windows_hardening_steps.md`)

---

## Why Endpoint Hardening Matters
Endpoints are the most targeted assets by attackers. By applying hardening techniques, we minimize risks such as:
- Malware infections
- Unauthorized access
- Data breaches
- Ransomware attacks

Strong endpoint protection is critical to safeguarding business operations.

---

## Author
**Sadiq Bashiru**  
Cybersecurity Analyst | SOC Analyst  
Email: bashirusadiq10@gmail.com  
LinkedIn: [Sadiq (Abubakar) Bashiru](https://linkedin.com/in/your-link)  
GitHub: [ogbash10](https://github.com/ogbash10)

---

## License
This project is open for learning and portfolio purposes. Please adapt and enhance it based on your organization’s security needs.



