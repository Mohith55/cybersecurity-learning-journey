## Day 5 – Reverse IP Lookup: Shared Hosting Risks

### Overview
On Day 5, I explored how a seemingly secure website can be compromised through the server it shares with other vulnerable sites. This is where **Reverse IP Lookup** becomes a powerful reconnaissance technique. It allows security researchers to find all domains hosted on the same server/IP address.

### What I Learned

- **What Is Reverse IP Lookup?**  
  A technique used to identify all domain names hosted on the same IP address (shared hosting).

- **Why It Matters:**  
  If one site on a shared server is poorly secured, it can expose or compromise the others — even if the target site looks secure from the outside.

- **Common Use Cases:**  
  - Uncover phishing domains hosted alongside real websites  
  - Identify attacker infrastructure clusters  
  - Audit all assets a company owns (shadow IT)

### Tools/Resources

- [viewdns.info/reverseip](https://viewdns.info/reverseip/)  
- [YouGetSignal Reverse IP](https://www.yougetsignal.com/tools/web-sites-on-web-server/)  
- `host` or `nslookup` commands  
- [SecurityTrails](https://securitytrails.com)

### Key Takeaways

- Shared servers = shared risk.  
- Reverse IP lookups are fast and legal ways to map hidden infrastructure.  
- Ideal for OSINT, bug bounty recon, and digital forensics.
![a-dark-cybersecurity-illustration-with-a_7j9sdhGuTa-HMwzqgpWMJQ_bcZSBqK8RKOkSW_dQC-WFA](https://github.com/user-attachments/assets/f4a45377-1de9-4da5-911d-401a581d48c3)
