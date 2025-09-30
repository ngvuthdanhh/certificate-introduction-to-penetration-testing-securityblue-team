# Penetration Testing Checklist

This checklist ensures consistency and completeness across penetration testing engagements.

---

## 1. Pre-Engagement
- [ ] Define engagement scope  
- [ ] Obtain written authorization  
- [ ] Identify in-scope assets (domains, IPs, APIs)  
- [ ] Clarify legal & compliance boundaries  
- [ ] Establish communication channels  

---

## 2. Reconnaissance
- [ ] Perform passive recon (WHOIS, DNS records, Shodan)  
- [ ] Gather subdomains (Sublist3r, Amass)  
- [ ] Map network ranges and open services (Nmap, Masscan)  
- [ ] Identify technologies used (Wappalyzer, WhatWeb)  

---

## 3. Vulnerability Analysis
- [ ] Check for outdated software & services  
- [ ] Scan for common CVEs (Nessus/OpenVAS/Nmap scripts)  
- [ ] Look for misconfigurations (default creds, directory listing)  
- [ ] Assess authentication & session handling  

---

## 4. Exploitation
- [ ] Test for SQL Injection  
- [ ] Test for XSS (stored/reflected)  
- [ ] Test for CSRF  
- [ ] Test for insecure file upload  
- [ ] Check access controls (horizontal & vertical privilege escalation)  

---

## 5. Post-Exploitation
- [ ] Attempt privilege escalation  
- [ ] Check data exfiltration paths  
- [ ] Identify persistence mechanisms  
- [ ] Verify lateral movement opportunities  

---

## 6. Reporting
- [ ] Draft executive summary (non-technical)  
- [ ] Document each finding with evidence & remediation  
- [ ] Assign risk ratings (Critical/High/Medium/Low)  
- [ ] Provide remediation roadmap  
- [ ] Peer-review report for accuracy  
