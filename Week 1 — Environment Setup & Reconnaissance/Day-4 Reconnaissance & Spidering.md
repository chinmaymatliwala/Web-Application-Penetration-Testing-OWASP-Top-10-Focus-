# Day 4 - Reconnaissance & Spidering

## Objective
### Perform reconnaissance and spidering to identify:
- application structure
- hidden routes
- sensitive endpoints
- authentication flows

## Reconnaissance Activities
### The following reconnaissance activities were performed:
- manual browsing
- application mapping
- route enumeration
- JavaScript analysis
- endpoint discovery
- spidering using OWASP ZAP
- parameter identification

## JavaScript Route Discovery
### Browser Developer Tools were used to inspect:
- main.js
- frontend route definitions
- hidden application paths

## Identified Routes
### Endpoint	Purpose
- /login	Authentication
- /administration	Admin dashboard
- /profile	User account management
- /rest/products/search	Product search API
- /contact	Feedback form

- Initial Security Observations
- Observation	Description
- Verbose Error Messages	Backend information leakage observed
- Route Exposure	Admin routes exposed in JavaScript
- Weak Input Validation	Improper validation behavior identified
- Search Reflection	Potential DOM-based XSS behavior observed

## Spidering
### OWASP ZAP spidering was used to:
- enumerate accessible endpoints
- analyze application structure
- discover hidden resources

## Evidence
### Route Discovery via DevTools
Add Screenshot:
<img width="650" height="385" alt="image" src="https://github.com/user-attachments/assets/706eb009-51aa-4096-87d4-bf9846f4007b" />
- screenshots/admin-route-discovery.png


## Spidering & Endpoint Mapping
Add Screenshot:
screenshots/spidering-results.png

## Learning Outcome
### Learned:
- application enumeration techniques
- attack surface mapping
- JavaScript reconnaissance
- route discovery methods
- endpoint analysis workflow
