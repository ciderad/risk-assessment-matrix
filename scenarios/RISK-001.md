# Scenario Deep Dive: Third-Party Vendor Data Leak

## 1. Threat Narrative
An external software vendor with portal access falls victim to a credential-harvesting campaign. The attacker uses the compromised vendor credentials to authenticate into the cloud management portal, bypassing primary perimeter defenses due to a lack of enforced multi-factor authentication (MFA).

## 2. Business Impact Analysis
* **Operational Impact:** Potential unauthorized exfiltration of internal configuration files and downstream customer PII.
* **Financial & Regulatory Impact:** Potential breach notification costs, compliance penalties under frameworks like GDPR/CCPA, and enterprise reputational damage.
* **Inherent Risk Score:** 20 (High) - Derived from a Likelihood of 4 and an Impact of 5.

## 3. Remediation & Control Implementation
To drive down the residual risk, the following controls were implemented:
* **Enforced MFA:** Mandated FIDO2 hardware security keys or authenticator apps for all third-party vendor accounts.
* **Least-Privilege Access:** Restricted vendor permissions strictly to their designated staging environments, removing cross-tenant access.
* **Continuous Monitoring:** Integrated vendor activity log monitoring with automated alerting for anomalous login locations.

## 4. Residual Risk Assessment
Following implementation, the score decreased to:
* **Residual Likelihood:** 2
* **Residual Impact:** 3
* **Residual Risk Score:** 6 (Medium)
