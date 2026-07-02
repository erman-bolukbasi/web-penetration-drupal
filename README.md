# Web Penetration Testing — Drupal (CVE-2018-7600)

> **Type:** Internship Project | **Company:** BB CyberSec | **Period:** Nov 2024 – Jan 2025

---

## 📋 Project Overview

This project documents a full penetration test conducted on a Drupal web application as part of my cybersecurity internship at BB CyberSec. The assessment focused on identifying and exploiting the critical vulnerability **CVE-2018-7600** (Drupalgeddon 2), a remote code execution vulnerability affecting Drupal core.

---

## 🎯 Objectives

- Perform a structured security audit of a Drupal-based web application
- Identify vulnerabilities using industry-standard tools
- Exploit CVE-2018-7600 to demonstrate impact and severity
- Document findings and recommend concrete security measures

---

## 🛠️ Tools Used

| Tool | Purpose |
|------|---------|
| **Nmap** | Network scanning & service enumeration |
| **Burp Suite** | Web application traffic analysis & manual testing |
| **Metasploit** | Exploitation of CVE-2018-7600 |
| **Droopescan** | Drupal version detection & plugin enumeration |
| **Nikto** | Web server vulnerability scanner |

---

## 🔍 Methodology

The penetration test followed the standard **PTES (Penetration Testing Execution Standard)** methodology:

### 1. Reconnaissance & Enumeration
- Scanned the target with **Nmap** to identify open ports and running services
- Detected Drupal version using **Droopescan**
- Enumerated web directories and endpoints

### 2. Vulnerability Analysis
- Identified **CVE-2018-7600** (Drupalgeddon 2) — a critical RCE vulnerability (CVSS: 9.8)
- Analyzed the attack surface using **Burp Suite**
- Scanned for additional weaknesses with **Nikto**

### 3. Exploitation
- Used **Metasploit** module `exploit/unix/webapp/drupal_drupalgeddon2` to exploit CVE-2018-7600
- Successfully gained remote code execution on the target system
- Demonstrated privilege escalation potential

### 4. Post-Exploitation & Reporting
- Documented all findings with severity ratings
- Assessed business impact of each vulnerability
- Derived concrete remediation recommendations

---

## 🚨 Vulnerability Details

| Field | Details |
|-------|---------|
| **CVE ID** | CVE-2018-7600 (Drupalgeddon 2) |
| **CVSS Score** | 9.8 (Critical) |
| **Affected Versions** | Drupal < 7.58, < 8.3.9, < 8.4.6, < 8.5.1 |
| **Vulnerability Type** | Remote Code Execution (RCE) |
| **Attack Vector** | Network — no authentication required |
| **Impact** | Full system compromise |

---

## ✅ Findings & Recommendations

| # | Finding | Severity | Recommendation |
|---|---------|----------|----------------|
| 1 | CVE-2018-7600 — Unauthenticated RCE | 🔴 Critical | Update Drupal to latest version immediately |
| 2 | Outdated Drupal core | 🔴 Critical | Implement patch management process |
| 3 | Unnecessary open ports | 🟡 Medium | Apply principle of least privilege on firewall |
| 4 | Missing security headers | 🟡 Medium | Configure CSP, HSTS, X-Frame-Options |
| 5 | Directory listing enabled | 🟠 High | Disable directory listing on web server |

---

## 🛡️ Skills Demonstrated

`Penetration Testing` `Ethical Hacking` `Web Application Security`
`Vulnerability Analysis` `Exploit Development` `Security Reporting`
`Nmap` `Metasploit` `Burp Suite` `CVE Research`

---

## ⚠️ Disclaimer

This project was conducted in a **controlled lab environment** as part of an authorized internship at BB CyberSec. All testing was performed with explicit permission. The techniques documented here are for **educational purposes only**. Unauthorized penetration testing is illegal.

---

## 👤 Author

**Erman Bölükbasi** — Cybersecurity Engineer & CS Student
- 🌐 [www.bb-cybersec.de](https://www.bb-cybersec.de)
- 💼 [LinkedIn](https://linkedin.com/in/erman-bb-cyber-security-engineer)
- 🐙 [GitHub](https://github.com/erman-bolukbasi)
