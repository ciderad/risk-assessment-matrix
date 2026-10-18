# Scenario Deep Dive: Legacy Web Application Injection Vulnerabilities

## 1. Threat Narrative
An older internal web application relies on unvalidated user input fields to construct database queries. An attacker exploits this by injecting malicious SQL payloads, allowing them to bypass login controls and extract internal records.

## 2. Business Impact Analysis
* **Operational Impact:** Compromise of database integrity and confidentiality for internal legacy tooling.
* **Financial & Regulatory Impact:** Diverted engineering hours for emergency patching and potential internal data loss.
* **Inherent Risk Score:** 12 (Medium) - Derived from a Likelihood of 4 and an Impact of 3.

## 3. Remediation & Control Implementation
* **WAF Protection:** Deployed Web Application Firewall (WAF) signature rules to block common injection vectors at the perimeter.
* **Input Sanitization:** Implemented parameterized queries and strict input type validation routines across the codebase.
* **Refactoring Schedule:** Prioritized the complete technical deprecation and migration of the legacy framework.

## 4. Residual Risk Assessment
* **Residual Likelihood:** 2
* **Residual Impact:** 2
* **Residual Risk Score:** 4 (Low)
