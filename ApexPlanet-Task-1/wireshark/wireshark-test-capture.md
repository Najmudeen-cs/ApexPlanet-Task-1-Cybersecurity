# Wireshark Test Capture

## Capture Interface

**Interface:** `eth0`

## Traffic Generated

ICMP traffic was generated from Kali to the Metasploitable2 target:

```bash
ping -c 4 192.168.56.101
```

## Display Filter

```text
icmp
```

## Observed Communication

```text
Kali
192.168.56.102
      │
      │ ICMP Echo Request / Reply
      ▼
Metasploitable2
192.168.56.101
```

The Wireshark capture showed ICMP packets traveling in both directions between the two lab machines.

## Evidence

Add the final Wireshark screenshot to:

```text
![alt text](image.png)
screenshots/
```

Recommended filename:

```text
![alt text](image-1.png)
wireshark-icmp-capture.png
```
