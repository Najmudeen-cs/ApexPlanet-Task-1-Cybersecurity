# Lab Setup Report

## 1. Environment

**Virtualization:** Oracle VirtualBox

**Attacker:** Kali Linux

**Target:** Metasploitable2

**Network:** VirtualBox Host-Only Adapter

## 2. Network Configuration

| Machine | Role | IP Address |
|---|---|---|
| Kali Linux | Attacker | `192.168.56.102` |
| Metasploitable2 | Target | `192.168.56.101` |

Subnet:

```text
192.168.56.0/24
```

## 3. Connectivity Verification

Connectivity was tested from Kali to Metasploitable2 using ICMP:

```bash
ping -c 4 192.168.56.101
```

The test produced successful ICMP replies with **0% packet loss**.

## 4. Wireshark Verification

Wireshark was run on Kali and a capture was performed on `eth0`.

The capture was filtered using:

```text
icmp
```

The captured traffic showed bidirectional ICMP communication between:

```text
192.168.56.102  ↔  192.168.56.101
```

## 5. Evidence

Add the following screenshots to this directory:

1. VirtualBox Host-Only network configuration
2. Metasploitable2 IP configuration
3. Kali IP configuration
4. Successful Kali → Metasploitable2 ping
5. Wireshark ICMP capture

## 6. Result

The isolated cybersecurity lab environment was successfully configured and connectivity between the attacker and target machines was verified.

> This report should be accompanied by the actual screenshots captured during the lab setup.
