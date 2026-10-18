# Scenario Deep Dive: Ransomware on Critical Infrastructure

## 1. Threat Narrative
A corporate employee opens a malicious phishing email containing a weaponized attachment, executing a payload that establishes persistence. The attacker moves laterally across internal file shares and deploys ransomware, locking core business data and disrupting daily operations.

## 2. Business Impact Analysis
* **Operational Impact:** Complete halt of internal file sharing, administrative workflows, and engineering processes.
* **Financial & Regulatory Impact:** Severe financial loss from business interruption, potential extortion payment demands, and incident response retainers.
* **Inherent Risk Score:** 15 (High) - Derived from a Likelihood of 3 and an Impact of 5.

## 3. Remediation & Control Implementation
* **EDR Deployment:** Deployed modern Endpoint Detection and Response (EDR) tooling across 100% of hosts for automated behavioral blocking.
* **Immutable Backups:** Established air-gapped, immutable backup storage with rigorous recovery testing routines.
* **Security Awareness:** Conducted mandatory, high-frequency phishing simulations for all personnel.

## 4. Residual Risk Assessment
* **Residual Likelihood:** 1
* **Residual Impact:** 2
* **Residual Risk Score:** 2 (Low)
