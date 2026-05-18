# Section C — Security Validation and Vulnerability Assessment

# Q3. Structural Vulnerability Examination using OWASP ZAP

## Scenario
A web application must be validated against common structural vulnerabilities before deployment.

---

# 1. Importance of Security-Oriented Validation

Security-oriented validation ensures software systems are protected against attacks, unauthorized access, and data breaches before deployment.

Security validation helps:
- identify vulnerabilities early,
- protect sensitive information,
- improve software reliability,
- reduce cyberattack risks,
- support compliance requirements.

---

# 2. Common Vulnerabilities

## SQL Injection

### Description
SQL Injection occurs when attackers insert malicious SQL queries into application input fields.

### Impact
- Unauthorized database access
- Data leakage
- Database manipulation

### Example

```sql
' OR '1'='1
```

---

## Cross-Site Scripting (XSS)

### Description
XSS occurs when malicious scripts are injected into web pages viewed by users.

### Impact
- Session hijacking
- Cookie theft
- Unauthorized actions

### Example

```html
<script>alert('Hacked')</script>
```

---

## Broken Authentication

### Description
Broken authentication occurs when authentication mechanisms are weak or improperly configured.

### Impact
- Unauthorized access
- Identity theft
- Account compromise

### Common Causes
- Weak passwords
- Missing MFA
- Poor session management

---

# 3. OWASP ZAP Vulnerability Assessment Workflow

## Step 1 — Configure Target

- Open OWASP ZAP
- Enter target URL
- Configure browser proxy

Example target:

```text
http://testphp.vulnweb.com
```

---

## Step 2 — Passive Scanning

Passive scanning analyzes application traffic without attacking the target system.

Checks include:
- Missing security headers
- Cookie vulnerabilities
- Information disclosure

Advantages:
- Safe
- No application damage

---

## Step 3 — Active Scanning

Active scanning actively attacks the application to identify vulnerabilities.

Checks include:
- SQL Injection
- Cross-Site Scripting
- Broken authentication

Procedure:
- Right-click target
- Select:
  
```text
Attack → Active Scan
```

---

## Step 4 — Risk Classification

OWASP ZAP classifies vulnerabilities based on severity.

| Severity | Description |
|---|---|
| High | Critical vulnerability |
| Medium | Significant security issue |
| Low | Minor vulnerability |
| Informational | Security recommendation |

---

## Step 5 — Validation Evidence Generation

Generate reports using:

```text
Report → Generate HTML Report
```

Generated evidence includes:
- scan reports,
- vulnerability details,
- screenshots,
- logs,
- affected URLs.

---

# Vulnerability Severity Table

| Vulnerability | Severity | Impact | Recommendation |
|---|---|---|---|
| SQL Injection | High | Database compromise | Use prepared statements |
| XSS | Medium | Session theft | Input sanitization |
| Missing Security Headers | Low | Weak browser protection | Configure secure headers |

---

# Mitigation Recommendations

| Vulnerability | Mitigation |
|---|---|
| SQL Injection | Parameterized queries |
| XSS | Input/output encoding |
| Broken Authentication | Multi-factor authentication |
| Sensitive Data Exposure | Data encryption |
| Security Misconfiguration | Secure server configuration |

---

# Expected Deliverables

- ZAP scan report
- Vulnerability severity table
- Evidence screenshots
- Validation logs
- Mitigation recommendations

---

# Conclusion

OWASP ZAP helps identify structural vulnerabilities before deployment and supports secure software validation and compliance activities.
