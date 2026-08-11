# Samuel Kaiser — Cybersecurity Portfolio

Aspiring cybersecurity professional (JMU CIS, cybersecurity concentration, May 2026) working toward **cloud security engineering**. This is my working portfolio spanning **security, cloud, and networking** — hands-on labs, certifications, study notes, and projects.

📍 Currently: **CompTIA Security+ ✅ certified** · studying for **AWS Solutions Architect – Associate** and **Cisco CCNA** · building a SOC/Active Directory home lab
🎯 Target: SOC / security analyst → cloud security engineer

---

## 🎓 Certifications

| Certification | Status |
|---------------|--------|
| CompTIA Security+ (SY0-701) | ✅ Certified |
| AWS Certified Solutions Architect – Associate (SAA-C03) | 🔄 In progress — studying |
| Cisco CCNA | 🔄 In progress — studying |

Full sequence and rationale in the [Cert Roadmap](Concepts/Cert%20Roadmap.md). Certs get interviews; each is paired with a hands-on lab or project to actually land the role.

---

## 🧪 Hands-on Labs

Applied security work from my coursework (CIS 425) — offensive and defensive.

| Lab | Focus | Skills demonstrated |
|-----|-------|---------------------|
| [Keylogger](Labs/Lab%201%20-%20Keylogger.md) | Malware / credential theft | Threat analysis, endpoint defense, MFA |
| [Phishing Email](Labs/Phishing%20Email%20Lab.md) | Social engineering | Lure construction, detection, IPS |
| [Metasploit + SET](Labs/Lab%202%20-%20SET%20Social%20Engineering%20Toolkit.md) | Exploitation framework | Attack chaining, EDR, incident response |
| [PGP Encryption](Labs/Lab%203%20-%20PGP%20Encryption.md) | Cryptography | Hybrid crypto, digital signatures, PKI |
| [DDoS](Labs/Lab%204%20-%20DDoS.md) | Availability attacks | Attack types, WAF, CDN mitigation |
| [Vulnerability Assessment](Labs/Lab%205%20-%20Vulnerability%20Assessment.md) | Vuln management | Scanning, triage, remediation |

> ✅ **Core lab complete:** [SOC home lab](https://github.com/brimblenot/soc-home-lab) — Wazuh SIEM monitoring a live endpoint, SSH brute force from Kali detected and MITRE ATT&CK–correlated, verified across three layers, with a custom detection rule I authored. Stretch goals (Suricata IDS, Windows AD) in progress.

---

## 🛠️ Tools & Technologies

**Security:** Wazuh (SIEM) · Suricata · Metasploit · SET · Nmap · Hydra · Nessus/vuln scanners · PGP · Kali Linux · MITRE ATT&CK
**Cloud:** AWS (EC2, IAM, VPC — studying SAA) · virtualization / VirtualBox
**Networking:** routing & switching, subnetting, network security (studying CCNA)
**Systems:** Windows / Active Directory · Linux · Bash
**Dev:** Python · Node.js · JavaScript · Git

---

## 🔗 Projects

- **[Security+ Study App](https://github.com/brimblenot/secplus-coach)** — a full-stack study app I built (Next.js) that generates AI-powered study guides and adaptive quizzes across all Sec+ domains, with weak-area tracking and progress analytics.
- **[Job Search Agent System](https://github.com/brimblenot/job-search-agent-system)** — an autonomous multi-agent system (Python) that automates job searching, analysis, resume tailoring, and outreach using Claude AI. Built with a scout/analyst/tailor/outreach agent architecture and an orchestration layer.
- **[Discord Admin Bot](https://github.com/brimblenot/discord-admin-bot)** — an AI-powered Discord bot that manages servers via natural-language commands, using Claude tool-use to create channels, roles, and permissions.
- **[SOC / SIEM Home Lab](https://github.com/brimblenot/soc-home-lab)** — a Wazuh SIEM home lab running the full attack → detect → verify pipeline: enrolled a live endpoint, launched recon + SSH brute force from Kali, detected and MITRE ATT&CK–correlated it, verified across three layers (source log → SIEM engine → dashboard), and authored a custom detection rule. Core lab (M0–M4) complete; Suricata IDS and Windows AD are stretch goals in progress.

---

## 📫 Contact
- GitHub: [brimblenot](https://github.com/brimblenot)
- LinkedIn: https://www.linkedin.com/in/samuel-thomas-kaiser/
- Email: sam.kaiser7@outlook.com
