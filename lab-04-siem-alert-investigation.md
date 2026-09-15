# SOC Lab 04 - SIEM Alert Investigation

## Lab Type
Defensive SOC Training Lab

## Alert Triage
- Alert ID: 1047
- Initial Severity: Medium
- Rule: Multiple Failed Login Attempts
- Username: administrator
- Source IP: 10.0.0.45
- Destination IP: 10.0.0.10
- Failed Attempts: 12
- Time Window: 45 seconds

## Investigation
The SIEM detected 12 failed login attempts within 45 seconds.

A successful login was then observed from the same source IP.

Shortly after the successful login, a new administrative account named backup-admin was created.

The legitimate administrator confirmed that the new account was not authorized.

## Severity
High

The alert was escalated from Medium to High because the investigation identified:
- Multiple failed authentication attempts
- Successful authentication from the same source
- Creation of an unauthorized administrator account

## Response
- Escalate the incident to the appropriate security team.
- Contain the suspicious session according to organizational procedures.
- Secure the administrator account.
- Disable or restrict the unauthorized backup-admin account when authorized.
- Preserve SIEM logs and other relevant evidence.
- Continue investigating activity associated with the source IP and affected accounts.

## Conclusion
The alert required escalation and containment because multiple suspicious authentication events were followed by unauthorized administrative account creation.

This is a simulated defensive SOC training lab. No real organization or production system was targeted.
