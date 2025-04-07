# 🛡️ Physical Lab Penetration Test

This project documents a real-world-style penetration test conducted in a controlled physical lab environment using dedicated hardware and isolated networking.

---

## 🔍 Lab Overview

**Goal:** Simulate an internal network penetration test targeting a Windows Server 2025 machine using Kali Linux, identifying vulnerabilities and practicing ethical hacking techniques.

---

## 🧪 Lab Setup

| Component | Details |
|----------|---------|
| **Target Machine** | Windows Server 2025 (IP: 192.168.1.2) |
| **Attacker Machine** | Kali Linux 2024.2 (IP: 192.168.1.10) |
| **Control Machine** | Windows 11 Pro |
| **Router** | Netgear (192.168.1.1 subnet) |
| **Network** | Isolated, no internet access |
| **Security** | Windows Defender, firewall, Sysmon |

---

## ⚙️ Tools Used

- Kali Linux tools (Nmap, Netcat, etc.)
- Nmap for scanning
- Metasploit (if used)
- Wireshark (if used)
- Windows Defender logs
- Sysmon
- SSH (enabled on target)
- Manual command-line enumeration

---

## 🚀 Attack Phases

### 1. Reconnaissance
- Network discovery with `nmap`
- OS detection
- Open ports & services

### 2. Scanning & Enumeration
- SMB enumeration (if open)
- RDP, SSH check
- Active Directory recon

### 3. Exploitation (Simulated)
- Attempted exploits (manual or with tools)
- Privilege escalation (if applicable)

### 4. Post-Exploitation
- Account enumeration
- File discovery
- Defense evasion attempts

---

## 🧠 What I Learned

- Proper scanning techniques in isolated environments
- Windows Server hardening challenges
- Power of Sysmon for blue team visibility
- Importance of documentation in real-world pentests

---

## 📸 Screenshots & Logs
![Nmap Scan Result](recon/nmap_scan_kali_2025-03-30.png)

### Reconnaissance Phase

📄 [Nmap Scan Result - 2025-03-30](recon/nmap_scan_2025-03-30.txt)


You can find terminal outputs, Nmap scans, and screenshots in the `/logs/` and `/screenshots/` folders.

---

## 📁 Project Structure

# physical-lab-penetration-test
