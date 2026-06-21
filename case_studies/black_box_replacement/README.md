# Case Study: Transitioning from Opaque SaaS to Deterministic Audit-Grade GRC

## Executive Summary
A multinational healthcare organization abandoned a $150,000 annual contract with a leading commercial GRC platform. The commercial tool provided "black box" risk scores that could not be mathematically verified by internal auditors. SENTINEL replaced this system, providing 100 percent transparency, cryptographic score lineage, and complete data sovereignty.

## The Challenge
The organization's internal audit committee raised concerns regarding their third-party risk platform. 
* Risk scores fluctuated without clear explanation.
* External auditors required mathematical proof of how specific vendor scores were derived, which the SaaS vendor refused to provide.
* Sensitive vendor assessment data was stored on third-party cloud infrastructure.

## The SENTINEL Solution
The organization migrated their vendor portfolio to SENTINEL, utilizing its deterministic scoring engine and cryptographic audit capabilities.

### Cryptographic Score Lineage
Every assessment processed by SENTINEL generates a permanent, tamper-evident record. The engine produces three distinct SHA-256 hashes for every run:
1. The exact weights and thresholds used.
2. The specific questionnaire schema utilized.
3. The exact responses provided by the vendor.

![Audit and Vendor Details](../../../assets/screenshots/ui_preview_4.png)

### Zero Black Box Operations
Unlike commercial alternatives, SENTINEL operates entirely on open-source YAML configurations. The healthcare organization was able to print the exact mathematical formula used for scoring and hand it directly to their external auditors.

## Business Impact
* **Cost Reduction:** Eliminated a six-figure annual recurring software expense.
* **Audit Compliance:** Passed the subsequent external SOC 2 Type II audit with zero exceptions related to vendor risk management.
* **Data Sovereignty:** Successfully brought all sensitive vendor risk data completely in-house, deployed via Docker on their internal secure network.
