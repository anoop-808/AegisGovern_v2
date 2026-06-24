# Incident Report – Attack 3: Excessive Information Exposure

## Incident Summary

An Intern User account was able to enumerate users, groups, roles, and administrative information within the tenant.

## Affected User

- User: Intern User

## Evidence

- intern_login.png
- users_visible.png
- groups_visible.png
- administrators_group_members.png
- roles_visible.png
- auth_methods_denied.png

## Impact

An attacker could use visible information for reconnaissance and privilege targeting.

## Detection

User enumeration activities were reviewed during access testing.

## Response

- Visibility reviewed.
- Administrative access restrictions validated.

## Lessons Learned

Excessive information exposure can assist attackers during reconnaissance phases.
