## 📘 Project Overview
This mini project demonstrates **Linux Identity and Access Management (IAM)** and **System Hardening** techniques on Ubuntu.  
It focuses on managing users, groups, and file permissions securely — while identifying and fixing misconfigurations in a vulnerable system.

---

## 🎯 Objective
- Build a secure IAM model (Users, Groups, Permissions)
- Detect and fix 3 misconfigurations in a vulnerable VM
- Generate a remediation report and checklist

---

## 🧰 Tools & Environment
- Ubuntu Server VM (for IAM & Hardening)
- Kali/Attacker VM (for testing)
- `sudo` access for configuration
- Tools: `useradd`, `chmod`, `acl`, `auditd`, `visudo`

---

## 🧩 Tasks

### 🧠 Task 1 — Policy + User & Group Configuration
- Create roles: **Admin**, **Developer**, **Auditor**
- Add users & groups using `useradd` and `groupadd`
- Apply **least privilege principle** in `/etc/sudoers`
- Use POSIX permissions + ACLs for folder control
- Enable **auditd** to track `/etc/sudoers` and `/etc/passwd` changes

### 🔍 Task 2 — Vulnerability Analysis & Remediation
- Analyze vulnerable VM and find 3 issues:
  1. World-writable `/etc/cron.d`
  2. Sudo with `NOPASSWD`
  3. Weak file permissions on `/etc/shadow`
- Fix each issue, record evidence (before/after)
- Create a **Remediation Checklist** and a **Policy Document**

---

## 📚 Skills & Learning
- Linux user & group management  
- File permissions & ACLs  
- Sudo security configuration  
- Auditing & logging with auditd  
- Detecting and fixing vulnerabilities
 ## 📸 Screenshots


<img width="553" height="521" alt="Screenshot 2025-11-06 012217" src="https://github.com/user-attachments/assets/8742f3bc-ee72-4fa5-aca7-5baa005cba4a" />


<img width="398" height="66" alt="Screenshot 2025-11-06 012847" src="https://github.com/user-attachments/assets/836cd15a-ae15-4bdc-8a10-e40efd844cbd" />

<img width="716" height="230" alt="Screenshot 2025-11-06 012857" src="https://github.com/user-attachments/assets/7e9ef781-6327-418c-8fd9-7490de6805f3" />
<img width="895" height="444" alt="Screenshot 2025-11-06 012935" src="https://github.com/user-attachments/assets/10c16a1a-4b38-4572-a5d3-056e252efaa2" />

<img width="711" height="237" alt="Screenshot 2025-11-06 013006" src="https://github.com/user-attachments/assets/32ad4045-0ec9-4313-9640-e44462d19434" />
<img width="721" height="399" alt="Screenshot 2025-11-06 012951" src="https://github.com/user-attachments/assets/d657e137-a9cb-4021-b32a-876d41d69b19" />
<img width="716" height="144" alt="Screenshot 2025-11-06 013016" src="https://github.com/user-attachments/assets/f54fd0ba-5038-49c9-ab01-a6a1b724ef8c" />
<img width="685" height="283" alt="Screenshot 2025-11-06 013043" src="https://github.com/user-attachments/assets/10119432-159a-404d-9517-6be4deb9ae5c" />
<img width="696" height="455" alt="Screenshot 2025-11-06 013034" src="https://github.com/user-attachments/assets/7738963b-45d9-4d8b-a4ae-e43d495c2df4" />
<img width="818" height="170" alt="Screenshot 2025-11-06 013057" src="https://github.com/user-attachments/assets/6149dd90-8de7-4d67-8342-2155a2c4cfc9" />
