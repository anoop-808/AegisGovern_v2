# AegisGovern_v2 - Identity Security Assessment Report

## Executive Summary

AegisGovern_v2 is a Microsoft Entra ID identity security laboratory designed to simulate common identity-based attack scenarios and corresponding SOC investigation workflows.

The project demonstrates identity attack detection, privilege management, audit log analysis, incident response, and security remediation within a cloud identity environment.

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

## Recommendations

1. Enforce least privilege access.
2. Review dormant accounts regularly.
3. Monitor privileged role assignments.
4. Restrict application consent permissions.
5. Perform periodic access reviews.

---

## Conclusion

The assessment successfully demonstrated identity-focused attack simulations and SOC investigation workflows using Microsoft Entra ID. The project highlights common identity risks and the defensive processes required to detect, investigate, and remediate them.
