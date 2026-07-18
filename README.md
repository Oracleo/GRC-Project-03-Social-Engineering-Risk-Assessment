# Social Engineering Risk Assessment & Incident Reporting | Email Forensics

![MITRE ATT&CK](https://img.shields.io/badge/MITRE-ATT%26CK%20T1566-red?style=for-the-badge&logo=mitre&logoColor=white)
![Threat Intel](https://img.shields.io/badge/Threat%20Intelligence-VirusTotal%20%7C%20AbuseIPDB%20%7C%20WHOIS-blue?style=for-the-badge)
![Status](https://img.shields.io/badge/Status-Completed-28A745?style=for-the-badge)
![Framework](https://img.shields.io/badge/Framework-ISO%2027001%20%7C%20NIST%20CSF-0057A8?style=for-the-badge)
![Classification](https://img.shields.io/badge/Classification-Phishing%20%7C%20Medium%20Severity-orange?style=for-the-badge)

**A structured social engineering risk assessment and incident investigation based on a live phishing email.** 
This project demonstrates the full lifecycle of a GRC/SOC incident—from email header analysis, SPF/DKIM/DMARC authentication verification, and IOC extraction, to threat intelligence enrichment (VirusTotal, AbuseIPDB, WHOIS), and a formal audit-grade incident report with business impact analysis.

---

## Project at a Glance (For Recruiters & Hiring Managers)

| Area | Details |
|:---|:---|
| **Incident Type** | Advance Fee Fraud (419 Scam) via Phishing |
| **MITRE ATT&CK** | T1566 - Phishing (Spearphishing via Service) |
| **Key Findings** | SPF Fail, DKIM None, DMARC None, Gmail Reply-To mismatch. |
| **Automated Tool Insight** | VirusTotal showed **0/93 detections** (Critical False Negative) - proving manual GRC investigation is essential. |
| **Third-Party Risk** | Relayed through a compromised subdomain of a legitimate Russian government entity (`54upr.rosreestr.ru`). |
| **Frameworks Mapped** | ISO 27001 (A.6.3, A.5.24), NIST CSF (DE.CM-3, RS.AN-1, PR.AT-1). |

---

## Repository Contents

Navigate this repository to view the formal GRC artifacts:

| Document | Description |
|:---|:---|
| **`docs/01-Executive-Summary.md`** | A non-technical summary for senior leadership detailing the phishing attempt and strategic control recommendations. |
| **`docs/02-Scope-Methodology.md`** | The formal Terms of Reference for the email forensics investigation. |
| **`docs/03-Risk-Register.md`** | A formalized risk register entry for the phishing incident and the organizational control gap. |
| **`docs/04-Remediation-Tracker.md`** | A project management artifact tracking the implementation of DMARC, user training, and IOC blocking. |
| **`docs/05-Compliance-Gap-Analysis.md`** | A control-by-control analysis mapping the incident to ISO 27001, NIST CSF, and GDPR. |
| **`docs/06-Asset-Business-Criticality.md`** | Contextualizing the email system as a critical business asset holding financial/PII data. |
| **`docs/07-MITRE-ATTACK-Mapping.md`** | Detailed mapping of the attacker's chain of actions and MITRE mitigations. |
| **`artifacts/`** | Raw forensic evidence including the `.eml` file, raw headers, IOC lists, and threat intelligence logs. |
| **`screenshots/`** | 8 annotated screenshots documenting the header analysis, SPF failure, and threat intel platforms. |

---
