---
title: Project Backlog
tags: [planning, labs, projects]
---

# 🎯 Project Backlog — Hands-On Labs to Pursue

Future home-lab projects to build out skills and resume, beyond the current [[_index|labs]] and the [SOC lab on GitHub](https://github.com/brimblenot/soc-home-lab). Each one pairs with the [[../Concepts/Cert Roadmap|cert roadmap]] — certs get interviews, projects land the role.

Source of the shortlist: Artem Polynko's "SOC Analyst — 10 Hands-On Projects" guide; filtered to remove anything already done or planned.

## Already covered / planned — not repeated here
- **SIEM Log Monitoring & Threat Detection** → ✅ done — the Wazuh [SOC lab](https://github.com/brimblenot/soc-home-lab) (M0–M4: SIEM, endpoint, Kali attack, custom detection rule).
- **Endpoint Monitoring with Sysmon + Wazuh** → planned — the deferred Windows endpoint on the SOC lab roadmap (add Win10 VM + Sysmon).
- **IDS Deployment & Packet Analysis (Snort/Suricata)** → planned — SOC lab stretch goal (Suricata forwarded into Wazuh).
- **Cloud Security Monitoring (AWS/Azure logs)** → planned — the AWS cert artifact in the [[../Concepts/Cert Roadmap|Cert Roadmap]] (CloudTrail/GuardDuty after AWS Security Specialty).

## Backlog

### 1. Simulated Phishing Attack & Incident Response
Recreate a phishing → malware scenario end to end, then investigate it from the logs as an IR exercise. *(Note: complements the existing offense-side [[Phishing Email Lab]] — this one is the blue-team/IR side.)*
- **Skills:** incident response, log analysis, attack-chain reconstruction.
- **Tools:** GoPhish, Wazuh/SIEM, Kali, victim VM.
- **Resume value:** 8/10 · **Time:** ~10–15 hrs · **Cost:** $0.
- **Resume bullet:** "Simulated a phishing-to-malware intrusion and reconstructed the attack timeline from endpoint and email logs during a mock incident response."

### 2. Threat Hunting in Real Datasets
Hunt for attacker activity in real-world log datasets (Windows Event Logs, Zeek) using structured, hypothesis-driven queries.
- **Skills:** SPL/KQL, anomaly detection, ATT&CK mapping.
- **Tools:** Splunk / Elastic, CyberDefenders & Boss of the SOC datasets.
- **Resume value:** 8/10 · **Time:** ~10–20 hrs · **Cost:** $0.
- **Resume bullet:** "Performed threat hunting on Zeek and Windows log datasets; identified lateral movement and brute-force indicators and mapped findings to MITRE ATT&CK."

### 3. Security Automation Script (SOAR Lite)
Write a Python/PowerShell script to enrich IOCs, parse logs, or auto-tag suspicious events. *(Plays to existing strength — already build Python/AI systems; this points it at SOC automation.)*
- **Skills:** scripting, API use, automation logic.
- **Tools:** Python, VirusTotal API, AbuseIPDB, log samples.
- **Resume value:** 7/10 · **Time:** ~8–15 hrs · **Cost:** $0.
- **Resume bullet:** "Developed a Python tool to enrich IOCs via the VirusTotal and AbuseIPDB APIs and summarize alert context in JSON reports."

### 4. Honeypot Deployment & Threat Intel
Stand up a Cowrie SSH honeypot (ideally on a cheap cloud VM) to capture real attacker behavior, then analyze login attempts, dropped files, and source IPs.
- **Skills:** real attacker interaction, log analysis, OSINT enrichment.
- **Tools:** Cowrie, ELK, VirusTotal, DigitalOcean.
- **Resume value:** 7/10 · **Time:** ~15 hrs over 1–2 weeks · **Cost:** $0–$10.
- **Resume bullet:** "Deployed an SSH honeypot in a cloud VM; captured and analyzed thousands of attacker attempts including common TTPs and credential patterns, enriched with OSINT."

### 5. Threat Intelligence IOC Research
Research a malware/APT campaign, collect and enrich indicators, and write a threat brief with ATT&CK mapping.
- **Skills:** IOC research, enrichment, ATT&CK mapping, reporting.
- **Tools:** VirusTotal, AlienVault OTX, WHOIS, MISP.
- **Resume value:** 6/10 · **Time:** ~10–15 hrs · **Cost:** $0.
- **Resume bullet:** "Compiled a threat report on a malware campaign with enriched IOCs and MITRE TTP mapping, integrated with an open-source MISP instance."

### 6. Phishing Email & Malware Analysis
Analyze phishing email headers, malicious links, and malware attachments in a sandbox; extract and report IOCs. *(Defensive forensics — distinct from the offense-side [[Phishing Email Lab]].)*
- **Skills:** email forensics, malware sandboxing, IOC extraction.
- **Tools:** Any.Run, VirtualBox, VirusTotal, Wireshark.
- **Resume value:** 6/10 · **Time:** ~6–12 hrs · **Cost:** $0.
- **Resume bullet:** "Analyzed a phishing email with a malicious attachment; performed sandbox detonation, extracted downloader behavior, and mapped it to the initial-access vector."

## Suggested order
Pragmatically: **#3 (SOAR Lite)** first — fast, plays to existing scripting strength, and pairs with the Wazuh lab. Then **#2 (Threat Hunting)** and **#5 (IOC Research)** for detection/analysis depth. **#4 (Honeypot)** when up for a multi-day cloud project. **#1 and #6 (phishing IR / malware analysis)** whenever a break from the SOC lab is wanted.
