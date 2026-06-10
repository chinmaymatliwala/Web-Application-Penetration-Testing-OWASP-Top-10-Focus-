# Day 2 — Broken Access Control Assessment

## Objective

Evaluate whether administrative functionality is adequately protected against unauthorized access.

---

## Vulnerability Information

| Field         | Value                  |
| ------------- | ---------------------- |
| Vulnerability | Admin Section Exposure |
| Category      | Broken Access Control  |
| Severity      | Critical               |

---

## Description

Administrative routes were discoverable through client-side resources and application route definitions.

The administration functionality could be identified and accessed through route enumeration techniques.

---

## Affected Endpoint

```text
https://juice-shop.herokuapp.com/#/administration
```

---

## Testing Methodology

### Step 1

Open Browser Developer Tools.

### Step 2

Inspect application JavaScript files.

### Step 3

Locate route definitions within the main.js file.

### Step 4

Identify the administration route.

### Step 5

Navigate directly to:

```text
/#/administration
```

### Step 6

Verify administrative functionality access.

---

## Impact

This weakness may allow attackers to:

* Discover hidden administrative functionality
* Access sensitive administrative interfaces
* Enumerate privileged features
* Increase attack surface

---

## Evidence

### Screenshot 1

Administration route discovered in application JavaScript.

**Source:** Report Page 9 (Upper Screenshot)

```text
screenshots/day2-route-discovery.png
```

### Screenshot 2

Administration dashboard displayed.

**Source:** Report Page 9 (Lower Screenshot)

```text
screenshots/day2-admin-dashboard.png
```

---

## Learning Outcome

Learned how route enumeration and exposed client-side resources can reveal sensitive administrative functionality.
