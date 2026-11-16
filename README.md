# 🛡️ Offensive & Defensive Security Lab

> A comprehensive, hands-on cybersecurity laboratory covering **offensive penetration testing**, **defensive network engineering**, **traffic analysis**, **threat modeling**, and **security awareness** — conducted in a safe, isolated virtual environment.

![Security](https://img.shields.io/badge/Domain-Cybersecurity-red?style=for-the-badge)
![Platform](https://img.shields.io/badge/Platform-Kali%20Linux-blue?style=for-the-badge)
![Tools](https://img.shields.io/badge/Tools-Nmap%20%7C%20Metasploit%20%7C%20Wireshark%20%7C%20Snort%20%7C%20ZAP%20%7C%20Hydra%20%7C%20GoPhish-green?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-10%20Labs%20Completed-brightgreen?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT%20%7C%20CC--BY--NC%204.0-purple?style=for-the-badge)

---

## 📋 Overview

This repository documents **10 structured laboratory experiments** demonstrating both offensive ethical penetration testing and defensive security operations. Each experiment includes rigorous step-by-step procedures, execution outputs, terminal evidence, MITRE ATT&CK mappings, and actionable remediation strategies.

### 🏗️ Lab Environment

| Component | Role | Description |
|---|---|---|
| **Kali Linux** | Attacker / Analyst Machine | Primary penetration testing and forensic platform |
| **Metasploitable 2** | Intentionally Vulnerable Target | Linux-based target containing known services, backdoors, and DVWA |
| **pfSense** | Firewall & Router | FreeBSD-based security perimeter configured with packet rules |
| **Snort** | Intrusion Detection System | Signature-based NIDS monitoring traffic for malicious signatures |
| **GoPhish** | Security Awareness Platform | Self-hosted framework for simulated phishing campaigns |
| **VirtualBox / VMware** | Hypervisor | Isolated Host-Only and Internal Network segments |

---

## 🧪 Experiments

| # | Experiment | Tools Used | Category | Focus Area |
|:---:|---|---|---|---|
| **01** | [Scanning for Vulnerabilities using Nmap & Nessus](Experiment-1-Nmap-Nessus/) | Nmap, Nessus Essentials | 🔍 Reconnaissance | Port scanning, OS/service detection & CVE vulnerability mapping |
| **02** | [Simulated Ethical Hacking with Metasploit](Experiment-2-Metasploit/) | Metasploit, Nmap, msfconsole | ⚔️ Exploitation | Controlled exploitation of vsftpd 2.3.4 backdoor to gain root shell |
| **03** | [Network Traffic Analysis with Wireshark](Experiment-3-Wireshark-Traffic-Analysis/) | Wireshark, cURL, FTP, Telnet | 📡 Traffic Analysis | Packet inspection, stream reconstruction & cleartext credential capture |
| **04** | [Firewall & IDS Setup with pfSense + Snort](Experiment-4-Firewall-IDS-Setup/) | pfSense, Snort NIDS, VirtualBox | 🛡️ Defense | Perimeter firewall rule creation & intrusion signature alert validation |
| **05** | [ARP Spoofing & Session Hijacking](Experiment-5-Sniffing-Session-Hijacking/) | arpspoof, Wireshark, sysctl | 🕵️ MITM / Sniffing | ARP cache poisoning, traffic diversion & web cookie inspection |
| **06** | [Website Risk Assessment Using OWASP ZAP](Experiment-6-OWASP-ZAP-Risk-Assessment/) | OWASP ZAP, DVWA | 🌐 Web Security | Automated DAST spidering, active scanning & OWASP Top 10 auditing |
| **07** | [OSINT Reconnaissance with Google Dorks & Shodan](Experiment-7-OSINT-Reconnaissance/) | Google Search, Shodan Search Engine | 🌐 Passive Recon | Public asset discovery, search operator dorking & banner inspection |
| **08** | [Threat Mapping & Adversary Emulation via MITRE ATT&CK](Experiment-8-MITRE-ATTACK-Threat-Mapping/) | Metasploit, Nmap, ATT&CK Matrix | 🗺️ Threat Intelligence | Mapping technical attack actions to Enterprise ATT&CK tactics & techniques |
| **09** | [Automated Password Guessing with Hydra](Experiment-9-Hydra-Password-Guessing/) | THC-Hydra, RockYou Wordlist | 🔑 Credential Access | Online dictionary & brute-force authentication testing against SSH/FTP |
| **10** | [Enterprise Phishing Simulation with GoPhish](Experiment-10-Phishing-Simulation-GoPhish/) | GoPhish Framework, SMTP | 🎣 Social Engineering | Campaign design, landing page creation & employee security awareness |

---

## 🔬 Key Competencies Demonstrated

- **Active & Passive Reconnaissance** — Subnet scanning, banner grabbing, service fingerprinting (Nmap/Nessus) alongside OSINT gathering via Google Dorks and Shodan.
- **Exploitation & Post-Exploitation** — Metasploit handler configuration, payload staging, shell interaction, and system verification under ethical boundaries.
- **Protocol Analysis & Packet Forensics** — Wireshark filter syntax, TCP stream following, cleartext protocol vulnerability analysis (HTTP, Telnet, FTP).
- **Network Defense & Monitoring** — Designing stateful firewall rules in pfSense, deploying Snort NIDS signatures, and validating intrusion alert logs.
- **Man-in-the-Middle (MITM) & Session Security** — ARP poisoning mechanics, kernel IP forwarding, and inspecting HTTP session cookie attributes (`Secure`, `HttpOnly`, `SameSite`).
- **Dynamic Application Security Testing (DAST)** — Spidering web targets, active attack injection, and automated reporting against the OWASP Top 10 checklist.
- **Threat-Informed Defense** — Translating offensive actions directly into MITRE ATT&CK Enterprise tactics, technique IDs, and blue-team detection strategies.
- **Authentication & Social Engineering Assessment** — Evaluating brute-force resilience using THC-Hydra and establishing organizational phishing simulations with GoPhish.

---

## 🚀 Getting Started

### Prerequisites

1. Hypervisor: [VirtualBox](https://www.virtualbox.org/) or [VMware Workstation](https://www.vmware.com/)
2. Attacker OS: [Kali Linux](https://www.kali.org/get-kali/) (VM or ISO)
3. Target OS: [Metasploitable 2](https://sourceforge.net/projects/metasploitable/) VM
4. Defensive Gateway: [pfSense Community Edition](https://www.pfsense.org/download/) ISO

### Setup

```bash
# Clone this repository
git clone https://github.com/Jaskaranbandral-07/Offensive-Defensive-Security-Lab.git

# Navigate into the lab directory
cd Offensive-Defensive-Security-Lab
```

Follow the self-contained `README.md` guide inside each experiment directory for step-by-step reproduction instructions and execution evidence.

---

## 📂 Repository Structure

```
Offensive-Defensive-Security-Lab/
├── README.md                                         # Master lab documentation & index
├── LICENSE                                           # MIT License for scripts & configs
├── Experiment-1-Nmap-Nessus/                         # Reconnaissance & Vulnerability Scanning
│   ├── README.md
│   └── images/
├── Experiment-2-Metasploit/                          # Ethical Hacking & Backdoor Exploitation
│   ├── README.md
│   ├── images/
│   └── demo/
├── Experiment-3-Wireshark-Traffic-Analysis/          # Packet Inspection & Protocol Forensics
│   ├── README.md
│   └── images/
├── Experiment-4-Firewall-IDS-Setup/                  # pfSense Perimeter Defense & Snort NIDS
│   ├── README.md
│   └── images/
├── Experiment-5-Sniffing-Session-Hijacking/          # ARP Cache Poisoning & Session Security
│   ├── README.md
│   └── images/
├── Experiment-6-OWASP-ZAP-Risk-Assessment/           # Web App DAST & OWASP Top 10 Auditing
│   ├── README.md
│   └── images/
├── Experiment-7-OSINT-Reconnaissance/                # Passive Recon: Google Dorking & Shodan
│   ├── README.md
│   └── images/
├── Experiment-8-MITRE-ATTACK-Threat-Mapping/         # Adversary Mapping to Enterprise ATT&CK
│   ├── README.md
│   └── images/
├── Experiment-9-Hydra-Password-Guessing/             # Credential Auditing with THC-Hydra
│   ├── README.md
│   └── images/
└── Experiment-10-Phishing-Simulation-GoPhish/        # Phishing Simulation & Awareness Training
    ├── README.md
    └── images/
```

---

## 🎓 Academic Notice & Citation

> **Academic Coursework:** This repository serves as a coursework record, research artifact, and educational reference for the Offensive & Defensive Cybersecurity Laboratory curriculum.
>
> **For Students & Researchers:** You are welcome to reference, study, and reproduce these experiments in an isolated virtual lab environment. Please uphold academic integrity and adhere to your institution's honor code by understanding and performing the experiments independently rather than copying verbatim.

---

## ⚠️ Disclaimer

> **All experiments are conducted in an isolated, private virtual lab environment for educational and defense validation purposes only.**
> Do not attempt any of these techniques, tools, or methodologies on networks, hosts, or web applications without explicit, written authorization from the system owner.
> Unauthorized access or interference with computer systems violates cyber law and is subject to criminal prosecution.

---

## 📜 Licensing & Usage

This repository employs a dual-licensing framework to differentiate executable utilities from academic documentation:

- **Source Code, Scripts & Configurations:** Licensed under the [MIT License](LICENSE). You are granted full permission to run, test, adapt, and build upon the implementations.
- **Lab Documentation, Walkthroughs & Evidence (`README.md`, reports, diagrams):** Licensed under the [Creative Commons Attribution-NonCommercial 4.0 International (CC BY-NC 4.0)](https://creativecommons.org/licenses/by-nc/4.0/) License. Free to share and adapt for non-commercial educational purposes with attribution.

---

## 🤝 Contributing

Feedback, corrections, and improvements are welcome. Please feel free to open an issue or submit a pull request!

---

<p align="center">
  Made with 🔐 by <a href="https://github.com/Jaskaranbandral-07">Jaskaran Bandral</a>
</p>
