# 4. Remediation & Treatment Plan Tracker

This artifact tracks the remediation plan with a **Cost-Benefit Analysis** to justify security spending to management and the Board of Directors.

## Cost-Benefit Context
*   **Cost of Inaction (Breach):** A successful Business Email Compromise (BEC) or employee credential theft costs organizations an average of **$50,000 - $100,000+** in incident response, legal fees, and regulatory fines (GDPR Article 32).
*   **Cost of Remediation:** Implementing DMARC `p=reject` is a configuration change. The cost is usually **< $200** in consulting or engineering time.

| Priority | Finding | Remediation Action | Assigned To | Due Date | Remediation Cost (Effort) | Cost of Inaction | Status |
|:---:|:---|:---|:---|:---:|:---|:---|:---|
| **P1** | **Absent DMARC Policy** | 1. Configure DMARC to `p=reject` (Quarantine/Reject).<br>2. Ensure SPF/DKIM pass before DMARC enforcement. | Security Engineer | **Immediate** | **~$200** (1 Engineer hour, DNS update) | **~$100,000** (BEC/Fraud lawsuit) | Not Started |
| **P2** | **IOC Blocking** | 1. Add IP `109.202.24.52` and domain `54upr.rosreestr.ru` to the email gateway blocklist.<br>2. Add to Perimeter Firewall blacklist. | Email Admin | 24 hrs | **~$100** (Admin time) | **~$50,000** (Future breach) | In Progress |
| **P2** | **User Security Awareness** | 1. Add "Email Header/Reply-To" scam recognition module to mandatory annual training.<br>2. Run a simulated phishing campaign replicating this 419 scam pattern. | HR / Security Team | 30 Days | **~$1,000** (External training vendor or internal setup) | **~$20,000** (Remedial fines and time) | Not Started |

## Budget Justification Summary
The **P1** and **P2** remediation actions represent a total estimated investment of **~$1,300**. 
**GRC Recommendation:** Immediate funding is requested for the DMARC DNS update to eliminate the highest residual brand and financial fraud risk.
