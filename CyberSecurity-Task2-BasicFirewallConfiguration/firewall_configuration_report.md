# Firewall Configuration Report Using UFW

## Task Information

**Task Name:** Basic Firewall Configuration Using UFW

**Platform:** Ubuntu Linux

**Firewall Tool:** UFW (Uncomplicated Firewall)

---

# Introduction

A firewall is a security system that monitors and controls incoming and outgoing network traffic based on predefined rules. Ubuntu provides UFW (Uncomplicated Firewall), which makes firewall configuration simple and effective.

The objective of this task was to install UFW, configure basic firewall rules, and verify the configuration using Nmap.

---

# Software Used

- Ubuntu Linux
- UFW (Uncomplicated Firewall)
- Nmap
- Linux Terminal

---

# Steps Performed

## 1. Installed UFW

Verified that UFW was installed on the system.

```bash
sudo apt install ufw -y
```

**Screenshot:** `01_ufw_install.png`

---

## 2. Enabled the Firewall

Enabled UFW to start protecting the system.

```bash
sudo ufw enable
```

**Screenshot:** `02_ufw_enable.png`

---

## 3. Configured Firewall Rules

The following firewall rules were added:

### Allow SSH

```bash
sudo ufw allow ssh
```

### Block HTTP

```bash
sudo ufw deny http
```

### Allow HTTPS

```bash
sudo ufw allow https
```

### Block Telnet

```bash
sudo ufw deny 23
```

**Screenshot:** `03_firewall_rules.png`

---

## 4. Verified Firewall Status

Displayed the current firewall configuration.

```bash
sudo ufw status verbose
```

The firewall showed:

- SSH allowed
- HTTPS allowed
- HTTP denied
- Telnet denied

**Screenshot:** `04_firewall_status.png`

---

## 5. Automated Firewall Configuration

A simple shell script was created to automate the firewall configuration process. The script enabled UFW, applied the firewall rules, and displayed the firewall status.

**Screenshots:**

- `05_script_execution_1.png`
- `05_script_execution_2.png`

---

## 6. Verified Using Nmap

Firewall configuration was verified using Nmap.

```bash
sudo nmap -Pn -p 22,23,80,443 localhost
```

Nmap scanned the specified ports and displayed their current status after applying the firewall rules.

**Screenshot:** `06_nmap_test.png`

---

# Results

The firewall was successfully configured using UFW.

Configured rules included:

- SSH (Port 22) → Allowed
- HTTPS (Port 443) → Allowed
- HTTP (Port 80) → Blocked
- Telnet (Port 23) → Blocked

The firewall configuration was successfully verified using both the UFW status command and Nmap.

---

# Conclusion

This task provided practical experience in configuring a Linux firewall using UFW. It demonstrated how firewall rules can be used to control network traffic and improve system security. The configuration was verified successfully using command-line tools.

---

# Learning Outcomes

- Learned how to install and enable UFW.
- Configured firewall rules using allow and deny commands.
- Verified firewall configuration using UFW.
- Tested firewall settings using Nmap.
- Understood the importance of firewall security in Linux systems.
