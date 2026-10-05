# DVWA — Client-Side Security Assessment

## 📌 Project Overview

A hands-on Web Application Security Assessment and Remediation project performed against **Damn Vulnerable Web Application (DVWA)** in a controlled local laboratory environment.

The assessment focused on identifying, validating, and understanding client-side and related web application security weaknesses.

## 🎯 Assessment Objectives

- Identify and validate common client-side vulnerabilities
- Understand their security impact
- Analyze HTTP responses and security headers
- Assess authentication behavior
- Identify exposed user-related information
- Document remediation recommendations
- Apply responsible and authorized security testing practices

## 🔐 Vulnerabilities & Security Areas Tested

- Reflected Cross-Site Scripting (XSS)
- Stored Cross-Site Scripting (XSS)
- DOM-based XSS
- Cross-Site Request Forgery (CSRF)
- HTTP Response & Security Headers
- Brute Force Authentication Testing
- PII Exposure Assessment

## 🛠️ Tools & Technologies

- Kali Linux
- DVWA
- Burp Suite
- Firefox

## 🔎 Key Findings

### XSS
Reflected, Stored, and DOM-based XSS were successfully demonstrated in the vulnerable DVWA environment.

### CSRF
A password-change CSRF scenario was successfully demonstrated against the local DVWA application.

### Security Headers
HTTP response headers were inspected using Burp Suite. Recommended defensive headers were not observed in the tested response.

### Brute Force
Authentication behavior was assessed using invalid and valid lab credentials. A Burp Intruder workflow was prepared, but no automated brute-force success was claimed due to the available Burp Community Edition environment.

### PII Exposure
User-related information was demonstrated as accessible through the vulnerable application.

## 🛡️ Remediation

Recommended security controls include:

- Context-aware output encoding
- Input validation and sanitization
- Safe DOM APIs
- Content Security Policy (CSP)
- Anti-CSRF tokens
- SameSite cookie controls
- Security headers
- Rate limiting and account throttling
- Strong password policies and MFA
- Proper authorization controls
- Data minimization and protection

## 📂 Repository Structure

```text
DVWA-Client-Side-Security-Assessment/
│
├── Evidence/
│   ├── 01_Reflected_XSS.png
│   ├── 02_Stored_XSS.png
│   ├── 03_DOM_XSS.png
│   ├── 04_CSRF_Password_Change.png
│   ├── 05_Security_Headers_Analysis.png
│   ├── 06_BruteForce_Failed_Login.png
│   └── 07_BruteForce_Success.png
│
├── Report/
│   └── Module_6_Web_Application_Security_Assessment.pdf
│
└── README.md
