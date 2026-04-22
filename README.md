# Penetration Testing Lab Project

## Project Title

Penetration Testing and Vulnerability Assessment on Metasploitable 2 Using Kali Linux

---

## Objective

This project demonstrates a complete penetration testing workflow in a controlled lab environment. The objective is to identify vulnerabilities in a target system and exploit them using industry-standard tools.

---

## Lab Setup

* Attacker Machine: Kali Linux
* Target Machine: Metasploitable 2
* Network: Host-Only (Isolated Environment)

---

## Tools Used

* Kali Linux
* Nmap
* Metasploit Framework
* Netdiscover
* Netcat

---

## Methodology

### 1. Network Discovery

Identified active hosts in the network using Netdiscover.

### 2. Port Scanning

Performed service and version detection using Nmap.

### 3. Service Enumeration

Analyzed open ports and identified running services such as FTP, SSH, HTTP, and SMB.

### 4. Vulnerability Identification

Detected a vulnerable Samba service running on port 445.

### 5. Exploitation

Used Metasploit module:
`exploit/multi/samba/usermap_script`

Successfully gained remote shell access.

### 6. Post-Exploitation

Verified system access using commands like:

* whoami
* uname -a
* pwd

---

## Key Finding

* Vulnerability: Samba usermap_script Command Execution
* Type: Remote Code Execution (RCE)
* Severity: High

---

## Result

Successfully exploited the Samba vulnerability and obtained root-level shell access on the target system.

---

## Mitigation

* Update Samba to latest version
* Disable unnecessary services
* Restrict SMB access
* Use firewall rules
* Perform regular vulnerability scanning

---

## Learning Outcome

* Understanding of penetration testing lifecycle
* Hands-on experience with scanning and exploitation tools
* Knowledge of real-world vulnerabilities
* Basics of post-exploitation techniques

---

## Author

Nilavarasan

---

## ⚠️ Disclaimer
* This project was performed in a controlled lab environment for educational purposes only. Do not attempt this on unauthorized systems.

This project was performed in a controlled lab environment for educational purposes only. Do not attempt this on unauthorized systems.
