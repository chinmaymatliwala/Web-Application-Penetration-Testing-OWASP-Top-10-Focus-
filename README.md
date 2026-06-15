# Web Application Penetration Testing (OWASP Top 10 Focus)

## Project Overview

This project demonstrates a structured web application penetration testing assessment performed against **OWASP Juice Shop**, a deliberately vulnerable web application designed for security training and awareness.

The assessment was conducted using the **OWASP Top 10 framework**, focusing on identifying, exploiting, documenting, and analyzing common web application vulnerabilities.

The project was completed in four phases covering reconnaissance, vulnerability discovery, exploitation, risk assessment, and remediation planning.

---

## Problem Statement

Perform a penetration test on a vulnerable web application using the OWASP Top 10 framework.

Objectives:

* Discover common web application vulnerabilities
* Exploit identified vulnerabilities in an authorized environment
* Document findings with proof-of-concept evidence
* Assess risk and business impact
* Provide remediation guidance
* Produce a professional penetration testing report

---

# Target Application

**OWASP Juice Shop**

A modern intentionally insecure web application maintained by OWASP for security training and penetration testing practice.

Target URL:

```text
https://juice-shop.herokuapp.com
```

---

# Testing Environment

| Component          | Details                      |
| ------------------ | ---------------------------- |
| Operating System   | Kali Linux                   |
| Browser            | Mozilla Firefox              |
| Proxy Tool         | Burp Suite Community Edition |
| Scanner            | OWASP ZAP                    |
| Additional Tools   | Browser Developer Tools      |
| Target Application | OWASP Juice Shop             |

---

# Methodology

The assessment followed a structured approach based on:

* OWASP Testing Guide
* OWASP Top 10
* PTES (Penetration Testing Execution Standard)

### Assessment Lifecycle

1. Reconnaissance
2. Information Gathering
3. Vulnerability Identification
4. Exploitation
5. Risk Analysis
6. Documentation
7. Remediation Planning

---

# Project Timeline

## Week 1 — Environment Setup & Reconnaissance

### Activities

* Studied OWASP Top 10 vulnerabilities
* Configured Kali Linux testing environment
* Installed and configured Burp Suite
* Configured OWASP ZAP
* Configured browser proxy interception
* Performed reconnaissance activities
* Conducted spidering and endpoint discovery
* Mapped application routes and authentication flows

### Skills Practiced

* Reconnaissance
* Traffic Analysis
* Proxy Configuration
* Application Mapping
* Route Enumeration

---

## Week 2 — Vulnerability Testing

### Focus Areas

* SQL Injection
* Broken Authentication
* Cross-Site Scripting (XSS)
* Sensitive Data Exposure

### Activities

* Login bypass testing
* Authentication assessment
* XSS payload testing
* Information disclosure testing
* Sensitive document exposure analysis
* Database schema disclosure testing

### Skills Practiced

* Vulnerability Discovery
* Request Manipulation
* Burp Repeater
* Burp Intruder
* Payload Analysis

---

## Week 3 — Security Misconfiguration & Broken Access Control

### Focus Areas

* Security Misconfiguration
* Broken Access Control
* Proof-of-Concept Development

### Activities

* Improper Error Handling assessment
* Administrative route discovery
* Access control validation
* CAPTCHA bypass testing
* PoC documentation

### Skills Practiced

* Access Control Testing
* Security Configuration Review
* Route Enumeration
* Request Replay Attacks
* PoC Creation

---

## Week 4 — Final Report & Documentation

### Activities

* Consolidated findings
* Performed risk assessment
* Prepared remediation recommendations
* Finalized penetration testing report
* Documented lessons learned
* Prepared project documentation

### Skills Practiced

* Security Reporting
* Risk Assessment
* Remediation Planning
* Professional Documentation

---

# Vulnerabilities Identified

| Vulnerability                                  | Category                  | Severity |
| ---------------------------------------------- | ------------------------- | -------- |
| Improper Error Handling                        | Security Misconfiguration | Low      |
| Improper Input Validation                      | Input Validation Failure  | Medium   |
| DOM-Based Cross-Site Scripting                 | Injection                 | High     |
| Broken Access Control (Admin Section Exposure) | Broken Access Control     | Critical |
| Login Bypass via SQL Injection                 | Injection                 | Critical |
| Cross-Site Request Forgery (CSRF)              | Access Control            | High     |
| Weak Password Policy                           | Authentication Failure    | Medium   |
| CAPTCHA Bypass                                 | Broken Anti-Automation    | Medium   |
| Database Schema Disclosure                     | Information Disclosure    | High     |
| Confidential Document Exposure                 | Sensitive Data Exposure   | Critical |

---

# Severity Distribution

| Severity | Count |
| -------- | ----- |
| Critical | 3     |
| High     | 3     |
| Medium   | 3     |
| Low      | 1     |

---

# OWASP Top 10 Mapping

| OWASP Category                                 | Findings                                                 |
| ---------------------------------------------- | -------------------------------------------------------- |
| A01 – Broken Access Control                    | Admin Section Exposure, CSRF                             |
| A02 – Cryptographic Failures                   | Confidential Document Exposure                           |
| A03 – Injection                                | SQL Injection, DOM-Based XSS, Database Schema Disclosure |
| A04 – Insecure Design                          | Improper Input Validation                                |
| A05 – Security Misconfiguration                | Improper Error Handling                                  |
| A07 – Identification & Authentication Failures | Weak Password Policy, CAPTCHA Bypass                     |

---

# Repository Structure

```text
Web-Application-Penetration-Testing-OWASP-Top10/
│
├── Week-1-Environment-Setup-and-Reconnaissance/
│
├── Week-2-Vulnerability-Testing/
│
├── Week-3-Security-Misconfiguration-and-Access-Control/
│
├── Week-4-Final-Report-and-Documentation/
│
└── README.md
```

---

# Tools Used

### Burp Suite

Used for:

* Proxy interception
* Request modification
* Repeater testing
* Intruder attacks

### OWASP ZAP

Used for:

* Spidering
* Endpoint discovery
* Reconnaissance

### Browser Developer Tools

Used for:

* JavaScript analysis
* Route discovery
* Source code inspection

---

# Key Learning Outcomes

Through this project, I gained practical experience in:

* Web Application Penetration Testing
* OWASP Top 10 Vulnerabilities
* HTTP Request/Response Analysis
* Burp Suite Workflow
* Authentication Testing
* Access Control Testing
* SQL Injection
* Cross-Site Scripting (XSS)
* Information Disclosure Analysis
* Vulnerability Reporting
* Risk Assessment
* Security Documentation

---

# Disclaimer

This project was conducted exclusively in an authorized educational environment using OWASP Juice Shop, a deliberately vulnerable application designed for security training purposes.

No production systems, third-party services, or unauthorized targets were tested.

---

# Author

**Chinmay Matliwala**

MCA (Cyber Security & Forensics)

Cybersecurity Enthusiast | Web Application Security | VAPT Learner
