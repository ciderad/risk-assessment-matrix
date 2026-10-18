# Scenario Deep Dive: Public Cloud Storage Bucket Misconfiguration

## 1. Threat Narrative
An administrator deploys a new AWS S3 storage bucket for project assets but inadvertently leaves public read access enabled. Automated web-scanning bots index the bucket within hours, exposing internal system design documents and customer data files.

## 2. Business Impact Analysis
* **Operational Impact:** Exposure of proprietary intellectual property and internal network topologies.
* **Financial & Regulatory Impact:** Loss of competitive advantage and reporting obligations for exposed PII.
* **Inherent Risk Score:** 16 (High) - Derived from a Likelihood of 4 and an Impact of 4.

## 3. Remediation & Control Implementation
* **Block Public Access:** Enabled account-level "Block Public Access" settings across all cloud environments.
* **Infrastructure as Code (IaC) Scanning:** Integrated policy-as-code tools (e.g., Checkov or OPA) to catch bucket permission errors pre-deployment.
* **CSPM Tooling:** Deployed a Cloud Security Posture Management platform for real-time compliance drifting alerts.

## 4. Residual Risk Assessment
* **Residual Likelihood:** 1
* **Residual Impact:** 3
* **Residual Risk Score:** 3 (Low)
