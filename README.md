<div align="center">

![header](https://capsule-render.vercel.app/api?type=waving&height=220&color=0:0D0221,40:4B0082,70:6A0DAD,100:8A2BE2&text=Security%20Writeups&fontSize=52&fontColor=E0AAFF&fontAlignY=38&animation=fadeIn&desc=Application%20Security%20%7C%20Exploitation%20%7C%20Remediation&descAlignY=58&descSize=18)

[![Typing SVG](https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&duration=3200&pause=900&color=C77DFF&center=true&vCenter=true&width=780&lines=Find+the+bug.;Prove+the+impact.;Explain+it+clearly.;Fix+it+properly.)](https://github.com/Khalid-Abdullahi-Ali)

![Focus](https://img.shields.io/badge/Focus-Application%20Security-8A2BE2?style=for-the-badge&logo=owasp&logoColor=white)
![Writeups](https://img.shields.io/badge/Writeups-10-6A0DAD?style=for-the-badge&logo=readthedocs&logoColor=white)
![Methodology](https://img.shields.io/badge/Method-OWASP%20Top%2010-4B0082?style=for-the-badge)
![Location](https://img.shields.io/badge/Kampala%2C%20Uganda-0D0221?style=for-the-badge&logo=googlemaps&logoColor=white)

[![GitHub](https://img.shields.io/badge/GitHub-0D0221?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Khalid-Abdullahi-Ali)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-4B0082?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR-LINKEDIN)
[![Email](https://img.shields.io/badge/Email-6A0DAD?style=for-the-badge&logo=gmail&logoColor=white)](mailto:YOUR-EMAIL)

</div>

---

## 🟣 About This Repo

A collection of my **application security writeups**: web vulnerabilities I found, exploited in authorized environments, and, most importantly, **how to fix them**.

I'm **Khalid Abdullahi**, a **BSc Cybersecurity & Networking** student at **ISBAT University, Kampala**, working toward a career in **Application Security**. Every writeup here follows the same professional structure used in real security reports, because finding a bug is only half the job. The other half is communicating the risk and guiding the fix.

> *"Understand the system. Test the security."*

**Open To:**

- Application Security roles
- AppSec / Penetration Testing internships

---

## 🟣 Writeup Index

> Click a title to open the full writeup. Severity uses **CVSS v3.1**.

| # | Writeup | Category | Platform | Severity | Key Takeaway |
|---|---------|----------|----------|----------|--------------|
| 01 | [Writeup title](./writeups/01-title/README.md) | SQL Injection | Lab / CTF | 🔴 High | One-line summary |
| 02 | [Writeup title](./writeups/02-title/README.md) | XSS (Stored) | Lab / CTF | 🟠 Medium | One-line summary |
| 03 | [Writeup title](./writeups/03-title/README.md) | IDOR | Lab / CTF | 🟠 Medium | One-line summary |
| 04 | [Writeup title](./writeups/04-title/README.md) | Broken Authentication | Lab / CTF | 🔴 High | One-line summary |
| 05 | [Writeup title](./writeups/05-title/README.md) | SSRF | Lab / CTF | 🔴 High | One-line summary |
| 06 | [Writeup title](./writeups/06-title/README.md) | Access Control | Lab / CTF | 🟠 Medium | One-line summary |
| 07 | [Writeup title](./writeups/07-title/README.md) | CSRF | Lab / CTF | 🟡 Low | One-line summary |
| 08 | [Writeup title](./writeups/08-title/README.md) | File Upload | Lab / CTF | 🔴 High | One-line summary |
| 09 | [Writeup title](./writeups/09-title/README.md) | Command Injection | Lab / CTF | 🔴 Critical | One-line summary |
| 10 | [Writeup title](./writeups/10-title/README.md) | Business Logic | Lab / CTF | 🟠 Medium | One-line summary |

---

## 🟣 Vulnerability Coverage

| Domain | Topics Covered |
| ------ | -------------- |
| **Injection** | SQLi, command injection, template injection |
| **Authentication & Sessions** | Broken auth, weak session handling, brute force, missing rate limiting |
| **Access Control** | IDOR, privilege escalation, forced browsing |
| **Client-Side** | Reflected / stored / DOM XSS, CSRF |
| **Server-Side** | SSRF, insecure file upload, path traversal |
| **Logic & Design** | Business logic flaws, insecure workflows |

---

## 🟣 How Every Writeup Is Structured

Each writeup follows the same format so it reads like a real security finding:

| Section | What It Covers |
| ------- | -------------- |
| 📝 **Summary** | What the vulnerability is and why it matters, in two or three sentences |
| 🎯 **Scope & Setup** | Target, environment, tools used |
| 🔍 **Discovery** | How the issue was found: recon, testing approach, the thing that looked off |
| 💥 **Exploitation** | Step-by-step reproduction with requests, payloads, and screenshots |
| 📊 **Impact & Severity** | What an attacker gains, with a CVSS v3.1 score and vector |
| 🛠️ **Root Cause** | The actual flaw in the code or design |
| ✅ **Remediation** | Concrete fix, with secure code examples where relevant |
| 📚 **References** | CWE, OWASP, and further reading |

---

## 🟣 Tools & Methodology

**Tooling**

![Burp Suite](https://img.shields.io/badge/Burp%20Suite-8A2BE2?style=for-the-badge&logo=burpsuite&logoColor=white)
![OWASP ZAP](https://img.shields.io/badge/OWASP%20ZAP-6A0DAD?style=for-the-badge&logo=owasp&logoColor=white)
![Kali Linux](https://img.shields.io/badge/Kali%20Linux-557C94?style=for-the-badge&logo=kalilinux&logoColor=white)
![SQLmap](https://img.shields.io/badge/SQLmap-4B0082?style=for-the-badge)
![Nmap](https://img.shields.io/badge/Nmap-0D0221?style=for-the-badge&logo=nmap&logoColor=white)
![Postman](https://img.shields.io/badge/Postman-8A2BE2?style=for-the-badge&logo=postman&logoColor=white)

**Approach**

`Recon` → `Map the app` → `Test against OWASP Top 10` → `Exploit & prove impact` → `Score with CVSS` → `Recommend the fix`

---

## 🟣 Repository Structure

```
security-writeups/
├── README.md
├── writeups/
│   ├── 01-writeup-name/
│   │   ├── README.md
│   │   └── images/
│   ├── 02-writeup-name/
│   │   ├── README.md
│   │   └── images/
│   └── ...
└── templates/
    └── writeup-template.md
```

---

## 🟣 Ethics & Disclaimer

All testing was performed **only** on intentionally vulnerable applications, CTF platforms, and systems I own or have explicit written permission to test. Writeups for retired or permitted targets only. Credentials, tokens, and personal data are redacted.

The content here is for **education and defensive purposes**. Do not use these techniques against systems you do not have permission to test.

---

## 🟣 Connect

[![Email](https://img.shields.io/badge/Email-6A0DAD?style=for-the-badge&logo=gmail&logoColor=white)](mailto:YOUR-EMAIL)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-4B0082?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/YOUR-LINKEDIN)
[![GitHub](https://img.shields.io/badge/GitHub-0D0221?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Khalid-Abdullahi-Ali)
[![About Me](https://img.shields.io/badge/About%20Me-8A2BE2?style=for-the-badge&logo=github&logoColor=white)](https://github.com/Khalid-Abdullahi-Ali/About_Me)

---

<div align="center">

*"Understand the system. Test the security."*

![footer](https://capsule-render.vercel.app/api?type=waving&height=120&color=0:8A2BE2,50:4B0082,100:0D0221&section=footer)

</div>
