# Incident Report – Attack 1: OAuth Consent Abuse

## Severity

High

## Incident Metrics

Detection Time: 5 Minutes

Investigation Time: 10 Minutes

Containment Time: 2 Minutes

Incident Status: Resolved

## Incident Summary

A finance department user (Priya Finance) was targeted through a malicious OAuth application named Rewards Portal.

The application requested permissions that could potentially allow access to user data and organizational resources.

## Affected User

- User: Priya Finance
- Department: Finance Team

## Evidence

- rewards_portal.png
- permissions.png
- api_permissions.png
- consent_settings.png
- sign_in_logs_attack1.png
- audit_log_consent_attempt.png

## Impact

Potential unauthorized access to user data if consent had been approved.

## Detection

The suspicious application request was identified through Entra ID application review and audit monitoring.

## Response

- User consent was denied.
- Application permissions were reviewed.
- Tenant consent settings were verified.

## Lessons Learned

Users should not approve unknown applications without verification.
