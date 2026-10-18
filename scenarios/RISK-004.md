# Scenario Deep Dive: Production CI/CD Pipeline Supply Chain Injection

## 1. Threat Narrative
An attacker injects malicious code into a widely used open-source Python library. Because the organization's build pipeline automatically pulls the latest minor version of dependencies without hash verification, the compromised package is compiled straight into production artifacts.

## 2. Business Impact Analysis
* **Operational Impact:** Compromise of internal application logic and potential execution of malicious remote commands in production environments.
* **Financial & Regulatory Impact:** High emergency remediation costs and loss of customer trust.
* **Inherent Risk Score:** 12 (Medium) - Derived from a Likelihood of 3 and an Impact of 4.

## 3. Remediation & Control Implementation
* **Software Composition Analysis (SCA):** Integrated automated dependency scanning tools into the CI/CD pipeline to block vulnerable or unverified packages.
* **Dependency Pinning:** Enforced strict cryptographic hash pinning for all imported third-party libraries.
* **SBOM Generation:** Implemented automated generation of Software Bill of Materials (SBOM) for every release build.

## 4. Residual Risk Assessment
* **Residual Likelihood:** 2
* **Residual Impact:** 2
* **Residual Risk Score:** 4 (Low)
