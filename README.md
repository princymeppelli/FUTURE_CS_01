# 🔐 Vulnerability Assessment & Security Testing (Task 1)

This repository documents **Task 1** of my **Cyber Security Internship at Future Interns**, where I conducted a structured **vulnerability assessment** on an intentionally vulnerable web application using **OWASP ZAP**. The objective was to identify security misconfigurations, analyze risks, and map findings to the **OWASP Top 10**.

## 📌 Project Overview
*Application Tested: OWASP Juice Shop
*Assessment Type: Web Application Vulnerability Assessment
*Tool Used: OWASP ZAP (Zed Attack Proxy)
*Role: Cyber Security Analyst Intern
*Date:** December 2025
This assessment focused on identifying configuration weaknesses and missing security controls that could expose the application to common web attacks.

## 🎯 Scope of Assessment
# In Scope
* Web application endpoints
* Passive and active vulnerability scanning
* Security header analysis
* OWASP Top 10 risk mapping

## Out of Scope
* Denial of Service (DoS) attacks
* Brute-force login attacks
* Payment gateway exploitation
* Business logic abuse

## 🧪 Tools & Environment
# OWASP ZAP
* Automated passive and active scanning
* Spider & AJAX Spider for endpoint discovery
* Alert classification (High, Medium, Low, Informational)
* HTTP request–response interception and analysis

# Supporting Tools
* Google Chrome (manual exploration & validation)
* Windows OS environment
* Screenshot tools for documentation

## 🧭 Methodology
The assessment followed a **structured, industry-aligned methodology** inspired by the OWASP Testing Guide:
1. **Reconnaissance & Information Gathering**
   * Manual exploration of application pages
   * Endpoint discovery using ZAP Spider and AJAX Spider

2. **Threat Modeling**
   * Identification of potential risks such as misconfigurations, missing headers, and data exposure

3. **Automated Vulnerability Scanning**
   * Passive and active scans using OWASP ZAP
   * Analysis of headers, cookies, CORS, and server responses

4. **Manual Verification**
   * Validation of findings to reduce false positives
   * Header inspection and response behavior analysis

5. **Risk Assessment & Severity Rating*
   * Vulnerabilities categorized based on impact, exploitability, and likelihood

## 🚨 Key Vulnerability Findings

| Vulnerability                         | Severity | OWASP Category                  |
| ------------------------------------- | -------- | ------------------------------- |
| Missing Content Security Policy (CSP) | Medium   | A05 – Security Misconfiguration |
| Permissive CORS Configuration         | Medium   | A01 / A05                       |
| Server Version Information Disclosure | Low      | A06 – Vulnerable Components     |
| Missing HSTS Header                   | Low      | A02 – Cryptographic Failures    |

## 🛡️ Sample Recommendations
* Implement **Content-Security-Policy (CSP)** to prevent XSS attacks
* Restrict **CORS policies** to trusted domains
* Mask server version headers using reverse proxies
* Enforce HTTPS with **HSTS** headers

## 📊 OWASP Top 10 Compliance Summary
Several OWASP Top 10 categories were found **non-compliant** due to configuration weaknesses, highlighting the importance of secure default settings and defense-in-depth practices.

## 📘 Learning Outcomes
* Hands-on experience with **OWASP ZAP**
* Understanding real-world **security misconfigurations**
* Practical OWASP Top 10 risk mapping
* Professional vulnerability reporting and documentation
* Improved analytical and security testing skills

## 📄 Documentation
A detailed **Vulnerability Assessment & Security Report** is included, containing:

* Executive summary
* Methodology
* Screenshots as evidence
* Risk ratings
* Remediation guidance

## 👩‍💻 Author
**Meppelli Princy**
Cyber Security Intern | BCA Student
⭐ *This project was completed as part of a structured cybersecurity internship and is intended for educational and learning purposes.*
