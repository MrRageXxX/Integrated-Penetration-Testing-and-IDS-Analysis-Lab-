# Integrated-Penetration-Testing-and-IDS-Analysis-
Integrated Penetration Testing and IDS Analysis Lab using Kali Linux, Metasploit, Hydra, and Snort.
# Integrated Penetration Testing & IDS Analysis Lab

## Overview
This project demonstrates a simulated cyber attack and intrusion detection workflow in a virtualized lab environment using Kali Linux, Metasploit, Hydra, and Snort IDS.

The objective of the lab was to:
- Perform reconnaissance and vulnerability enumeration
- Simulate brute-force and exploitation attacks
- Gain reverse shell access to a vulnerable system
- Detect malicious activity using Snort IDS
- Create custom intrusion detection rules

---

# Lab Environment

## Tools Used
- Kali Linux
- Metasploitable 2
- Snort IDS
- Hydra
- Metasploit Framework
- Nmap
- Oracle VirtualBox

---

# Reconnaissance & Enumeration

Performed service discovery and version detection using Nmap.

![Nmap Enumeration](screenshots/nmap-enumeration.png)

Key exposed services identified:
- FTP
- SSH
- Samba
- PostgreSQL
- Apache Tomcat
- MySQL

---

# SSH Brute Force Simulation

Hydra was used to simulate SSH brute-force attacks against the target system.

![Hydra SSH Brute Force](screenshots/hydra-ssh-bruteforce.png)

---

# Samba Exploitation Using Metasploit

Metasploit was used to identify and exploit Samba vulnerabilities.

## Searching Samba Exploits

![Metasploit Samba Search](screenshots/metasploit-samba-search.png)

## Exploit Configuration

![Metasploit Exploit Setup](screenshots/metasploit-exploit-config.png)

---

# Reverse Shell Access

Successful exploitation resulted in a reverse shell session with root access.

![Reverse Shell](screenshots/reverse-shell-access.png)

---

# Snort IDS Monitoring

Snort was configured in IDS mode to monitor malicious traffic generated during attacks.

## SSH Brute Force Detection

![SSH Alert Detection](screenshots/snort-ssh-alerts.png)

## Reverse Shell Detection

![Reverse Shell Detection](screenshots/snort-reverse-shell-alerts.png)

---

# Custom Snort Rules

Custom Snort signatures were created to detect:
- SSH brute force attacks
- Samba exploitation attempts
- Reverse shell activity
- Netcat reverse shells

![Custom Snort Rules](screenshots/custom-snort-rules.png)

---

# Skills Demonstrated

- Penetration Testing
- Vulnerability Assessment
- IDS/IPS Monitoring
- Threat Detection
- Network Security
- Reverse Shell Analysis
- Linux Administration
- Detection Engineering

---

# Key Outcomes

- Detected SSH brute-force attacks using custom Snort rules
- Generated IDS alerts for reverse shell activity
- Successfully exploited vulnerable Samba services
- Simulated attack lifecycle from reconnaissance to exploitation
- Developed custom intrusion detection signatures

---

# Disclaimer

This project was conducted in an isolated virtual lab environment for educational and defensive cybersecurity purposes only.
