# Attack 4: Privilege Escalation via Unauthorized Role Assignment

## Objective

Simulate an identity-based privilege escalation attack by assigning an administrative role to a contractor account.

## Attack Simulation

The Contractor User account was assigned the User Administrator role. This simulated a scenario where excessive privileges were granted to a non-administrative user.

## Detection

The following sources were reviewed:

* Role Assignments
* Administrative Role Membership
* Microsoft Entra Audit Logs
* User Role Information

## Evidence

* user_before_assignment.png
* user_administrator_role_empty.png
* user_admin_role_assigned.png
* contractor_elevated_access.png
* user_administrator_role_assigned.png
* audit_log_role_assignment.png
* role_removed_remediation.png
* audit_log_role_removal.png

## Impact

A contractor account gained administrative capabilities that exceeded business requirements.

Potential risks included:

* User account manipulation
* Password resets
* Unauthorized identity management actions
* Privilege abuse

## Remediation

The excessive role assignment was removed and audit logs were reviewed to verify remediation.

## MITRE ATT&CK

* T1078 Valid Accounts
* T1098 Account Manipulation
* T1068 Privilege Escalation
