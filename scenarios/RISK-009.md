# Scenario Deep Dive: Corporate Laptop Theft and Data Loss

## 1. Threat Narrative
An employee traveling for a conference has their corporate laptop stolen from their luggage at an airport. Because Full Disk Encryption (FDE) was not uniformly enforced or verified, the physical hard drive is extracted by an opportunistic actor, exposing locally cached corporate emails and documents.

## 2. Business Impact Analysis
* **Operational Impact:** Localized loss of device productivity and potential disclosure of cached internal communications.
* **Financial & Regulatory Impact:** Mandatory data breach notification expenses and asset replacement costs.
* **Inherent Risk Score:** 8 (Medium) - Derived from a Likelihood of 2 and an Impact of 4.

## 3. Remediation & Control Implementation
* **Mandatory MDM Enrollment:** Enforced automatic Mobile Device Management (MDM) enrollment for every corporate endpoint before network access is granted.
* **Enforced FDE Policies:** Programmatically mandated BitLocker and FileVault full-disk encryption with escrowed recovery keys.
* **Remote Wipe Capabilities:** Configured remote-wipe commands accessible via the security operations portal to instantly purge lost hardware.

## 4. Residual Risk Assessment
* **Residual Likelihood:** 1
* **Residual Impact:** 2
* **Residual Risk Score:** 2 (Low)
