# Case Studies – Penetration Testing

## Case Study 1: Targeted Web App RCE (Hypothetical)
- **Scenario:** An organization runs a legacy web application with an insecure file upload endpoint.
- **Root Cause:** Lack of file type validation and unsafe file handling.
- **Impact:** Remote code execution (RCE) allowing attacker to run commands on the server.
- **Remediation:** Enforce strict file-type checks, sanitize filenames, store uploads outside webroot, apply least privilege to file storage.

---

## Case Study 2: Misconfigured S3 Bucket (Realistic Pattern)
- **Scenario:** Sensitive backups stored in an S3 bucket with public read permission.
- **Root Cause:** Incorrect bucket ACL and missing automated policy checks.
- **Impact:** Exposure of sensitive data, potential compliance violations.
- **Remediation:** Apply least-privilege IAM policies, enable MFA delete, enable bucket-level logging and alerts, audit S3 permissions regularly.

---

## Case Study 3: Weak Credential Reuse (Common)
- **Scenario:** Compromised developer GitHub credentials reused across cloud console.
- **Root Cause:** Hardcoded credentials and no MFA.
- **Impact:** Unauthorized access to cloud resources and data exfiltration.
- **Remediation:** Enforce MFA, use secrets management (Vault/Secrets Manager), scan repos for secrets, rotate credentials after incidents.

---

## Case Study 4: SQL Injection in Public-Facing Form (Classic)
- **Scenario:** Search/filter form concatenates user input into SQL queries.
- **Root Cause:** Missing parameterized queries and input validation.
- **Impact:** Data exfiltration and possible privilege escalation.
- **Remediation:** Use parameterized queries / prepared statements, implement input validation and least-privilege DB accounts.
