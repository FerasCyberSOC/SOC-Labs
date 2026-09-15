# SOC Lab 05 - Alert Triage Casebook

## Lab Type
Defensive SOC Training Lab

## Objective
Practice SOC alert triage and distinguish between:
- True Positive
- False Positive
- Needs Investigation

---

## Case 1 - Failed Login Attempts

User: sara
Failed Attempts: 6
Severity: Medium

### Investigation
The user confirmed that she forgot her password.
The IT team reset the password and no additional suspicious activity was detected.

### Decision
False Positive

---

## Case 2 - Suspicious Admin Login

User: admin
Source IP: 10.0.0.88
Failed Attempts: 15

A successful login occurred after the failed attempts.
A new administrator account was then created.

The legitimate administrator confirmed that the activity was unauthorized.

### Decision
True Positive

### Response
Escalate the incident and begin appropriate containment procedures.

---

## Case 3 - Large Backup Download

User: khaled
File: company-backup.zip
Size: 8 GB
Time: 02:15 AM

### Investigation
The user was responsible for backups.
A scheduled backup operation was authorized for this time.

### Decision
False Positive

---

## Case 4 - Unusual Account Activity

User: mohammed
Login Time: 03:40 AM
Device: New Device

Additional events:
- finance.xlsx accessed
- finance.xlsx downloaded
- MFA disabled

The legitimate user denied performing the activity.

### Decision
True Positive

### Response
Escalate the incident, begin containment according to organizational procedures, and preserve evidence.

---

## Case 5 - Malware Detection

Device: PC-FINANCE-04
User: ali
File: invoice_update.exe

The security system detected known malware and quarantined the file.

Further investigation showed:
- The file was executed.
- The process initiated an outbound network connection.
- The malware was subsequently quarantined.

### Decision
True Positive

### Response
- Escalate the incident.
- Preserve relevant evidence.
- Contain the affected device according to organizational procedures.
- Investigate the external connection.
- Review additional activity on the affected device.

## Key Lessons

- An alert does not automatically prove compromise.
- Context is important during alert triage.
- False positives should be documented.
- Suspicious activity may require additional investigation before classification.
- Confirmed malicious activity should be escalated.
- Evidence should be preserved during incident investigation.

## Disclaimer

This is a simulated defensive SOC training lab.
No real organization or production system was targeted.
