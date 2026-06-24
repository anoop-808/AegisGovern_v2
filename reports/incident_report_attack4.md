# Incident Report – Attack 4: Privilege Escalation

## Severity

Critical

## Incident Metrics

Detection Time: 2 Minutes

Investigation Time: 8 Minutes

Containment Time: 2 Minutes

Incident Status: Resolved

## Incident Summary

A contractor account was intentionally assigned the User Administrator role to simulate privilege escalation.

## Affected User

- User: Contractor User

## Evidence

- user_before_assignment.png
- user_administrator_role_empty.png
- user_admin_role_assigned.png
- contractor_elevated_access.png
- audit_log_role_assignment.png
- role_removed_remediation.png
- audit_log_role_removal.png

## Impact

Unauthorized administrative privileges could enable account manipulation and identity compromise.

## Detection

Role assignment activity was identified in Entra ID audit logs.

## Response

- Role assignment reviewed.
- Administrative privilege removed.
- Audit logs validated remediation.

## Lessons Learned

Least privilege principles must be enforced and privileged role assignments monitored continuously.
