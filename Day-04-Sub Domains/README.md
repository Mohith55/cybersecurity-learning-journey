## Day 4 – Subdomain Enumeration & Hidden Attack Surfaces

### Overview
Today I learned how attackers and ethical hackers use **subdomain enumeration** to discover hidden or forgotten parts of a company’s web infrastructure. While a main website may appear secure, subdomains often host admin panels, development environments, or legacy systems that are poorly maintained — and vulnerable.

### What I Learned

- **What Are Subdomains?**  
  Subdomains are extensions of a root domain, e.g., `admin.example.com`, `test.example.com`. They often represent different services or environments.

- **Why They Matter:**  
  Many companies secure their main domain (e.g., `example.com`), but forget about subdomains — which may expose login panels, APIs, staging servers, or old CMS systems.

- **Enumeration Tools & Techniques:**  
  - **Passive Enumeration:** Using public sources like `crt.sh`, DNSdumpster, or security search engines (e.g., Censys, Shodan).
  - **Active Enumeration:** Using tools like `Amass`, `Sublist3r`, or brute-forcing with wordlists.

- **Real-World Risks:**  
  Attackers often gain a foothold through these “hidden” systems. One vulnerable forgotten subdomain can compromise the whole infrastructure.

### Key Takeaways

- Subdomain discovery is a crucial step in recon and bug bounty hunting.
- Even a secure homepage doesn’t mean the domain is fully safe.
- Regular asset inventory and cleanup are essential for organizations.

![The Secret Doors of the Internet](https://github.com/user-attachments/assets/0de5ed8a-095b-4e11-b0a8-48c927792cc7)
![The Secret Doors of the Internet (1)](https://github.com/user-attachments/assets/6552b6df-f5ab-4392-8c5c-d058bad0a0f4)
![The Secret Doors of the Internet (2)](https://github.com/user-attachments/assets/ec9d451f-3505-45d0-a73c-ab8992477142)
![The Secret Doors of the Internet (3)](https://github.com/user-attachments/assets/a550cb85-121c-4a44-be13-8c1307b0aae7)
![The Secret Doors of the Internet (4)](https://github.com/user-attachments/assets/699d1339-35a5-4376-b8f3-a4efca86dd7a)
![The Secret Doors of the Internet (5)](https://github.com/user-attachments/assets/7110201d-675c-4a1e-a8b8-b0193dee07a8)
![The Secret Doors of the Internet (6)](https://github.com/user-attachments/assets/c891a941-69f7-4aa0-be0f-da72723af47b)


