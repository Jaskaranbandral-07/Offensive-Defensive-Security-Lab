# 🛡️ Offensive & Defensive Security Lab

> A hands-on cybersecurity lab covering **penetration testing**, **traffic analysis**, **firewall/IDS configuration**, and **web application security** — all in a safe, isolated virtual environment.

![Security](https://img.shields.io/badge/Domain-Cybersecurity-red?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Kali%20Linux-blue?style=for-the-badge)
![Tools](https://img.shields.io/badge/Tools-Nmap%20|%20Metasploit%20|%20Wireshark%20|%20Snort-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Lab%20Completed-brightgreen?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT%20%7C%20CC--BY--NC%204.0-purple?style=for-the-badge)

---

## 📋 Overview

This repository documents **6 structured academic laboratory experiments** demonstrating both offensive ethical penetration testing and defensive cybersecurity techniques. Each experiment includes step-by-step procedures, execution outputs, and detailed analytical walkthroughs.

### 🏗️ Lab Environment

| Component | Role |
|---|---|
| **Kali Linux** | Attacker / Analyst machine |
| **Metasploitable 2** | Intentionally vulnerable target |
| **pfSense** | Firewall & IDS platform |
| **VirtualBox / VMware** | Virtualization layer |
| **Network** | Host-Only / Internal Adapter |

---

## 🧪 Experiments

| # | Experiment | Tools Used | Category |
|---|---|---|---|
| 1 | [Scanning for Vulnerabilities using Nmap & Nessus](Experiment-1-Nmap-Nessus/) | Nmap, Nessus | 🔍 Reconnaissance |
| 2 | [Simulated Ethical Hacking with Metasploit](Experiment-2-Metasploit/) | Metasploit, Nmap | ⚔️ Exploitation |
| 3 | [Network Traffic Analysis with Wireshark](Experiment-3-Wireshark-Traffic-Analysis/) | Wireshark, cURL | 📡 Traffic Analysis |
| 4 | [Firewall & IDS Setup with pfSense + Snort](Experiment-4-Firewall-IDS-Setup/) | pfSense, Snort | 🛡️ Defense |
| 5 | [ARP Spoofing & Session Hijacking](Experiment-5-Sniffing-Session-Hijacking/) | arpspoof, Wireshark | 🕵️ Sniffing & MITM |
| 6 | [OWASP ZAP & Risk Assessment](Experiment-6-OWASP-ZAP-Risk-Assessment/) | OWASP ZAP | 🌐 Web App Security |

---

## 🔬 What You'll Learn

- **Reconnaissance & Scanning** — Discover hosts, ports, and services with Nmap; identify CVEs with Nessus
- **Exploitation** — Use Metasploit to exploit known vulnerabilities (vsftpd backdoor) in a controlled setting
- **Packet Analysis** — Capture live traffic with Wireshark and detect cleartext credentials (FTP, Telnet, HTTP)
- **Firewall & IDS** — Deploy pfSense rules and Snort intrusion detection to monitor and block suspicious traffic
- **Network Attacks** — Understand ARP spoofing, MITM attacks, and session hijacking risks
- **Web App Security** — Scan web applications for OWASP Top 10 vulnerabilities using ZAP

---

## 🚀 Getting Started

### Prerequisites

1. Install [VirtualBox](https://www.virtualbox.org/) or VMware
2. Download [Kali Linux](https://www.kali.org/get-kali/) ISO/VM
3. Download [Metasploitable 2](https://sourceforge.net/projects/metasploitable/) VM
4. *(Optional)* Download [pfSense](https://www.pfsense.org/download/) ISO for Experiment 4

### Setup

```bash
# Clone this repository
git clone https://github.com/Jaskaranbandral-07/Offensive-Defensive-Security-Lab.git

# Navigate into the lab directory
cd Offensive-Defensive-Security-Lab
```

Then follow the instructions in each experiment's `README.md`.

---

## 📂 Repository Structure

```
Offensive-Defensive-Security-Lab/
├── README.md                                    # This file
├── Experiment-1-Nmap-Nessus/
│   ├── README.md                                # Full walkthrough
│   └── images/                                  # Screenshots
├── Experiment-2-Metasploit/
│   ├── README.md
│   ├── images/
│   └── demo/
├── Experiment-3-Wireshark-Traffic-Analysis/
│   ├── README.md
│   └── images/
├── Experiment-4-Firewall-IDS-Setup/
│   ├── README.md
│   └── images/
├── Experiment-5-Sniffing-Session-Hijacking/
│   ├── README.md
│   └── images/
└── Experiment-6-OWASP-ZAP-Risk-Assessment/
    ├── README.md
    └── images/
```

## 📱 Quick Access (QR Codes)

All experiments include styled QR codes for rapid mobile access and submission. A single-page, high-resolution A4 print sheet is available in the [`qr-codes/`](qr-codes/) directory:
- [📄 Download Printable A4 Sheet (PDF)](qr-codes/ALL-QR-CODES-PRINTABLE.pdf)
- [🖼️ View Printable A4 Sheet (PNG)](qr-codes/ALL-QR-CODES-PRINTABLE.png)

---

## 🎓 Academic Notice & Citation

> **Academic Coursework:** This repository serves as a coursework record and educational reference for the Offensive & Defensive Cybersecurity Laboratory.
>
> **For Students & Researchers:** You are welcome to reference, study, and reproduce these experiments in an isolated virtual lab environment. Please uphold academic integrity and adhere to your institution's honor code by understanding and performing the experiments independently rather than copying verbatim.

---

## ⚠️ Disclaimer

> **All experiments are conducted in an isolated virtual lab environment for educational purposes only.**
> Do not attempt any of these techniques on systems you do not own or have explicit authorization to test.
> Unauthorized access to computer systems is illegal and unethical.

---

## 📜 Licensing & Usage

This repository uses dual licensing to distinguish practical scripts/configurations from educational documentation:

- **Source Code & Scripts:** Licensed under the [MIT License](LICENSE). You are granted full permission to run, test, modify, and learn from the code implementations.
- **Lab Documentation & Materials (`README.md`, writeups, screenshots, scan reports):** Licensed under the [Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/) License. You may freely read, reference, and share the material for non-commercial educational purposes with appropriate attribution.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to open an issue or submit a pull request.

---

<p align="center">
  Made with 🔐 by <a href="https://github.com/Jaskaranbandral-07">Jaskaran Bandral</a>
</p>
