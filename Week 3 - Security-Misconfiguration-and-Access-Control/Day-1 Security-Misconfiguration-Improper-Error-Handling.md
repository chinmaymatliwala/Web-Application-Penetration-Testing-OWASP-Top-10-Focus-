# Day 1 — Security Misconfiguration Assessment (Improper Error Handling)

## Objective

The objective of this activity was to identify whether the application exposes sensitive internal information through improperly configured error messages.

---

## Vulnerability Information

| Field         | Value                     |
| ------------- | ------------------------- |
| Vulnerability | Improper Error Handling   |
| Category      | Security Misconfiguration |
| Severity      | Low                       |
| Target        | OWASP Juice Shop          |
| Tool Used     | Burp Suite Repeater       |

---

## Description

During testing, the application returned verbose error messages when invalid search input was supplied.

The error responses disclosed backend processing information and application behavior that should not normally be visible to users.

Such disclosures can assist attackers during reconnaissance and vulnerability discovery.

---

## Affected Endpoint

```text
https://juice-shop.herokuapp.com/rest/product/search?q=
```

---

## Testing Methodology

### Step 1

Navigate to the product search functionality.

### Step 2

Intercept the request using Burp Suite.

### Step 3

Send the request to Burp Repeater.

### Step 4

Replace the search value with unexpected input.

Example:

```text
mlxody
```

### Step 5

Forward the modified request.

### Step 6

Observe the detailed error message returned by the application.

---

## Impact

Improper error handling may reveal:

* Backend application logic
* Database behavior
* Internal application structure
* Technology stack information

This information can assist attackers during later attack phases.

---

## Evidence

### Screenshot 1

Error response captured in Burp Suite.

**Source:** Report Page 5 (Upper Screenshot)

```text
screenshots/day1-error-response-1.png
```

### Screenshot 2

Detailed backend error information.

**Source:** Report Page 5 (Lower Screenshot)

```text
screenshots/day1-error-response-2.png
```

---

## Learning Outcome

Learned how verbose error messages can expose internal implementation details and increase the attack surface of a web application.
