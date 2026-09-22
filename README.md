# YummyRecipesForMe Security Incident - Analysis

### Project Overview
This is a project from Google Cybersecurity Certificate Course 4.
Investigated a security incident where `yummyrecipesforme.com` was compromised via brute-force attack and was redirecting users to a malicious site `greatrecipesforme.com`.

### What I Did
- Analyzed tcpdump traffic logs to understand the attack chain
- Identified protocols involved: DNS, TCP, HTTP
- Documented the incident using NIST Incident Response lifecycle
- Proposed remediation steps

### Files in this Repo
- `tcpdump-traffic.log` - Original network log (evidence)
- `analysis-explanation.md` - My simple explanation of the log
- `incident-report.md` - Final incident report

### Key Learning
- How DNS resolution can be abused for malicious redirection
- How to read tcpdump logs (3-way handshake, GET requests)
- Incident documentation

### Tools Used
Wireshark concepts, tcpdump, DNS Analysis, GitHub

---
*This project is part of my Google Cybersecurity portfolio. Original logs provided by Google for educational purposes.*
