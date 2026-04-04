# 🏢 Enterprise Active Directory Lab

> **Windows Server · Active Directory DS · Group Policy · NTFS · File Server · VMware**

![Status](https://img.shields.io/badge/Status-Completed-2ea44f?style=flat-square)
![Platform](https://img.shields.io/badge/Platform-Windows%20Server-0078D4?style=flat-square&logo=windows)
![Tool](https://img.shields.io/badge/Virtualization-VMware%20Workstation-607078?style=flat-square)
![Type](https://img.shields.io/badge/Lab-Enterprise%20Simulation-6e40c9?style=flat-square)

---

## 📌 Overview

This project simulates a **real-world enterprise IT environment** built from scratch in an isolated virtual lab.

It covers the full lifecycle of a Windows domain infrastructure: Active Directory design, secure file server configuration, Group Policy enforcement, and end-to-end validation — directly applicable to **IT Support**, **Junior Sysadmin**, and **Network Administrator** roles.

---

## 🧱 Lab Architecture

| Component | Details |
|---|---|
| Domain Controller | Windows Server (AD DS) |
| Client Machine | Windows 10 |
| Network Type | Host-only — isolated internal lab |
| Virtualization | VMware Workstation |

---

## ⚙️ Technologies & Tools

`Active Directory DS` · `Group Policy (GPO)` · `NTFS Permissions` · `SMB / File Sharing` · `Windows Server` · `Windows 10` · `VMware Workstation` · `DNS`

---

## 🗂️ Project Structure

```
Lab
├── Part 1 — Active Directory Structure (OUs + Users)
├── Part 2 — File Server Configuration (NTFS Permissions)
├── Part 3 — Group Policy (GPO Enforcement)
└── Part 4 — Testing & Validation
```

---

## 🔹 Part 1 — Active Directory Structure

### Organizational Units

Created a structured OU hierarchy to mirror a real enterprise:

| OU | Users |
|---|---|
| IT | `it.admin` · `it.support` |
| HR | `hr.manager` · `hr.agent` |
| Finance | `fin.manager` · `fin.agent` |

> 📸 **Screen 1** — OU structure in Active Directory Users and Computers

![Organizational Units](./s1-ou.png)

> 📸 **Screen 2** — Domain users created per department

![IT Users](./s2-it.png)
![HR Users](./s2-hr.png)
![Finance Users](./s2-finance.png)

---

## 🔹 Part 2 — File Server Configuration

### Folder Structure

Centralized file storage with department-level isolation:

```
C:\Company\
├── IT\
├── HR\
└── Finance\
```

> 📸 **Screen 3** — Company folder structure

![Folder Structure](./s3-folders.png)

### NTFS Permissions

Applied the **principle of least privilege**:

- Each department accesses **only its own folder**
- Cross-department access is **explicitly denied**

> 📸 **Screen 4** — NTFS permission configuration

![NTFS Permissions](./s4-permissions.png)

---

## 🔹 Part 3 — Group Policy (GPO)

| GPO Name | Target OU | Restriction Applied |
|---|---|---|
| HR-Policy | HR | Block Control Panel access |

> 📸 **Screen 5** — GPO creation and linking in Group Policy Management Console

![GPO Configuration](./s5-gpo.png)

---

## 🔹 Part 4 — Testing & Validation

All configurations were verified through functional testing:

| Test | Result |
|---|---|
| GPO enforcement — Control Panel blocked | ✅ Pass |
| `gpupdate /force` policy refresh | ✅ Pass |
| `ping lab.local` DNS resolution | ✅ Pass |
| Domain login with restricted user | ✅ Pass |

> 📸 **Screen 6.1** — Control Panel access blocked by GPO

![GPO Restriction](./s6-1-restriction.png)

> 📸 **Screen 6.2** — `gpupdate /force` + ping test

![Policy Test](./s6-2-gpupdate.png)

> 📸 **Screen 6.3** — Successful domain login with policies applied

![Domain Login](./s6-3-login.png)

---

## ✅ Key Achievements

- Designed and deployed a complete **Active Directory domain environment**
- Structured domain with **Organizational Units** and **6 domain users**
- Implemented **NTFS permissions** following least-privilege principles
- Created and enforced **Group Policy Objects** for centralized control
- Performed full **functional testing and validation** of all configurations

---

## 🎯 Skills Demonstrated

| Category | Skills |
|---|---|
| Windows Administration | Windows Server, AD DS, DNS, Domain Management |
| Security & Access Control | NTFS Permissions, GPO, Least Privilege |
| File Services | SMB, File Server, Folder Permissions |
| Networking | DNS Resolution, Connectivity Testing |
| Virtualization | VMware Workstation, VM Configuration |

---

## 💼 Target Roles

This project directly demonstrates skills required for:

- **IT Support Technician**
- **Junior System Administrator**
- **Network Administrator**

---

*Lab built in an isolated VMware environment — all configurations documented with screenshots and test results.*
