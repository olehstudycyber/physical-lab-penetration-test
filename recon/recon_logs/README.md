# 🔍 Reconnaissance Logs

This folder contains reconnaissance data and findings collected during the initial phase of the penetration test against a Windows Server 2025 target in a controlled lab environment.

## 📌 Objective
Identify live hosts, open ports, running services, and potential vulnerabilities to prepare for active exploitation.

## 🧰 Tools Used
- `nmap` for network scanning and service discovery
- `enum4linux` for SMB enumeration
- `rdp-enum-encryption` script for RDP inspection

## 📁 Files Included
- `192.168.1.2_nmap_full.txt`: Full TCP port scan
- `enum4linux_192.168.1.2.txt`: SMB enumeration details
- `rdp_enum_output.txt`: RDP encryption analysis

## 🧠 Insights
- Host 192.168.1.2 running Windows Server 2025 with SMB, RDP, SSH, and WinRM exposed
- AD likely enabled (LDAP port visible in deeper scans)
- Multiple attack vectors identified for further exploitation
![Nmap Full TCP Scan](recon/nmap_full_tcp_scan_192.168.1.2_2025-03-30.png)

This image shows the result of a full TCP SYN scan (`-sS -p-`) against the Windows Server 2025 target (192.168.1.2) conducted on March 30, 2025.

---

> All tests were conducted in an isolated lab for ethical hacking and educational purposes only.
