# SOC Lab 02 - Brute Force Investigation

## Lab Type
Defensive SOC Training Lab

## Incident Summary
Multiple failed login attempts were detected against the admin account.

The source IP 192.168.1.77 generated 8 failed login attempts within a short period.

A successful login from the same source was later observed, followed by access to and download of an employee data file.

## Evidence
- Target account: admin
- Source IP: 192.168.1.77
- Failed login attempts: 8
- Successful login: Yes
- File accessed: employees-data.xlsx
- File downloaded: employees-data.xlsx

## Initial Severity
Medium

The repeated failed login attempts indicated a possible brute-force attempt, but there was initially no evidence of successful access.

## Escalated Severity
High

The severity was increased after a successful login from the same IP and subsequent activity involving employee data.

## Investigation
The activity requires further investigation to determine whether the admin account was compromised and whether the actions were authorized.

## Containment
- Escalate the incident.
- Verify the activity with the legitimate account owner.
- Secure the admin account according to organizational procedures.
- Terminate or isolate suspicious sessions when authorized.
- Preserve relevant logs and evidence.
- Review subsequent activity associated with the account and source IP.

## Conclusion
The sequence of repeated failed logins, successful authentication, and subsequent file activity represents highly suspicious behavior requiring investigation and containment.

This is a simulated defensive SOC training lab. No real organization or production system was targeted.
