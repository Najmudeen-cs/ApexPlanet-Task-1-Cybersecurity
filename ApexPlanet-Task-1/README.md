# 🛡️ ApexPlanet Cybersecurity Internship — Task 1

## Foundations & Environment Setup

This repository documents **Task 1** of the ApexPlanet Software Pvt. Ltd. Cybersecurity & Ethical Hacking Internship Program.

### 🎯 Objective

Build and demonstrate a controlled cybersecurity lab environment using Kali Linux as the attacker machine and Metasploitable2 as the target machine over an isolated Host-Only network.

## 🧪 Lab Architecture

```text
                VirtualBox Host-Only Network
                     192.168.56.0/24
                              │
                 ┌────────────┴────────────┐
                 │                         │
          Kali Linux                  Metasploitable2
          Attacker                    Target
        192.168.56.102              192.168.56.101
                 │                         │
                 └───────────┬─────────────┘
                             │
                      Wireshark Capture
```

### Environment

| Component | Role | Network |
|---|---|---|
| Kali Linux | Attacker / Security Testing Machine | Host-Only |
| Metasploitable2 | Intentionally Vulnerable Target | Host-Only |
| Wireshark | Network Traffic Capture | Kali / `eth0` |
| VirtualBox | Virtualization Platform | Host |

## 🔗 Lab Verification

The lab was verified by:

- Confirming the Host-Only Adapter configuration in VirtualBox.
- Identifying the Metasploitable2 address: `192.168.56.101`.
- Identifying the Kali address: `192.168.56.102`.
- Successfully testing connectivity from Kali to Metasploitable2 using ICMP.
- Capturing the ICMP traffic in Wireshark on Kali's `eth0` interface.

## 📁 Repository Structure

```text
Task-1-Foundations/
├── README.md
├── notes/
│   └── cybersecurity-foundations.md
├── linux/
│   └── linux-cheatsheet.md
├── lab/
│   └── lab-setup-report.md
├── wireshark/
│   └── wireshark-test-capture.md
└── screenshots/
    └── README.md
```

## 📚 Documentation

- [Cybersecurity Foundations](notes/cybersecurity-foundations.md)
- [Linux Cheat Sheet](linux/linux-cheatsheet.md)
- [Lab Setup Report](lab/lab-setup-report.md)
- [Wireshark Test Capture](wireshark/wireshark-test-capture.md)

## ⚠️ Lab Safety

All security testing documented in this repository is intended for the isolated lab environment and intentionally vulnerable target. No unauthorized external systems are targeted.

---

**Internship:** ApexPlanet Cybersecurity & Ethical Hacking  
**Task:** 1 — Foundations & Environment Setup
