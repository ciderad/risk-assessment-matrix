# Scenario Deep Dive: Unauthorized API Data Exposure

## 1. Threat Narrative
A malicious actor targets a customer-facing web API and exploits a Broken Object-Level Authorization (BOLA) flaw. By sequentially guessing user ID parameters in HTTP requests, the attacker scrapes thousands of user profile records without triggering authentication alerts.

## 2. Business Impact Analysis
* **Operational Impact:** Loss of data confidentiality and mass scraping of user PII.
* **Financial & Regulatory Impact:** Reputational fallout and potential regulatory scrutiny regarding data protection duties.
* **Inherent Risk Score:** 12 (Medium) - Derived from a Likelihood of 4 and an Impact of 3.

## 3. Remediation & Control Implementation
* **Token Validation:** Refactored endpoint logic to strictly validate session context against the requested resource ownership.
* **Rate Limiting:** Implemented API gateway rate limiting and anomaly detection for rapid high-volume requests.
* **Code Review Integration:** Added automated API security checks into the software development lifecycle (SDLC).

## 4. Residual Risk Assessment
* **Residual Likelihood:** 2
* **Residual Impact:** 2
* **Residual Risk Score:** 4 (Low)
