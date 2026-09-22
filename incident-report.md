# Security Incident Report - YummyRecipesForMe.com

**Date:** Sep 22, 2026
**Analyst:** [Tera Naam]
**Incident ID:** YRF-2026-001

## 1. Protocols Identified
- DNS (Port 53): Resolved yummyrecipesforme.com -> 203.0.113.22 and greatrecipesforme.com -> 192.0.2.17
- TCP (3-way handshake): SYN, SYN-ACK, ACK observed
- HTTP (Port 80): GET / request observed
- IP: Routing layer

## 2. Incident Summary
Attacker (former employee) performed brute force attack using default passwords. Gained admin access, injected malicious JavaScript that forced users to download executable. File redirected users to greatrecipesforme.com containing malware. Customers reported slow PCs. Owner locked out.

Evidence: tcpdump logs, customer emails, source code analysis by senior analyst.

## 3. Remediation
Recommended: Implement 2FA and Limit Login Attempts to 5 per 10 mins + Account Lockout. Also enforce strong password policy and remove default credentials.
