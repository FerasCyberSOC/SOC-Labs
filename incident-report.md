# SOC Incident Report - Lab 01

## Lab Type
Defensive SOC Training Lab

## Incident Summary
Three failed login attempts were detected on the admin account.
A successful login then occurred from the same source IP.
Shortly afterward, a new account named newadmin was created.

## Evidence
- User: admin
- Source IP: 192.168.1.50
- Failed login attempts: 3
- Successful login: Yes
- New account created: newadmin

## Analysis
The failed login attempts could initially have been caused by an employee entering an incorrect password.

However, the successful login followed by the creation of a new account increased the level of suspicion.

The incident should be investigated to determine whether the activity was authorized.

## Severity
High

## Response
- Escalate the incident for further investigation.
- Verify whether the new account was authorized.
- Secure the admin account if compromise is confirmed.
- Disable the unauthorized new account according to the organization's incident-response procedures.
- Review active sessions and preserve relevant logs.

## Conclusion
The activity was classified as highly suspicious because multiple failed login attempts were followed by a successful login and the creation of a new account.

This is a simulated defensive SOC training lab. No real organization or production system was targeted.
