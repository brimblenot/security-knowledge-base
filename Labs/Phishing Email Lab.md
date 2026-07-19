---
title: Phishing Email Lab
date: 
tags: [lab, social-engineering, phishing]
tools: []
domain: 2 - Threats, Vulnerabilities & Mitigations
course: CIS 425 (Team 4)
---

# Phishing Email Lab

## Objective
Craft a realistic phishing email to understand attacker techniques, then analyze how to detect and mitigate phishing.

## Environment / Setup
- Course: CIS 425 (group lab / in-class, Team 4)
- Artifacts: `CIS 425 Phishing Email Lab 1.docx`, `9-11 PhishEmail In-Class Assignment.docx`

## The crafted phish (themed example)
A fake "Avengers Regional Medical Center" email to Steve Rogers claiming urgent test results, using:
- **Authority** — signed by a "Dr." / medical center.
- **Urgency** — "review within 24 hours may delay treatment."
- **Lookalike domain** — `avengers-medical-secure.com` login and reset links.
- **Credential harvesting** — links to a fake login/reset page.

## Detection & mitigation (our analysis)
- Verify **link metadata is consistent with the real company** — hover before clicking.
- Check whether the email makes **logical sense** (one lure said the password was expired but asked to keep the current password — a tell).
- Treat every email as phishing until proven safe.
- **AI-driven Intrusion Prevention Systems** can flag suspicious traffic patterns, malicious domains, and credential-harvesting sites in real time, blocking connections and disrupting exfiltration — a layer beyond user education.

## What I Learned
Phishing works on psychology (authority + urgency), not technical exploits. Detection combines human skepticism with technical controls (URL scanning, IPS, email filtering). Building the lure myself made the red flags much easier to recognize as a defender.

## Related
- Sec+ domain 2: social engineering, phishing
- See also: [[Lab 2 - SET Social Engineering Toolkit]]
