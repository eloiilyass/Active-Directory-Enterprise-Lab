# 🏢 Enterprise Active Directory Lab

## 📌 Project Overview

This project simulates a **real-world enterprise IT environment** using **Active Directory Domain Services (AD DS)**, **File Server**, and **Group Policy (GPO)**.

It demonstrates how to design, deploy, and secure a Windows domain infrastructure with centralized management and access control.

---

## 🧱 Lab Architecture

* **Domain Controller:** Windows Server
* **Client Machine:** Windows 10
* **Network Type:** Host-only (isolated lab)

---

## ⚙️ Technologies & Tools

* VMware Workstation
* Windows Server
* Windows 10
* Active Directory (AD DS)
* Group Policy (GPO)
* NTFS Permissions
* File Sharing (SMB)

---

# 🔹 Part 1: Active Directory Structure

## 🏢 Organizational Units & Users

### 🖥️ Screen 1: Organizational Units

Creation of Organizational Units to structure the enterprise:

* IT
* HR
* Finance

![Organizational Units](./s1-ou.png)

---

### 🖥️ Screen 2: Users Creation

Creation of domain users for each department.

#### 🔧 IT Department

* it.admin
* it.support

![IT Users](./s2-it.png)

#### 👥 HR Department

* hr.manager
* hr.agent

![HR Users](./s2-hr.png)

#### 💰 Finance Department

* fin.manager
* fin.agent

![Finance Users](./s2-finance.png)

---

# 🔹 Part 2: File Server Configuration

## 📂 Folder Structure

### 🖥️ Screen 3: Company Folder

Centralized structure:

* `C:\Company\IT`
* `C:\Company\HR`
* `C:\Company\Finance`

![Folder Structure](./s3-folders.png)

---

### 🖥️ Screen 4: NTFS Permissions

Implementation of secure access control:

* Each department accesses only its folder
* Access between departments is restricted

![NTFS Permissions](./s4-permissions.png)

---

# 🔹 Part 3: Group Policy (GPO)

### 🖥️ Screen 5: GPO Configuration

* Created GPO: **HR-Policy**
* Applied restriction: **Block Control Panel access**

![GPO Configuration](./s5-gpo.png)

---

# 🔹 Part 4: Testing & Validation

## 🧪 Functional Testing

### 🖥️ Screen 6.1: GPO Enforcement

* Control Panel access is blocked
* Restriction message displayed

![GPO Restriction](./s6-1-restriction.png)

---

### 🖥️ Screen 6.2: Policy & Network Test

* `gpupdate /force` successful
* `ping lab.local` successful

![Policy Test](./s6-2-gpupdate.png)

---

### 🖥️ Screen 6.3: Domain Login

* Successful login using domain user
* Policies applied correctly

![Domain Login](./s6-3-login.png)

---

# ✅ Key Achievements

* Designed and deployed a complete **Active Directory environment**
* Implemented **Organizational Units and user management**
* Configured **NTFS permissions for secure file access**
* Applied **Group Policy for centralized control**
* Performed **real-world testing and validation**

---

# 🎯 Skills Demonstrated

* Windows Server Administration
* Active Directory Management
* Group Policy Configuration
* File Server & Permissions
* Network Troubleshooting (DNS, Connectivity)
* Security & Access Control

---

# 📌 Conclusion

This project demonstrates the ability to build and manage a **secure enterprise-level infrastructure** using Microsoft technologies.

It reflects strong skills required for:

* IT Support Technician
* Junior System Administrator
* Network Administrator

---
