# Oleh Borysovskyy - Cybersecurity Home Lab

Welcome to my physical cybersecurity home lab! This repository documents the full setup, testing process, and analysis of a simulated enterprise network I built for learning and demonstration purposes.

## 🔧 Project Overview

- Physical lab with Kali Linux, Windows Server 2025, Windows 11 Pro
- Active Directory configured and targeted in penetration testing
- Tools used: Nmap, Metasploit, Mimikatz, Wazuh, Sysmon, etc.

## 📁 Repository Structure

- `PHYSICAL_LAB.md`: Details of hardware setup and networking
- `BUILD_SERVER.md`: Windows Server 2025 installation and AD setup
- `recon_logs/`: Network scans and enumeration
- `exploitation/`: Exploit strategies and execution logs
- `post_exploitation/`: Credential dumping, persistence methods
- `hardening/`: Defense tactics (GPOs, Defender settings)
- `SIEM_IDS/`: Wazuh, Sysmon, and logging configuration
- `reports/`: Final assessment, recommendations, documentation

## 📬 Contact
For feedback or collaboration: [Your Email or LinkedIn]

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
![Nmap Full TCP Scan]([recon/nmap_full_tcp_scan_192.168.1.2_2025-03-30.pn](https://github.com/olehstudycyber/physical-lab-penetration-test/blob/main/recon/nmap_full_tcp_scan_192.168.1.2_2025-03-30.jpg)


### Reconnaissance Phase

📄 [Nmap Scan Result - 2025-03-30](recon/nmap_scan_2025-03-30.txt)


You can find terminal outputs, Nmap scans, and screenshots in the `/logs/` and `/screenshots/` folders.

---

## 📁 Project Structure

# physical-lab-penetration-test
