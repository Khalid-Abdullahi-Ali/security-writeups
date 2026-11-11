<div align="center">

![header](https://capsule-render.vercel.app/api?type=waving&height=220&color=0:0D0221,40:4B0082,70:6A0DAD,100:8A2BE2&text=Security%20Writeups&fontSize=52&fontColor=E0AAFF&fontAlignY=38&animation=fadeIn&desc=Application%20Security%20%7C%20Exploitation%20%7C%20Remediation&descAlignY=58&descSize=18)

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3200&pause=900&color=C77DFF&center=true&vCenter=true&width=780&lines=Find+the+bug.;Prove+the+impact.;Explain+it+clearly.;Fix+it+properly.)](https://github.com/Khalid-Abdullahi-Ali)

![Focus](https://img.shields.io/badge/Focus-Application%20Security-8A2BE2?style=for-the-badge&logo=owasp&logoColor=white)
![Writeups](https://img.shields.io/badge/Writeups-6-6A0DAD?style=for-the-badge&logo=readthedocs&logoColor=white)
![Methodology](https://img.shields.io/badge/Method-OWASP%20Top%2010-4B0082?style=for-the-badge)
![Location](https://img.shields.io/badge/Kampala%2C%20Uganda-0D0221?style=for-the-badge&logo=googlemaps&logoColor=white)

[![GitHub](https://img.shields.io/badge/GitHub-0D0221?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Khalid-Abdullahi-Ali)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-4B0082?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR-LINKEDIN)
[![Email](https://img.shields.io/badge/Email-6A0DAD?style=for-the-badge&logo=gmail&logoColor=white)](mailto:YOUR-EMAIL)

</div>

---

## About This Repo

A collection of my **application security writeups**: web vulnerabilities I found, exploited in authorized environments, and, most importantly, **how to fix them**.

> *"Understand the system. Test the security."*

**Open To:**

- Application Security roles
- AppSec / Penetration Testing 

---

## Writeup Index

> Click a title to open the full writeup. Severity is a qualitative rating, not a calculated CVSS score.

| # | Writeup | Category | Platform | Severity | Key Takeaway |
|---|---------|----------|----------|----------|--------------|
| 01 | [SQL Injection with sqlmap: DVWA](./Sqli-sqlmap-dvwa/README.md) | Injection | DVWA | 🔴 Critical | Unparameterized queries let an automated tool dump every database and table in minutes. |
| 02 | [JWT Authentication Bypass: "The Archive"](./jwt-auth-bypass-the-archive/README.md) | Broken Authentication | p3rf3ctr00t (Dojo) | 🔴 Critical | A low-severity IDOR leaked exactly the key material needed for a critical JWT algorithm-confusion attack. |
| 03 | [Mr. Robot CTF](./Mr-Robot/README.md) | Multi-stage (Auth → RCE → PrivEsc) | TryHackMe | 🔴 Critical | Chained username enumeration, no lockout, and a SUID binary into full root. |
| 04 | [The Planets: Earth](./The-planets-earth/README.md) | Cryptographic Failures / Chained RCE | VulnHub | 🔴 Critical | A reused XOR key in home-made "encryption" unraveled the entire attack chain to root. |
| 05 | [Wireless WPA2 Handshake Capture & Cracking](./Wireless-wpa2-handshake-cracking/README.md) | Wireless Security | University Lab | 🔴 High | Unauthenticated deauth frames force a handshake that's only as strong as the passphrase. |
| 06 | [Shift Registers (picoCTF)](./shift-registers/README.md) | Cryptography | CyLab / picoCTF | 🔴 High | A strong random key was masked down to 8 bits before use, collapsing the keyspace to ~128 values. |

---

## Vulnerability Coverage

| Domain | Topics Covered |
| ------ | -------------- |
| **Injection** | SQL injection (manual UNION-based and automated via sqlmap) |
| **Authentication & Sessions** | JWT algorithm confusion, username enumeration, missing rate limiting / lockout |
| **Access Control** | IDOR, privilege escalation (SUID abuse), chained authorization bypass |
| **Cryptographic Failures** | Reused XOR keystreams, weak key-space reduction, broken home-made crypto |
| **Wireless Security** | WPA2-PSK handshake capture, deauthentication attacks, offline dictionary cracking |
| **Reconnaissance & Enumeration** | Service fingerprinting, directory/virtual-host enumeration, information disclosure |

---

## How Every Writeup Is Structured

Each writeup follows the same format so it reads like a real security finding:

| Section | What It Covers |
| ------- | -------------- |
|  **Summary** | What the vulnerability is and why it matters, in a short paragraph |
|  **Attack Chain** | The full path from initial access to final impact, at a glance |
|  **Findings** | Each weakness with its CWE reference and severity |
|  **Finding Details / Procedure** | Step-by-step reproduction with commands and screenshots |
|  **Root Cause** | The actual flaw in the code or design |
|  **Remediation** | Concrete fix for each finding |
|  **References** | CWE, OWASP, and further reading |

---

## Tools & Methodology

**Tooling**

![Burp Suite](https://img.shields.io/badge/Burp%20Suite-8A2BE2?style=for-the-badge&logo=burpsuite&logoColor=white)
![Kali Linux](https://img.shields.io/badge/Kali%20Linux-557C94?style=for-the-badge&logo=kalilinux&logoColor=white)
![SQLmap](https://img.shields.io/badge/SQLmap-4B0082?style=for-the-badge)
![Nmap](https://img.shields.io/badge/Nmap-0D0221?style=for-the-badge&logo=nmap&logoColor=white)
![Aircrack--ng](https://img.shields.io/badge/Aircrack--ng-6A0DAD?style=for-the-badge)
![Metasploit](https://img.shields.io/badge/Metasploit-0D0221?style=for-the-badge&logo=metasploit&logoColor=white)
![CyberChef](https://img.shields.io/badge/CyberChef-8A2BE2?style=for-the-badge)

**Approach**

`Recon` → `Map the target` → `Confirm the vulnerability` → `Exploit & prove impact` → `Identify root cause` → `Recommend the fix`

---

## Repository Structure

```
security-writeups/
├── README.md
├── Sqli-sqlmap-dvwa/
│   ├── README.md
│   └── images/
├── jwt-auth-bypass-the-archive/
│   ├── README.md
│   └── images/
├── Mr-Robot/
│   ├── README.md
│   └── images/
├── The-planets-earth/
│   ├── README.md
│   └── images/
├── Wireless-wpa2-handshake-cracking/
│   ├── README.md
│   └── images/
└── shift-registers/
    ├── README.md
    └── images/
```

---

## Ethics & Disclaimer

All testing was performed **only** on intentionally vulnerable applications, CTF platforms, and systems I own or have explicit written permission to test. Writeups for retired or permitted targets only. Credentials, tokens, and personal data are redacted.

The content here is for **education and defensive purposes**. Do not use these techniques against systems you do not have permission to test.

---

## Connect

[![Email](https://img.shields.io/badge/Email-6A0DAD?style=for-the-badge&logo=gmail&logoColor=white)](mailto:YOUR-EMAIL)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-4B0082?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR-LINKEDIN)
[![GitHub](https://img.shields.io/badge/GitHub-0D0221?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Khalid-Abdullahi-Ali)
[![About Me](https://img.shields.io/badge/About%20Me-8A2BE2?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Khalid-Abdullahi-Ali/About_Me)

---

<div align="center">

*"Understand the system. Test the security."*

![footer](https://capsule-render.vercel.app/api?type=waving&height=120&color=0:8A2BE2,50:4B0082,100:0D0221&section=footer)

</div>
