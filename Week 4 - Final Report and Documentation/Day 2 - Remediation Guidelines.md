# Day 2 - Remediation Guidelines

## Objective

Provide practical remediation recommendations for all identified vulnerabilities.

---

## SQL Injection

### Recommendation

* Use parameterized queries.
* Use prepared statements.
* Validate all user input.
* Implement least-privilege database accounts.

---

## Cross-Site Scripting (XSS)

### Recommendation

* Implement output encoding.
* Use Content Security Policy (CSP).
* Avoid unsafe DOM manipulation.
* Sanitize user-controlled input.

---

## Broken Access Control

### Recommendation

* Enforce server-side authorization checks.
* Implement Role-Based Access Control (RBAC).
* Restrict access to administrative endpoints.

---

## Cross-Site Request Forgery (CSRF)

### Recommendation

* Implement CSRF tokens.
* Validate Origin headers.
* Use SameSite cookies.

---

## Weak Password Policy

### Recommendation

* Enforce complexity requirements.
* Implement account lockout policies.
* Enable Multi-Factor Authentication.

---

## Sensitive Data Exposure

### Recommendation

* Disable public access to sensitive files.
* Store confidential files outside the web root.
* Apply authentication and authorization controls.

---

## Security Misconfiguration

### Recommendation

* Disable verbose error messages.
* Harden server configurations.
* Remove unnecessary debugging information.
