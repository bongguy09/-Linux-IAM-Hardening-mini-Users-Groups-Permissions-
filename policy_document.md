# 🔐 Linux IAM Policy Document

### 🎯 Purpose:
To define a secure access control model for users and groups on an Ubuntu server following the **Principle of Least Privilege**.

---

### 👥 Roles and Responsibilities:

**1. Admin**
- Full sudo privileges.
- Responsible for user creation, permission management, and auditing setup.

**2. Developer**
- Can read and write files in `/project` folder.
- No sudo or system-level access.

**3. Auditor**
- Read-only access to `/project` and system logs.
- No write access anywhere else.

---

### ⚙️ Policy Rules:

| Role      | Folder Access | Sudo Access | Audit Access |
|------------|----------------|--------------|----------------|
| Admin      | All directories | Full | Yes |
| Developer  | `/project` (rwx) | No | No |
| Auditor    | `/project` (r--) | No | Yes |

---

### 🔑 Security Rules:
- Password expiry: 30 days  
- Minimum password length: 10 characters  
- No shared accounts  
- Sudo access must require a password  
- All changes logged using `auditd`

---

### 🧾 Audit Configuration:
- Monitor: `/etc/sudoers`, `/etc/passwd`, `/etc/shadow`  
- Generate log report weekly  
- Save logs in `/var/log/audit/`

---

### ✅ Summary:
This policy ensures:
- Controlled privilege separation  
- Auditable system changes  
- Reduced risk of unauthorized access
