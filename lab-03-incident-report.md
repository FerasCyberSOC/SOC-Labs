# SOC Lab 03 - Suspicious User Activity Investigation

## Lab Type
Defensive SOC Training Lab

## Incident Summary
A successful login was observed for the user ahmad.

Shortly after login, the account accessed multiple files containing customer, employee, and financial information.

Several files were then downloaded within a short period before the account logged out.

## Evidence
- User: ahmad
- Login: Successful
- Multiple sensitive files accessed
- customers.xlsx downloaded
- employees.xlsx downloaded
- finance.xlsx downloaded
- Multiple downloads occurred within seconds
- User later denied performing the activity
- Login was associated with an unusual device

## Analysis
The successful login alone does not prove account compromise.

However, the account accessed files outside the user's expected job requirements and downloaded multiple files within a short period.

The legitimate user denied performing the activity.

The unusual device is an additional indicator of suspicious activity, but it is not by itself conclusive proof of compromise.

## Severity
High

## Response
- Escalate the incident to the appropriate security team.
- Identify the device and session associated with the activity.
- Contain the suspicious session according to organizational procedures.
- Secure the affected account.
- Preserve logs and relevant evidence.
- Continue investigation to determine the scope of the incident.

## Conclusion
Multiple indicators make this activity highly suspicious and require escalation and containment.

This is a simulated defensive SOC training lab. No real organization or production system was targeted.
