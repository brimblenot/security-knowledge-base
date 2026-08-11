---
title: Cert Roadmap
tags: [certs, planning]
---

# Certification Roadmap

Path toward **security engineer + cloud security/cloud engineer** roles. Certs get interviews; pair each one with a hands-on lab or project to actually land the role.

## Sequence

1. **CompTIA Security+ (SY0-701)** — ✅ done (baseline; meets DoD 8570 IAT II)
2. **AWS Certified Solutions Architect – Associate (SAA-C03)** — 🔄 **in progress (currently studying).** The anchor cloud cert; broad and recruiter-recognized. *(Skip Cloud Practitioner — see note below.)*
3. **Cisco CCNA** — 🔄 **in progress (currently studying, in parallel).** Solid networking foundation with double value in the cleared/network-adjacent market (DMV/DoD). Pairs well with the security + cloud track by grounding the networking fundamentals both rely on.
4. **HashiCorp Terraform Associate** — cheap, fast, high-ROI. Infrastructure-as-Code is the skill that defines modern cloud/security engineering. Slot in during/after SAA.
5. **AWS Certified Security – Specialty** — the differentiator that fuses cloud + security into "cloud security engineer." Do after AWS grounding from SAA.
6. **CISSP** — *long-term (3–5 yrs).* Architecture/management credibility; needs ~5 yrs experience (can pass early and hold Associate of ISC2 until qualified).

## Cloud Practitioner — skip it
CCP is foundational, aimed at people with **zero** cloud exposure. With a CIS degree, cloud coursework (EC2/IAM), and Security+ already, it's a redundant résumé line that SAA fully supersedes. **Learn the CCP content as a free ~1-week warm-up, but don't sit the exam** — go straight to SAA.

## Pair every cert with an artifact
- After **SAA** → deploy a real app on AWS; document the architecture.
- After **Security Specialty** → secure that deployment (least-privilege IAM, CloudTrail, GuardDuty) and write it up like the [SOC lab](../Labs/_index.md).
- **Terraform** → provision the above with IaC, security controls baked in.

## Notes
- **Vendor:** stick with **AWS** (market leader; matches my coursework). Only pivot to Azure for Microsoft-shop / certain gov roles (some DoD leans Azure Gov / AWS GovCloud).
- Verify current exam codes on aws.amazon.com/certification before booking — versions update periodically.

> Full phased career plan lives in the career roadmap. High-level: Security+ ✅ → AWS SAA + CCNA (both in progress) → Terraform → AWS Security Specialty, with CISSP later.
