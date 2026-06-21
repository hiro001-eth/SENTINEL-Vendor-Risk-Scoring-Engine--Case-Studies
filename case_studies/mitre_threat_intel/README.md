# Case Study: Unifying Compliance and Threat Intelligence via MITRE ATT&CK

## Executive Summary
A global retail corporation struggled to bridge the gap between their compliance analysts and their Security Operations Center (SOC). Compliance data was viewed as an administrative exercise, while the SOC focused purely on technical threats. SENTINEL bridged this divide by automatically translating vendor compliance gaps into actionable MITRE ATT&CK threat tactics.

## The Challenge
* The GRC team successfully identified that a major logistics vendor lacked proper multi-factor authentication and data-at-rest encryption.
* This information was buried in a 50-page PDF report.
* The SOC team was unaware of this specific supply chain vulnerability and did not adjust their threat hunting or monitoring parameters accordingly.

## The SENTINEL Solution
SENTINEL's advanced analysis engine was configured to automatically map specific questionnaire failures directly to the MITRE ATT&CK framework.

### Actionable Threat Mapping
When the logistics vendor failed the access control and encryption requirements, SENTINEL immediately flagged the exact threat tactics that malicious actors could exploit due to these missing controls.

![MITRE Mapping Interface](../../assets/screenshots/ui_preview_6.png)

### Automated SOC Alerting
Instead of waiting for a manual report, SENTINEL utilized its webhook integration to instantly alert the SOC channel. The alert explicitly detailed that the vendor was vulnerable to T1078 (Valid Accounts) and T1486 (Data Encrypted for Impact).

## Business Impact
* **Proactive Defense:** The SOC team was able to immediately deploy custom detection rules for anomalous authentication attempts originating from the vulnerable vendor's IP space.
* **Cross-Department Synergy:** Compliance checklists were transformed into highly technical, actionable intelligence.
* **Risk Mitigation:** A subsequent credential stuffing attack against the vendor was successfully contained because the retail organization had already elevated their monitoring posture based on SENTINEL's MITRE output.
