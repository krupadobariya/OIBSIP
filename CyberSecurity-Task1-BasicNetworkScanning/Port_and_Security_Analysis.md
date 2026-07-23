# Port and Security Analysis

## Overview

This document explains the purpose of each open port detected during the Nmap scan and the potential security risks associated with them.

---

## Port 135 - MSRPC (Microsoft Remote Procedure Call)

**Purpose:**
Port 135 is used by Microsoft Windows for Remote Procedure Call (RPC). It enables communication between applications and system services on different computers.

**Security Risk:**
- Can be targeted by attackers to exploit Windows vulnerabilities.
- If exposed to untrusted networks, it may allow unauthorized remote access attempts.

**Recommendation:**
Keep Windows updated, enable the firewall, and restrict access to trusted networks only.

---

## Port 139 - NetBIOS Session Service

**Purpose:**
Port 139 supports file and printer sharing using the NetBIOS protocol.

**Security Risk:**
- May expose shared files and folders.
- Can be used for information gathering by attackers.

**Recommendation:**
Disable NetBIOS if it is not required and allow access only within trusted local networks.

---

## Port 445 - Microsoft Directory Services (SMB)

**Purpose:**
Port 445 is used by the Server Message Block (SMB) protocol for file and printer sharing in Windows.

**Security Risk:**
- Frequently targeted by malware and ransomware.
- Unpatched SMB vulnerabilities have been used in major cyberattacks.

**Recommendation:**
Keep SMB updated, disable SMBv1, and restrict access using a firewall.

---

## Port 5357 - Web Services on Devices (WSDAPI)

**Purpose:**
Port 5357 is used by Windows for discovering and managing network devices such as printers and scanners.

**Security Risk:**
- May reveal information about connected devices.
- If unnecessarily exposed, it can increase the system's attack surface.

**Recommendation:**
Disable the service if it is not required and restrict network access where possible.

---

## Conclusion

The Nmap scan identified four open ports on the target Windows 10 system. Each port provides legitimate network services but may introduce security risks if left unnecessarily exposed. Applying security updates, using firewalls, disabling unused services, and limiting access to trusted networks help reduce these risks.