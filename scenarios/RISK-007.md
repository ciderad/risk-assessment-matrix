# Scenario Deep Dive: Stale Account Privilege Escalation

## 1. Threat Narrative
A database server retains active privileged credentials belonging to a contractor who left the company nine months prior. An attacker discovers these dormant credentials via an external leak forum and logs directly into core financial databases with full administrative rights.

## 2. Business Impact Analysis
* **Operational Impact:** Full exposure, modification, or deletion of sensitive financial tables and customer transaction logs.
* **Financial & Regulatory Impact:** Severe regulatory penalties for failing access-control baselines and lack of user lifecycle management.
* **Inherent Risk Score:** 12 (Medium) - Derived from a Likelihood of 3 and an Impact of 4.

## 3. Remediation & Control Implementation
* **Automated Identity Governance:** Integrated HR offboarding workflows to automatically disable accounts across all systems upon contract termination.
* **Periodic Access Reviews:** Instituted mandatory quarterly IAM recertification campaigns where managers must explicitly re-approve access rights.
* **Just-In-Time (JIT) Access:** Eliminated permanent standing privileges in favor of JIT elevated access sessions.

## 4. Residual Risk Assessment
* **Residual Likelihood:** 1
* **Residual Impact:** 3
* **Residual Risk Score:** 3 (Low)
