# Day 3 - HTTP Traffic Interception Using Burp Suite

## Objective
- Intercept and analyze HTTP/HTTPS traffic between the browser and the target application.

## Activities Performed
### The following activities were completed using Burp Suite:
- HTTP request interception
- Response analysis
- Cookie inspection
- Session analysis
- Parameter discovery
- Request modification
- Repeater testing
- Intruder configuration

## HTTP Components Analyzed
### Component	Purpose
- Headers	Identify server behavior
- Cookies	Analyze session management
- Parameters	Discover user-controlled input
- JSON Payloads	Observe API communication
- Responses	Identify information leakage

##Reconnaissance Workflow

## Step 1 — Intercept Browser Requests
- Browser traffic was intercepted using Burp Suite Proxy.

## Step 2 — Analyze Application Requests
### Captured requests were examined for:
- hidden endpoints
- parameters
- session identifiers
- authentication flows

## Step 3 — Send Requests to Repeater
- Requests were forwarded to Burp Repeater for manual testing and response analysis.

## Evidence Collected
- Intercepted HTTP Request
Add Screenshot:
screenshots/intercepted-request.png

## Suggested screenshots from report:
- Screenshot 1
- Screenshot 4
- Screenshot 9

## Burp Suite Repeater Analysis
Add Screenshot:
screenshots/burp-repeater-analysis.png

## Learning Outcome
## Learned:
- HTTP request/response structure
- browser-to-server communication
- session analysis
- parameter inspection
- request manipulation workflow
