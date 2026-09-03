# Privileged Access Model

## Overview

NovaTech Solutions separates standard user activities from privileged administrative operations.

Privileged access must only be used when administrative permissions are required.

## Standard Accounts

Standard accounts are used for normal day-to-day activities such as:

- Email
- Slack
- Jira
- Web browsing
- Standard corporate applications

Example:

`sofia.taylor@novatech.example`

## Privileged Accounts

Administrative activities must be performed using dedicated privileged accounts.

Example:

`adm.sophia.taylor@novatech.example`

The privileged account may be authorized to perform activities such as:

- User administration
- Group management
- Access configuration
- Identity lifecycle operations
- Administrative configuration

## Security Principles

Privileged accounts must:

- Be separate from standard user accounts
- Use Multi-Factor Authentication (MFA)
- Not be used for email or general web browsing
- Follow the principle of least privilege
- Have administrative actions logged
- Be periodically reviewed
- Be disabled when privileged access is no longer required

## Objective

Separating standard and privileged identities reduces the attack surface and limits the impact of compromised credentials.
