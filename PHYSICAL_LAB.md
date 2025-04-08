# 🧪 Physical Cybersecurity Lab Setup

This document outlines the hardware and network layout for my physical cybersecurity home lab used to simulate real-world attacks and defenses in an isolated environment.

---

## 🧱 Hardware Inventory

| Device             | OS / Role              | Specs                        |
|--------------------|------------------------|-------------------------------|
| Dell Laptop        | Kali Linux (Attacker)  | 8GB RAM, i5 CPU               |
| iBUYPOWER PC       | Windows Server 2025    | 16GB RAM, i7 CPU              |
| HP Laptop          | Windows 11 Pro (Admin) | 12GB RAM, Ryzen 5             |
| Netgear Router     | Internal Network       | 192.168.1.1                   |

---

## 🌐 Network Design

- **Subnet:** `192.168.1.0/24`
- **Kali IP:** `192.168.1.10`
- **Server IP:** `192.168.1.2`
- **Router:** `192.168.1.1`
- **No external internet access**

All devices are connected via Ethernet to ensure low latency and security.

---

## 🔒 Security

- Physically isolated room with restricted access
- Default router login credentials changed
- Windows Defender firewall enabled
- Sysmon installed on Server for logging

---

## 🧰 Tools Used

- Ethernet cables (Cat5e)
- USB boot drives for OS installation
- Monitor switch (optional)
