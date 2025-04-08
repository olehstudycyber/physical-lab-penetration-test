# 🔍 Reconnaissance Phase Log

This document outlines the reconnaissance (recon) phase of the penetration test against the Windows Server 2025 environment in the isolated home lab. The goal of recon is to discover hosts, open ports, services, and potential vulnerabilities before moving into active exploitation.

---

## 🌐 Lab Network Overview

- **Subnet:** `192.168.1.0/24`  
- **Attacker (Kali):** `192.168.1.10`  
- **Target (Windows Server 2025):** `192.168.1.2`  
- **Router:** `192.168.1.1`

---

## 🧪 Step 1: Host Discovery

**Command:**
```bash
nmap -sn 192.168.1.0/24
Results:

192.168.1.1 → Netgear Router

192.168.1.2 → Windows Server 2025 (Target)

192.168.1.10 → Kali Linux (Self)

🚪 Step 2: Port Scanning
Command:

bash
Copy
Edit
nmap -sS -p- -T4 -v 192.168.1.2
Open Ports Detected:

Port	Protocol	Service
22	TCP	OpenSSH
135	TCP	MSRPC
139	TCP	NetBIOS
445	TCP	SMB
3389	TCP	RDP
5985	TCP	WinRM
📜 Step 3: Service Enumeration
🔍 SMB Enumeration
Command:

bash
Copy
Edit
enum4linux -a 192.168.1.2
Nmap Scripts:

bash
Copy
Edit
nmap -p 445 --script smb-enum-shares.nse,smb-enum-users.nse 192.168.1.2
🔐 RDP Check
Command:

bash
Copy
Edit
nmap -p 3389 --script rdp-enum-encryption 192.168.1.2
🧠 Observations
AD is enabled on the target (LDAP port found in deeper scans)

SSH was manually enabled on the Windows Server

Target machine is not exposed to the internet

Likely entry points: SMB, RDP, and WinRM

📁 Attached Logs
scan1_nmap_full.txt

enum4linux_192.168.1.2.txt

rdp_enum_output.txt

📌 Recon was performed in a closed, internal lab network for educational purposes.
