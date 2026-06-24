# AegisGovern_v2 - Cloud Identity Security & SOC Investigation Lab

## Overview

AegisGovern_v2 is a Microsoft Entra ID based identity security lab designed to simulate real-world identity attacks, privilege abuse scenarios, and SOC investigation workflows.

The project focuses on Identity and Access Management (IAM), privilege management, audit log analysis, attack detection, incident response, and security remediation within a cloud identity environment.

---

## Objectives

* Build a realistic Microsoft Entra ID lab environment
* Create users, groups, and administrative roles
* Simulate identity-based attack scenarios
* Investigate attacks using audit and sign-in logs
* Document findings using SOC-style incident reports
* Demonstrate identity security and governance concepts

---

## Environment

### Identity Platform

* Microsoft Entra ID

### Components

* Users
* Groups
* Administrative Roles
* Authentication Controls
* Audit Logs
* Sign-In Logs

---

## Attack Scenarios

---

## MITRE ATT&CK Mapping

| Attack Scenario | MITRE Technique | Technique ID |
|----------------|----------------|-------------|
| OAuth Consent Abuse | Steal Application Access Token | T1528 |
| Dormant Account Abuse | Valid Accounts: Cloud Accounts | T1078.004 |
| Excessive Permissions & Information Exposure | Account Discovery: Cloud Account | T1087.004 |
| Privilege Escalation via Role Assignment | Account Manipulation: Additional Cloud Roles | T1098.003 |

---

## Risk Severity Classification

| Attack Scenario | Severity |
|----------------|----------|
| OAuth Consent Abuse | High |
| Dormant Account Abuse | Medium |
| Excessive Permissions & Information Exposure | Medium |
| Privilege Escalation via Role Assignment | Critical |

---
### Attack 1 - OAuth Consent Abuse

**Affected User:** Priya Finance

**MITRE ATT&CK:** T1528 - Steal Application Access Token

Simulated a malicious OAuth application requesting delegated permissions through a fake rewards portal.

**Skills Demonstrated**

* OAuth Security
* Application Permission Review
* Audit Log Analysis
* Sign-In Log Investigation

**Evidence**

`evidence/attack1_oauth_consent`

![Attack 1](images/attack1_preview.png)

---

### Attack 2 - Dormant Account Abuse

**Affected User:** John Former

**MITRE ATT&CK:** T1078.004 - Valid Accounts: Cloud Accounts

Simulated risks associated with inactive employee accounts remaining in the environment after departure.

**Skills Demonstrated**

* Identity Lifecycle Management
* Account Review
* Account Disablement
* Access Validation

**Evidence**

`evidence/attack2_dormant_account`

![Attack 2](images/attack2_preview.png)

---

### Attack 3 - Excessive Permissions & Information Exposure

**Affected User:** Intern User

**MITRE ATT&CK:** T1087.004 - Account Discovery: Cloud Account

Demonstrated how a low-privileged account could enumerate users, groups, and directory information.

**Skills Demonstrated**

* Identity Reconnaissance
* Permission Analysis
* Directory Enumeration
* Access Review

**Evidence**

`evidence/attack3_excessive_permissions`

![Attack 3](images/attack3_preview.png)

---

### Attack 4 - Privilege Escalation via Role Assignment

**Affected User:** Contractor User

**MITRE ATT&CK:** T1098.003 - Account Manipulation: Additional Cloud Roles

Simulated unauthorized assignment of the User Administrator role and investigated the resulting privilege escalation.

**Skills Demonstrated**

* Privileged Identity Management
* Role Assignment Analysis
* Audit Log Investigation
* Privilege Remediation

**Evidence**

`evidence/attack4_privilege_escalation`

![Attack 4](images/attack4_preview.png)

---

## Investigation Reports

The project includes SOC-style incident reports for each attack scenario:

* incident_report_attack1.md
* incident_report_attack2.md
* incident_report_attack3.md
* incident_report_attack4.md

Location:

`reports/`

---

## Final Assessment

A consolidated security assessment report is available at:

`reports/AegisGovern_v2_Assessment_Report.md`

The report summarizes:

* Attack Scenarios
* Findings
* Risk Analysis
* Detection Activities
* Remediation Actions
* Security Recommendations

---

## Skills Demonstrated

### Identity Security

* Microsoft Entra ID
* Identity Governance
* Authentication Controls
* Administrative Role Management

### Security Operations

* Incident Investigation
* Audit Log Analysis
* Sign-In Log Analysis
* Security Documentation

### Governance, Risk & Compliance

* Access Reviews
* Least Privilege
* Identity Risk Assessment
* Security Recommendations

---

## Project Structure

```text
AegisGovern_v2
├── docs
├── evidence
│   ├── attack1_oauth_consent
│   ├── attack2_dormant_account
│   ├── attack3_excessive_permissions
│   └── attack4_privilege_escalation
├── reports
└── README.md
```

## Architecture Diagram

```mermaid
flowchart TD

    A[Microsoft Entra ID Tenant]

    A --> B[Users]
    A --> C[Groups]
    A --> D[Roles]

    B --> E[Attack Simulations]
    C --> E
    D --> E

    E --> F[OAuth Consent Abuse]
    E --> G[Dormant Account Abuse]
    E --> H[Excessive Permissions]
    E --> I[Privilege Escalation]

    F --> J[Audit Logs]
    G --> J
    H --> J
    I --> J

    J --> K[Investigation]
    K --> L[Remediation]
    L --> M[Incident Reports]
```

---

## Lessons Learned

Throughout this project, several key identity security lessons were observed:

### OAuth Consent Abuse

* User consent can introduce significant identity risk.
* Third-party applications should be reviewed before approval.
* Application permissions must be continuously monitored.

### Dormant Account Abuse

* Former employee accounts increase organizational attack surface.
* Regular account lifecycle reviews are critical.
* Dormant accounts should be disabled or removed promptly.

### Excessive Information Exposure

* Excessive visibility enables attacker reconnaissance.
* Least privilege principles should be applied to directory access.
* User enumeration can support future attacks.

### Privilege Escalation

* Administrative role assignments require continuous monitoring.
* Audit logs provide valuable evidence during investigations.
* Privileged access reviews help prevent abuse.

---

## Detection Gaps & Future Improvements

### Current Gaps

* OAuth consent activity required manual review.
* Dormant account discovery relied on periodic assessment.
* Privilege escalation detection depended on audit log investigation.
* Identity reconnaissance activities lacked automated alerting.

### Future Improvements

* Implement automated alerting for privileged role assignments.
* Monitor OAuth application registrations and consent grants.
* Automate dormant account identification.
* Improve visibility into identity reconnaissance activity.
* Integrate Entra ID logs with a SIEM platform for continuous monitoring.

---

## Author

**B. Giri Anoop**

Cloud Identity Security Researcher | SOC Analyst Aspirant

Focused on Microsoft Entra ID, Identity Governance, Incident Investigation, Audit Log Analysis, Identity Threat Detection, and Cloud Security.
