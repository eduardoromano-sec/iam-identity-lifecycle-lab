# Joiner Process

## Purpose

The Joiner Process defines how new identities are validated, provisioned, activated, and reviewed when joining NovaTech Solutions.

The objective is to ensure that new users receive the appropriate access required for their role while following the principles of least privilege and secure identity lifecycle management.

## Authoritative Source

Human Resources is responsible for providing the authoritative information required to initiate the onboarding process.

In the current manual workflow, onboarding is initiated through an approved HR request.

A mature implementation could integrate the HR Information System (HRIS) directly with the Identity Management platform, allowing approved employment records to automatically trigger identity lifecycle workflows.

## Required Identity Attributes

The onboarding request must contain the attributes required to establish the corporate identity, including:

- Full name
- Employee ID
- Personal contact information when required for initial onboarding
- Job title
- Department
- Team
- Manager
- Start date
- Employment type
- Additional relevant onboarding information

Additional personal information must only be collected when required for a legitimate business purpose.

## Identity Validation

Before provisioning begins, the onboarding request must be validated to confirm:

- The employment relationship has been approved
- The start date is valid
- The assigned department and job title are correct
- The appropriate manager has been identified
- Required identity attributes are available

## Access Assignment

Access is assigned using predefined access models.

### Birthright Access

Eligible employees receive standard corporate access:

- Google Workspace — Standard User
- Slack — Standard User
- Jira — Standard User

### Role-Based Access

Additional access is assigned according to the user's approved business role.

Example:

**Software Engineer**

- GitHub — Developer
- AWS — Developer

Role definitions must be documented, approved, and periodically reviewed.

Access outside the predefined role must follow the Access Request Policy.

## Pre-Provisioning and Activation

Accounts may be provisioned before the employee's start date to allow sufficient time for technical preparation.

Pre-provisioning must not result in unauthorized early access.

Where technically possible, identity activation and access availability must correspond with the approved employment start date.

## Initial Authentication

Initial authentication must follow a secure activation process.

Permanent passwords must not be transmitted through unsecured communication channels or plain-text email.

Users must configure required authentication mechanisms, including Multi-Factor Authentication (MFA), during the initial account activation process.

## Provisioning Validation

After provisioning, the assigned access must be validated against the approved identity attributes and role.

The onboarding record must identify:

- Accounts created
- Roles assigned
- Entitlements granted
- Provisioning status
- Activation status
- Exceptions or additional requests

## Post-Onboarding Review

A post-onboarding review may be performed after the user's first days of employment to identify:

- Missing required access
- Incorrect permissions
- Excessive access
- Provisioning failures
- Access granted outside the approved role

Post-onboarding validation should be tracked separately from the initial provisioning process to maintain accurate operational metrics.

## Audit Trail

The organization must maintain sufficient records to reconstruct the identity lifecycle and determine:

- Who initiated the onboarding
- Who approved it
- When the identity was created
- When the identity was activated
- Which roles were assigned
- Which entitlements were provisioned
- Any exceptions or modifications made during onboarding
