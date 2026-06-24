# Attack Mapping

## Attack 1 - OAuth Consent Abuse
Affected User: Priya Finance
Attack Type: Malicious OAuth Application Consent
Evidence Folder: evidence/attack1_oauth_consent

## Attack 2 - Dormant Account Abuse
Affected User: John Former
Attack Type: Dormant / Former Employee Account
Evidence Folder: evidence/attack2_dormant_account

## Attack 3 - Excessive Information Exposure
Affected User: Intern User
Attack Type: Excessive Visibility and Enumeration
Evidence Folder: evidence/attack3_excessive_permissions

## Attack 4 - Privilege Escalation
Affected User: Contractor User
Attack Type: Excessive Administrative Role Assignment
Evidence Folder: evidence/attack4_privilege_escalation

# MITRE ATT&CK Mapping

| Attack | MITRE Technique | Technique ID |
|----------|----------|----------|
| OAuth Consent Abuse | Steal Application Access Token | T1528 |
| Dormant Account Abuse | Valid Accounts: Cloud Accounts | T1078.004 |
| Excessive Permissions & Information Exposure | Account Discovery: Cloud Account | T1087.004 |
| Privilege Escalation via Role Assignment | Account Manipulation: Additional Cloud Roles | T1098.003 |

## Coverage Summary

This project demonstrates multiple cloud identity attack techniques mapped to the MITRE ATT&CK framework.

Focus Areas:

- Initial Access
- Valid Accounts
- Account Discovery
- Privilege Escalation
- Identity Abuse
- Cloud Security Monitoring
- Incident Investigation
