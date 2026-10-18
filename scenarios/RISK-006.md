# Scenario Deep Dive: Employee Workstation Spear-Phishing

## 1. Threat Narrative
An attacker crafts a highly targeted spear-phishing email mimicking internal IT support, tricking a staff member into entering their credentials into a cloned authentication portal. The attacker uses the harvested session token to access the corporate intranet.

## 2. Business Impact Analysis
* **Operational Impact:** Unauthorized internal network access and lateral movement capability.
* **Financial & Regulatory Impact:** Costs associated with credential resets, device forensics, and potential internal data exfiltration.
* **Inherent Risk Score:** 12 (Medium) - Derived from a Likelihood of 4 and an Impact of 3.

## 3. Remediation & Control Implementation
* **FIDO2 Security Keys:** Replaced soft MFA (SMS/push) with unphishable FIDO2 hardware security keys for all employees.
* **Targeted Training:** Upgraded security awareness programs with contextual simulation tests.
* **Conditional Access Policies:** Implemented strict device-compliance checks before permitting network sign-ins.

## 4. Residual Risk Assessment
* **Residual Likelihood:** 2
* **Residual Impact:** 2
* **Residual Risk Score:** 4 (Low)
