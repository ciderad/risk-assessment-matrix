# Quantitative Risk Assessment Matrix

A structured risk register and evaluation model designed to quantify IT and infrastructure risks, calculate exposure, and prioritize remediation strategies based on industry frameworks.

## Objective
To bridge the gap between technical vulnerabilities and business impact by modeling risk scenarios, calculating residual vs. inherent risk, and justifying security controls.

## Tools & Frameworks Used
* **Spreadsheet Modeling / Python (Pandas)**
* **NIST SP 800-30** (Risk Assessment Methodology)
* **Qualitative & Quantitative Scoring Metrics** (Likelihood & Impact Scales)

## What's Included
* `risk_register.csv`: The complete master tracking sheet featuring asset valuations, threat scenarios, and mitigation controls.
* `scenarios/`: Documented walkthroughs of modeled threats (e.g., cloud data exfiltration, unpatched asset compromise).

## Sample Scenarios Evaluated
1. **Third-Party Vendor Data Leak:** Evaluated likelihood of unauthorized vendor access and modeled downstream financial and regulatory impact.
2. **Ransomware on Critical Infrastructure:** Assessed operational downtime costs and mapped mitigation improvements via multi-factor authentication and immutable backups.
