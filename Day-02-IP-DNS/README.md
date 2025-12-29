[Scan document2025-12-29 22-51-15.pdf](https://github.com/user-attachments/files/24371962/Scan.document2025-12-29.22-51-15.pdf)
<img width="4211" height="5737" alt="flow chart" src="https://github.com/user-attachments/assets/90ced3b9-9ddc-4b04-8729-50c680c82fd8" />
# Day 2 – Networking Fundamentals (DFIR Perspective)

In Digital Forensics and Incident Response (DFIR), networking basics are core investigative tools, not background knowledge.

You cannot investigate a digital intrusion unless you understand:
- where a connection originated,
- who it was communicating with,
- and how that communication occurred.

Day 2 focuses on viewing networking fundamentals through the lens of an investigator.

---

## 1. IP Addresses – The Digital Footprint

IP addresses answer the primary investigative question:

**Where did the connection come from?**

### IPv4 vs IPv6

**IPv4**
- Legacy addressing standard (e.g., `192.168.1.1`)
- Limited address space
- Uses Network Address Translation (NAT)
- Common in most enterprise environments

**IPv6**
- Modern addressing standard (e.g., `2001:0db8:85a3::`)
- Extremely large address space
- Enables unique public IPs per device
- Can improve attribution accuracy in investigations

---

### Public vs Private IPs

**Private IP Addresses**
- Used within internal networks
- Common ranges:
  - `192.168.x.x`
  - `10.x.x.x`
  - `172.16.x.x – 172.31.x.x`
- Suspicious activity from private IPs often indicates internal movement or VPN usage

**Public IP Addresses**
- Used on the open internet
- Can reveal:
  - ISP
  - Approximate geolocation
  - Hosting or cloud provider

**Investigator Note**
If a private IP appears in a public-facing web server log, it may indicate:
- Reverse proxy or load balancer misconfiguration
- Header spoofing (e.g., `X-Forwarded-For`)
- Internal lateral movement after compromise

---

## 2. DNS – The Phonebook of the Internet

Attackers rarely communicate using raw IP addresses.

The Domain Name System (DNS) translates human-readable domains into IP addresses. DNS logs are often critical during incident response because they reveal outbound communication attempts.

---

### Domain Structure

Example: `mail.google.com`

- Top-Level Domain (TLD): `.com`
- Second-Level Domain (SLD): `google`
- Subdomain: `mail`

---

### Why DNS Matters in Investigations

Attackers commonly:
- Use typosquatting domains
- Generate random or rotating subdomains
- Hide Command and Control (C2) infrastructure behind legitimate-looking domains

DNS analysis helps identify malicious infrastructure and attacker communication patterns.

---

## 3. Ports and Protocols – The Doors and Languages

If an IP address is the building:
- The port is the door
- The protocol is the language spoken at that door

---

### Commonly Targeted Ports

| Port | Service | Description |
|-----|--------|-------------|
| 80 / 443 | HTTP / HTTPS | Frequently abused to hide malicious traffic |
| 22 | SSH | Common brute-force target |
| 3389 | RDP | Frequently exploited by ransomware operators |

---

### Protocols

**TCP (Transmission Control Protocol)**
- Connection-oriented
- Reliable delivery
- Used for web traffic, email, file transfers

**UDP (User Datagram Protocol)**
- Connectionless
- Faster but unreliable
- Used for DNS, streaming, VoIP, gaming

---

## Key Takeaways

Networking fundamentals allow investigators to:
- Trace the origin of malicious connections
- Detect lateral movement
- Identify attacker-controlled infrastructure
- Reconstruct attack timelines from logs

Strong fundamentals enable effective investigations before tools are applied.

---

## Tags
CyberSecurity  
DFIR  
Networking  
IncidentResponse  
BlueTeam  
LearningInPublic
