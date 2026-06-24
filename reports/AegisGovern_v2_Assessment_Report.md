# AegisGovern_v2 - Identity Security Assessment Report

## Executive Summary

AegisGovern_v2 is a Microsoft Entra ID identity security laboratory designed to simulate common identity-based attack scenarios and corresponding SOC investigation workflows.

The project demonstrates identity attack detection, privilege management, audit log analysis, incident response, and security remediation within a cloud identity environment.

---

## Risk Summary

| Attack Scenario | Severity |
|----------------|----------|
| OAuth Consent Abuse | High |
| Dormant Account Abuse | Medium |
| Excessive Permissions & Information Exposure | Medium |
| Privilege Escalation via Role Assignment | Critical |

---

## Environment

- Microsoft Entra ID Tenant
- User Accounts
- Groups
- Administrative Roles
- Authentication Controls
- Audit Logs
- Sign-In Logs

---

## Attack Scenarios Performed

## MITRE ATT&CK Coverage

| Attack Scenario | MITRE Technique | Technique ID |
|----------------|----------------|-------------|
| OAuth Consent Abuse | Steal Application Access Token | T1528 |
| Dormant Account Abuse | Valid Accounts: Cloud Accounts | T1078.004 |
| Excessive Permissions & Information Exposure | Account Discovery: Cloud Account | T1087.004 |
| Privilege Escalation via Role Assignment | Account Manipulation: Additional Cloud Roles | T1098.003 |

---

### Attack 1 - OAuth Consent Abuse

Affected User:
- Priya Finance

Result:
- Suspicious application identified
- Permission review completed
- User consent controls validated

---

### Attack 2 - Dormant Account Abuse

Affected User:
- John Former

Result:
- Dormant account identified
- Account disabled
- Access blocked

---

### Attack 3 - Excessive Information Exposure

Affected User:
- Intern User

Result:
- User enumeration performed
- Group visibility reviewed
- Role visibility reviewed

---

### Attack 4 - Privilege Escalation

Affected User:
- Contractor User

Result:
- User Administrator role assigned
- Elevated access verified
- Audit logs reviewed
- Privileges removed

---

## Security Findings

### High Risk

- Excessive administrative role assignment

### Medium Risk

- Dormant account exposure

### Low Risk

- Excessive directory visibility

---

## Lessons Learned

### OAuth Consent Abuse

- User consent can introduce significant identity risk.
- Application permissions should be reviewed before approval.
- User consent policies should be restricted.

### Dormant Account Abuse

- Former employee accounts increase attack surface.
- Regular identity reviews are essential.
- Account lifecycle management should be enforced.

### Excessive Information Exposure

- Low-privileged users should not have unnecessary visibility.
- Directory information can support attacker reconnaissance.
- Least privilege principles should be continuously reviewed.

### Privilege Escalation

- Administrative role assignments must be monitored.
- Audit logs provide critical investigation evidence.
- Privileged access should be reviewed regularly.

---

## Detection Gaps & Future Improvements

### Gap 1 - Automated Alerting

Current State:
Role assignment activity required manual review.

Improvement:
Implement automated alerts for privileged role assignments.

### Gap 2 - OAuth Monitoring

Current State:
OAuth application review was manual.

Improvement:
Create alerts for new application registrations and permission grants.

### Gap 3 - Dormant Account Detection

Current State:
Inactive accounts were identified through review.

Improvement:
Automate dormant account identification and reporting.

### Gap 4 - Identity Visibility Monitoring

Current State:
User enumeration activities were manually observed.

Improvement:
Implement monitoring for unusual identity discovery activity.

---

## Recommendations

1. Enforce least privilege access.
2. Review dormant accounts regularly.
3. Monitor privileged role assignments.
4. Restrict application consent permissions.
5. Perform periodic access reviews.

---

## Conclusion

The assessment successfully demonstrated identity-focused attack simulations and SOC investigation workflows using Microsoft Entra ID. The project highlights common identity risks and the defensive processes required to detect, investigate, and remediate them.
