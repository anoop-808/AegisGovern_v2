# Attack 3: Excessive Permissions and Directory Enumeration

## Objective

Demonstrate how a low-privileged user can enumerate directory information beyond business requirements.

## Attack Simulation

The Intern User account was used to explore available directory information, including users, groups and administrative roles.

## Detection

The investigation reviewed:

* User Visibility
* Group Visibility
* Administrative Role Visibility
* Access Restrictions

## Evidence

* intern_login.png
* users_visible.png
* groups_visible.png
* administrators_group_members.png
* roles_visible.png
* auth_methods_denied.png

## Remediation

* Apply least privilege principles
* Restrict directory visibility where possible
* Monitor excessive enumeration activities

## MITRE ATT&CK

* T1087 Account Discovery
* T1069 Permission Group Discovery
