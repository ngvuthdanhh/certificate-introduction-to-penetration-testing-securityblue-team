# Penetration Test Report Template

**Prepared for:** [Client Name]  
**Prepared by:** [Your Name / Company]  
**Date:** [DD/MM/YYYY]  
**Confidentiality:** This document is confidential and intended only for the client.

---

## 1. Executive Summary
This section provides a high-level overview of the engagement. It should be written in non-technical language for management stakeholders.  
- **Overall security posture:** [e.g., Moderate risk, 3 critical findings]  
- **Key strengths observed:** [e.g., Proper firewall segmentation, strong password policies]  
- **Major risks identified:** [Summarize top 3 critical vulnerabilities]  

---

## 2. Scope
Define the scope clearly.  
- **In-scope targets:**  
  - Domains: [example.com]  
  - IP ranges: [192.168.1.0/24]  
  - Applications: [Web Portal, Mobile API]  

- **Out-of-scope targets:**  
  - [List any excluded systems]  

- **Testing period:** [Start Date] – [End Date]  

---

## 3. Methodology
Outline the approach taken.  
- **Reconnaissance:** OSINT, network scanning, enumeration  
- **Vulnerability Analysis:** Automated + manual testing  
- **Exploitation:** Attempted to exploit identified vulnerabilities  
- **Post-Exploitation:** Privilege escalation, lateral movement (if allowed)  
- **Reporting:** Documented findings and recommendations  

---

## 4. Findings
Each finding should be documented as follows:

### Finding #[ID]: [Title of Vulnerability]  
- **Severity:** [Critical / High / Medium / Low]  
- **Affected Assets:** [IP/Domain/Application]  
- **Description:** Clear explanation of the issue  
- **Impact:** What happens if exploited  
- **Evidence:** Screenshots, payloads, tool outputs  
- **Recommendation:** Concrete remediation steps  

---

## 5. Risk Rating Matrix
| Severity | CVSS Score | Business Impact | Description |
|----------|------------|-----------------|-------------|
| Critical | 9.0–10.0   | Very High       | Immediate risk of compromise |
| High     | 7.0–8.9    | High            | Serious impact, needs urgent fix |
| Medium   | 4.0–6.9    | Moderate        | Potential compromise, should fix |
| Low      | 0.1–3.9    | Low             | Minor issue, defense-in-depth |

---

## 6. Remediation Roadmap
| Priority | Finding | Recommended Fix | Owner | Timeline |
|----------|---------|-----------------|-------|----------|
| Critical | SQL Injection | Use parameterized queries | Dev Team | 1 week |
| High     | Weak TLS Config | Enable TLS 1.2+ | Infra Team | 2 weeks |

---

## 7. Conclusion
Summarize the overall security health, key risks, and next steps. Highlight that remediation + retesting will significantly improve security posture.  

---

## 8. Appendix
- Tool versions used (e.g., Nmap 7.94, Burp Suite Pro 2025.1)  
- References (CVE, OWASP Top 10, CWE IDs)  
- Glossary of terms  
