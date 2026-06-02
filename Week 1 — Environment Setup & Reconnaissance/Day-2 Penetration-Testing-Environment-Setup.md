# Day 2 - Penetration Testing Environment Setup

## Objective
Set up a controlled penetration testing environment using Kali Linux and OWASP Juice Shop.

## Operating System
### Kali Linux was used as the primary penetration testing operating system because it includes:
- web testing tools
- interception proxies
- reconnaissance utilities
- vulnerability assessment frameworks

## Tools Installed & Configured
### Tool	Purpose
- Burp Suite Community Edition	HTTP interception and request manipulation
- OWASP ZAP	Automated scanning and spidering
- Mozilla Firefox	Browser-based testing
- FoxyProxy	Proxy switching
- Browser Developer Tools	JavaScript analysis and route discovery

## Target Application
### The target application used was:
- OWASP Juice Shop

## A deliberately insecure web application designed for:
- security awareness
- penetration testing practice
- OWASP Top 10 learning

## Deployment Used:
- Heroku hosted instance
- Local Docker setup

## Target URL:
- https://juice-shop.herokuapp.com

## Testing Scope
### Parameter	Details
- Target Application	OWASP Juice Shop
- Testing Type	Authorized educational testing
- Scope	Publicly accessible endpoints
- Out of Scope	Real systems and third-party APIs

## Environment Configuration
## Burp Suite Proxy Listener
- 127.0.0.1:8080
- Browser traffic was routed through Burp Suite for request interception and manipulation.

## SSL Certificate Installation
- The Burp Suite CA certificate was installed in Firefox to intercept HTTPS traffic securely.

## Evidence
- Kali Linux Testing Environment
<img width="1713" height="978" alt="image" src="https://github.com/user-attachments/assets/1d39cd42-c619-4cfc-939e-37c4dc34d3cf" />
screenshots/kali-environment.png

- Burp Suite Proxy Configuration
<img width="500" height="298" alt="BurpSuite Proxy Configuration" src="https://github.com/user-attachments/assets/ffefd581-f1b3-42b5-a7c7-c87e4add031c" />
screenshots/burp-proxy-config.png
