# Case Study: Eliminating Supply Chain Vulnerabilities with Strict Category Floors

## Executive Summary
A government contracting agency suffered a data breach originating from a third-party vendor. The vendor had an overall security score of 92 out of 100 on the agency's legacy GRC platform. An investigation revealed that the legacy platform averaged the scores, allowing a catastrophic failure in "Encryption Standards" to be hidden by perfect scores in administrative policies. SENTINEL was deployed to enforce strict Category Floors to prevent this from ever happening again.

## The Challenge
* Legacy GRC platforms use simple weighted averages.
* A vendor could completely fail a critical technical requirement but still achieve an "Acceptable" or "Low Risk" overall rating by over-performing in non-technical categories.
* Analysts lacked the time to manually audit every single line item for hundreds of acceptable-scoring vendors.

## The SENTINEL Solution
The agency deployed SENTINEL and configured the `CATEGORY_FLOOR_ENABLED` policy within the core ruleset.

### Uncompromising Floor Enforcement
SENTINEL evaluates each risk domain independently before calculating the aggregate score. The agency set a strict category floor of 40.0. If a vendor scores below this threshold in any single category, SENTINEL intercepts the scoring process.

![Dashboard Overview](../../assets/screenshots/ui_preview_1.png)

### Automatic Policy Blocking
Instead of averaging the failure into a passing grade, SENTINEL instantly overrides the aggregate score. The vendor is automatically classified as "High Risk", a Threshold Violation event is logged in the permanent audit trail, and webhook alerts are fired to the security team.

## Business Impact
* **Zero Silent Failures:** The agency successfully identified 14 existing vendors who had critical single-domain failures hidden behind high aggregate scores.
* **Automated Triage:** Security analysts no longer waste time manually double-checking passing vendors for hidden technical flaws.
* **Enhanced Security Posture:** The enforcement of strict category floors ensures that foundational security controls (like Encryption and Access Control) are non-negotiable prerequisites for doing business with the agency.
