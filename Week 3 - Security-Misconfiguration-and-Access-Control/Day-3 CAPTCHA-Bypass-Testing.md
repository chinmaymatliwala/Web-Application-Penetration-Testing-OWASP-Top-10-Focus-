# Day 3 — CAPTCHA Bypass Testing

## Objective

Assess anti-automation controls implemented within the feedback submission process.

---

## Vulnerability Information

| Field         | Value                  |
| ------------- | ---------------------- |
| Vulnerability | CAPTCHA Bypass         |
| Category      | Broken Anti-Automation |
| Severity      | Medium                 |

---

## Description

The CAPTCHA implementation allowed reuse of previously valid CAPTCHA values.

Requests could be replayed without requiring fresh CAPTCHA validation.

---

## Affected Endpoint

```text
https://juice-shop.herokuapp.com/#/contact
```

---

## Testing Methodology

### Step 1

Open the feedback form.

### Step 2

Submit valid feedback.

### Step 3

Intercept the POST request using Burp Suite.

### Step 4

Observe CAPTCHA-related parameters.

### Step 5

Replay the request using the same CAPTCHA information.

### Step 6

Verify successful submission.

---

## Impact

An attacker may perform:

* Automated submissions
* Spam campaigns
* Bot abuse
* Brute-force support attacks

---

## Evidence

### Screenshot 1

Feedback form with CAPTCHA.

**Source:** Report Page 17 (Upper Screenshot)

```text
screenshots/day3-captcha-form.png
```

### Screenshot 2

Captured POST request.

**Source:** Report Page 17 (Lower Screenshot)

```text
screenshots/day3-captcha-request.png
```

### Screenshot 3

Successful replay request.

**Source:** Report Page 18

```text
screenshots/day3-captcha-bypass-success.png
```

---

## Learning Outcome

Learned how weak CAPTCHA validation can undermine anti-automation protections.
