# Common Network Security Threats Report

## Introduction

Network security threats are cyber attacks that target computer networks, systems, or communication channels to steal data, interrupt services, or gain unauthorized access. As organizations increasingly rely on digital networks, understanding these threats and implementing appropriate security measures has become essential. This report discusses common network security threats, their impact, real-world examples, and effective mitigation techniques.

---

# 1. Denial of Service (DoS) and Distributed Denial of Service (DDoS)

## How it Works

A Denial of Service (DoS) attack attempts to make a system or website unavailable by overwhelming it with excessive traffic or requests. A Distributed Denial of Service (DDoS) attack works similarly, but the traffic originates from thousands or even millions of compromised devices (called a botnet), making the attack much more difficult to stop.

## Real-World Example

In 2016, the Mirai Botnet launched one of the largest DDoS attacks against Dyn, a major DNS service provider. This attack caused popular websites such as Twitter, Netflix, Reddit, and Spotify to become temporarily unavailable.

## Impact

- Website or server downtime
- Financial losses due to service interruption
- Reduced customer trust
- Decreased business productivity

## Mitigation Strategies

1. Use firewalls and intrusion prevention systems.
2. Implement DDoS protection services such as Cloudflare or AWS Shield.
3. Monitor network traffic and block suspicious requests.

---

# 2. Man-in-the-Middle (MITM) Attack

## How it Works

A Man-in-the-Middle attack occurs when an attacker secretly intercepts communication between two parties. The attacker can monitor, modify, or steal sensitive information without either party noticing.

## Real-World Example

Attackers often create fake public Wi-Fi hotspots in airports or cafes. When users connect, attackers intercept login credentials and personal information.

## Impact

- Theft of usernames and passwords
- Financial fraud
- Data leakage
- Identity theft

## Mitigation Strategies

1. Always use HTTPS websites.
2. Avoid connecting to unsecured public Wi-Fi.
3. Enable VPN when using public networks.

---

# 3. IP Spoofing

## How it Works

IP Spoofing is a technique where an attacker changes the source IP address of network packets to impersonate another trusted device or hide their identity.

## Real-World Example

IP spoofing is commonly used during DDoS attacks to hide the attacker's real location and bypass security filters.

## Impact

- Unauthorized access
- Network disruption
- Difficult attack tracing
- Supports larger cyber attacks

## Mitigation Strategies

1. Configure packet filtering on routers.
2. Use ingress and egress filtering.
3. Implement authentication mechanisms for network communication.

---

# 4. DNS Poisoning (Bonus)

## How it Works

DNS Poisoning, also called DNS Spoofing, occurs when attackers manipulate DNS records so that users are redirected to malicious websites instead of legitimate ones.

## Real-World Example

Several banking malware campaigns have used DNS poisoning to redirect users to fake banking websites that steal login credentials.

## Impact

- Credential theft
- Malware infections
- Financial fraud
- Loss of user trust

## Mitigation Strategies

1. Use DNSSEC (Domain Name System Security Extensions).
2. Regularly update DNS servers.
3. Use trusted DNS providers.

---

# Comparison of Network Security Threats

| Threat | Attack Target | Difficulty | Impact | Mitigation |
|---------|--------------|------------|--------|------------|
| DoS / DDoS | Servers & Websites | Medium | Very High | DDoS Protection, Firewalls |
| MITM | User Communication | Medium | High | HTTPS, VPN |
| IP Spoofing | Network Devices | Medium | High | Packet Filtering |
| DNS Poisoning | DNS Infrastructure | Medium | High | DNSSEC |

---

# Conclusion

## Key Takeaways

1. Network security threats can significantly affect the availability, confidentiality, and integrity of systems.
2. Preventive security measures are more effective and less costly than recovering from cyber attacks.
3. Regular monitoring, security awareness, and updated security controls help reduce cyber risks.

---

# References

1. NIST Cybersecurity Framework – https://www.nist.gov/cyberframework
2. CISA – https://www.cisa.gov
3. OWASP – https://owasp.org
4. Cloudflare Learning Center – https://www.cloudflare.com/learning/