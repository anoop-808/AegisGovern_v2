# Attack 1: OAuth Consent Abuse Simulation

## Objective

Simulate a malicious OAuth application requesting Microsoft Graph permissions within a Microsoft Entra ID environment.

## Attack Simulation

A custom application named Employee Rewards Portal was registered and configured with delegated Microsoft Graph permissions. The objective was to understand how malicious applications can request access to user data through the consent process.

## Detection

The following sources were reviewed:

* Enterprise Applications
* Application Permissions
* Audit Logs
* Sign-In Logs

## Evidence

* enterprise_apps.png
* rewards_portal.png
* permissions.png
* consent_settings.png
* api_permissions.png
* audit_log_consent_attempt.png
* sign_in_logs_attack1.png

## Remediation

* Restrict user consent to applications
* Require administrator approval for sensitive permissions
* Monitor application registrations and permission grants

## MITRE ATT&CK

* T1078 Valid Accounts
* T1528 Steal Application Access Token
