# 🔐 Footprinting & Scanning Lab (CEH)

This repository contains my hands-on practical work for cybersecurity labs focused on footprinting and scanning techniques.

---

## 📌 Tools Used

* Kali Linux
* Wireshark
* Nmap
* hping3

---

## 🔍 What I Did

### 1. OS Discovery using Wireshark

* Captured ICMP packets
* Analyzed TTL values
* Identified OS:

  * TTL = 128 → Windows
  * TTL = 64 → Linux

---

### 2. Scanning using Nmap

Commands used:

```
nmap -A 10.10.1.22
nmap -O 10.10.1.22
```

---

### 3. Firewall Evasion Techniques

```
nmap -f 10.10.1.11
nmap -g 80 10.10.1.11
nmap -D RND:10 10.10.1.11
```

---

### 4. Packet Crafting using hping3

```
hping3 10.10.1.11 --udp --rand-source --data 500
hping3 -S 10.10.1.11 -p 80 -c 5
```

---

## 📊 Key Learning

* TTL helps identify OS
* Nmap scans ports and services
* Evasion techniques bypass firewalls
* hping3 creates custom packets

---

## 📁 Files Included

* Screenshots of lab
* Practical outputs
* Commands used

---

🚀 This is part of my CEH learning journey.
