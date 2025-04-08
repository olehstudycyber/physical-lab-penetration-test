# 🏗️ Windows Server 2025 Build & Active Directory Setup

Documenting the installation, configuration, and preparation of the Windows Server 2025 environment.

---

## 🔧 Installation

- Installed **Windows Server 2025 Build 25398** from ISO
- Set hostname: `DC-Server`
- Static IP: `192.168.1.2`

---

## 🧱 Roles and Features

- Active Directory Domain Services (AD DS)
- DNS Server
- Group Policy Management
- File Server (for simulation)

---

## 🏛️ Domain Configuration

- Domain Name: `lab.internal`
- Forest and Domain Functional Level: Windows Server 2025
- Users created:
  - `admin_user`
  - `test_user`
  - `svc_account`

---

## 🔐 Security Features Enabled

- Windows Defender enabled
- Sysmon installed
- PowerShell logging enabled
- RDP and SSH access with strong passwords

---

## ✅ Next Steps

- Connect clients to domain
- Begin recon from Kali machine
- Log and analyze traffic for blue team simulations
