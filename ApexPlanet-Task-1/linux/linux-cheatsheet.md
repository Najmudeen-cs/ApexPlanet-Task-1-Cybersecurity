# 🐧 Linux Security Lab Cheat Sheet

## Navigation

```bash
pwd
ls
ls -la
cd <directory>
cd ..
cd ~
```

## Files & Directories

```bash
touch file.txt
mkdir directory
cp source destination
mv source destination
rm file.txt
rm -r directory
```

## Permissions

```bash
ls -l
chmod 755 script.sh
chmod +x script.sh
chown user:group file
```

## Package Management

```bash
apt update
apt install <package>
apt remove <package>
apt search <package>
dpkg -l
```

## Networking

```bash
ip addr
ip route
ping <IP>
ss -tuln
```

Legacy commands referenced in the task:

```bash
ifconfig
netstat
traceroute
```

## Useful Security Commands

### Nmap

```bash
nmap <TARGET-IP>
nmap -sV <TARGET-IP>
```

### Netcat

```bash
nc -h
```

### Hashing

```bash
sha256sum <file>
```

### OpenSSL

```bash
openssl version
```

## Wireshark

Start Wireshark:

```bash
wireshark
```

For the Task 1 lab capture:

- Capture on the Host-Only interface (`eth0` in the demonstrated Kali environment).
- Generate ICMP traffic with `ping`.
- Use the display filter:

```text
icmp
```

## Lab Target

```text
Kali:           192.168.56.102
Metasploitable: 192.168.56.101
Network:        192.168.56.0/24
```

