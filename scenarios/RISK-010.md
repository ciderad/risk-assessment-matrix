# Scenario Deep Dive: SaaS Collaboration Tool Accidental Data Leak

## 1. Threat Narrative
Default tenant settings on a cloud collaboration platform allow any internal user to generate unconstrained, public web-sharing links for documents. An employee accidentally pastes a public link containing unreleased product roadmaps and strategic plans into a public forum.

## 2. Business Impact Analysis
* **Operational Impact:** Premature disclosure of confidential business strategies and proprietary intellectual property.
* **Financial & Regulatory Impact:** Loss of competitive advantage and potential market impacts.
* **Inherent Risk Score:** 9 (Medium) - Derived from a Likelihood of 3 and an Impact of 3.

## 3. Remediation & Control Implementation
* **Default Sharing Restrictions:** Updated tenant policies to block external public links by default, requiring explicit administrator approval for external sharing.
* **Data Loss Prevention (DLP):** Deployed DLP scanning to automatically flag documents containing sensitive keywords if sharing links are generated.
* **Audit Logging:** Configured continuous log monitoring for file-sharing activities to catch broad permission shifts early.

## 4. Residual Risk Assessment
* **Residual Likelihood:** 1
* **Residual Impact:** 2
* **Residual Risk Score:** 2 (Low)
