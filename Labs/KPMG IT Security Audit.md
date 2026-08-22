---
title: IT Security Audit — Midwest Central Bank (KPMG-Sponsored Competition)
date: 2025-12
tags: [lab, project, grc, risk-assessment, compliance]
tools: [NIST CSF, GLBA, PCI DSS v4.0, threat intelligence]
domain: 5 - Security Program Management & Oversight
---

# IT Security Audit — Midwest Central Bank

A cybersecurity risk assessment and regulatory-compliance audit of a (fictitious) financial institution, produced for a **KPMG-sponsored competition** in CIS 424. This is my strongest GRC artifact: framework-driven assessment, risk prioritization, compliance gap analysis, and a costed remediation roadmap presented to a panel of industry professionals.

📄 **[Full audit report (PDF)](attachments/Midwest-Central-Bank-Security-Audit-Report.pdf)**
📊 **[Presentation deck (PDF)](attachments/Midwest-Central-Bank-Security-Audit-Presentation.pdf)**

## Objective
Assess Midwest Central Bank's IT infrastructure for security weaknesses and regulatory exposure, then deliver a prioritized, cost-aware remediation roadmap that leadership could act on.

## Methodology & Sources
Structured the audit around the **NIST Cybersecurity Framework**, evaluating technical and administrative controls against the **GLBA Safeguards Rule** and **PCI DSS v4.0**. Risks were prioritized with a likelihood-vs-impact model informed by real breach data. Threat context drew from the **FBI IC3**, **CISA advisories**, and the **2024 Verizon DBIR** (financial-services sector).

## Key Findings
Six major gaps, tied to the controls they violate:

- **Outdated infrastructure** — core servers on end-of-life Windows Server 2008/2012 with known, actively exploited vulnerabilities.
- **Missing MFA** — no MFA on privileged or customer-facing systems (blocks ~99% of automated credential attacks).
- **Flat network** — no segmentation isolating financial data from general office systems; enables lateral movement.
- **Inconsistent patching** — ~60% of systems with critical patches 30+ days overdue, including CISA-flagged actively-exploited CVEs.
- **Weak encryption** — no consistent encryption in transit, and cardholder data unencrypted at rest (PCI DSS violations).
- **No real-time monitoring** — no SIEM, so attacks go undetected (industry average ~200+ days to discover a breach without monitoring).

## Compliance Status
Assessed overall compliance at roughly **52%**. GLBA gaps included an outdated (2018) risk assessment, insufficient access controls, weak encryption, and untested training. PCI DSS violations spanned MFA (Req 8), cardholder-data encryption at rest (Req 3), monitoring/logging (Req 10), and vulnerability management (Req 6).

## Recommendations
A phased, costed roadmap: **0–3 months** (MFA, emergency patching, SIEM deployment, security training), **3–12 months** (network segmentation with zero-trust principles, legacy-system modernization, EDR, a tested incident-response plan, third-party risk management), and **12+ months** (cloud migration, 24/7 SOC monitoring, recurring penetration testing). Estimated total investment **$1.5–2M over 18 months** for **>80% risk reduction** and full compliance — framed against an average financial-sector breach cost of **$5.9M**.

## What I Learned
This was the clearest link between the security concepts I study and how they land in a real environment: mapping findings to specific GLBA/PCI DSS requirements, prioritizing by business risk rather than technical severity alone, and translating all of it into a costed, executive-ready roadmap with an ROI argument. The presentation to industry judges was practice at communicating security risk to a mixed technical/business audience, which is the core of GRC and audit work.

## Related
- Sec+ domains: 5 (Program Management & Oversight), 4 (Security Operations)
- Frameworks: NIST CSF, GLBA, PCI DSS v4.0
- See also: [[_index|Labs index]] · [[../Concepts/Cert Roadmap|Cert Roadmap]]
