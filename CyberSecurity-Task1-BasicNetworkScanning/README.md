# Basic Network Scanning with Nmap

## Project Overview

This project demonstrates how Nmap can be used to scan a local machine to identify open ports, running services, and the operating system. The scan results are documented along with a security analysis of the detected services.

---

## Objective

- Install Nmap on a Windows system.
- Perform different types of network scans.
- Identify open ports and running services.
- Detect the operating system.
- Analyse the security risks of the discovered services.
- Document all findings.

---

## Development Environment

| Component | Details |
|----------|---------|
| Operating System | Windows 10 |
| Tool Used | Nmap |
| Terminal | Command Prompt |

---

## Nmap Installation

Nmap was installed using the official installer downloaded from the Nmap website.

Official Website:
https://nmap.org/download.html

### Installation Steps

1. Download the latest Windows installer.
2. Run the installer.
3. Keep the default installation options.
4. Install Npcap when prompted.
5. Finish the installation.
6. Verify installation using:

```bash
nmap --version
```

---

## Scan Types Performed

The following scans were performed during this task:

- Basic Scan (`nmap <target IP>`)
- Service Version Scan (`nmap -sV <target IP>`)
- Operating System Detection (`nmap -O <target IP>`)

The detailed scan results are available in **nmap_scan_results.txt**.

---

## Repository Contents

- README.md
- nmap_scan_results.txt
- Port_and_Security_Analysis.md
- screenshots/

---

## About Nmap

Nmap (Network Mapper) is an open-source network scanning tool used to discover devices, identify open ports, detect running services, and gather information about a target system. It is widely used for network administration and security testing.

---

## Why Network Scanning Matters

Network scanning helps identify active services running on a system. It allows administrators to detect unnecessary open ports, verify network configurations, and identify possible security risks before they can be exploited.

---

## Ethical Use Guidelines

Network scanning should only be performed on systems that you own or have permission to test. Scanning unauthorized systems may violate laws and ethical guidelines. This project was performed only on a local machine for educational purposes.

---

## Key Learnings

- Learned how to install and use Nmap.
- Performed different types of network scans.
- Identified open ports and running services.
- Understood the security risks associated with open ports.
- Learned the importance of ethical network scanning.