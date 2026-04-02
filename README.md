# 🏢 Enterprise Active Directory Lab

## 📌 Project Overview

This project simulates a real enterprise IT environment using Active Directory, File Server, and Group Policy.

---

## 🧱 Lab Architecture

* Domain Controller: Windows Server
* Client Machine: Windows 10
* Network: Host-only

---

## ⚙️ Technologies Used

* VMware Workstation
* Windows Server
* Windows 10
* Active Directory
* Group Policy (GPO)
* NTFS Permissions

---

# 🔹 Part 1: Active Directory Structure

## 🏢 Organizational Units

### 🖥️ Screen 1: Create Organizational Units

This step shows creating Organizational Units (OUs) to organize departments in the enterprise environment (IT, HR, Finance).

![Screen 1](./s1-ou.png)


### 🖥️ Screen 2: Create Users

This step shows creating users within each Organizational Unit to represent employees in different departments.

#### IT Department
![IT Users](./s2-it.png)

#### HR Department
![HR Users](./s2-hr.png)

#### Finance Department
![Finance Users](./s2-finance.png)


# 🔹 Part 2: File Server

## 📂 Folder Structure

```
D:\Company
 ├── IT
 ├── HR
 ├── Finance
```

---

## 🔐 Permissions

* Each department has access only to its folder
* Access between departments is restricted

---

# 🔹 Part 3: Group Policy (GPO)

* HR: Block Control Panel
* Finance: Disable CMD
* IT: No restrictions

---

# 🔹 Part 4: Client Testing

* Domain join successful
* Users tested
* Policies applied successfully

---

# ✅ Conclusion

This project demonstrates enterprise-level Active Directory configuration including security, file sharing, and policy management.
