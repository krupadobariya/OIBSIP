# Task 1 - Basic Network Scanning with Nmap

## Objective

Perform a basic network scan using Nmap on my local Windows machine to identify open ports, services, and operating system information.

---

## Tools Used

- Nmap 7.99
- Windows 10
- Command Prompt

---

## Target

Local Machine IP:

10.130.146.163

---

## Commands Used

### Basic Scan

```bash
nmap 10.130.146.163
```

### Service Version Scan

```bash
nmap -sV 10.130.146.163
```

### OS Detection

```bash
nmap -O 10.130.146.163
```