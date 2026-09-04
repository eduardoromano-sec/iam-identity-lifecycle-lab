# Mover Process

## Purpose

The Mover Process defines how identity attributes and access rights are reviewed and updated when a user's position, department, responsibilities, manager, employment type, or other relevant attributes change.

The objective is to ensure that users retain only the access required for their current responsibilities and to prevent privilege accumulation over time.

## Authoritative Source

Changes to authoritative identity attributes must originate from an approved source, such as Human Resources or the organization's HR Information System (HRIS).

Manager requests alone must not modify authoritative employment attributes such as department, job title, or employment status.

## Access Recalculation

When a relevant identity attribute changes, the user's access must be evaluated against the access model associated with the new role.

The process must identify:

- Access that must be retained
- Access that must be added
- Access that must be removed
- Access requiring additional review
- Existing exceptions that may be affected by the change

Access associated with the previous role must not be retained by default.

## Role-Based Access

Access predefined and approved for the user's new role may be provisioned according to the established Role-Based Access Control model.

Access outside the approved role must follow the Access Request Policy.

## Removal of Previous Access

Permissions associated exclusively with the user's previous responsibilities must be revoked when they are no longer required.

This process reduces the risk of privilege creep caused by users accumulating permissions as they move between roles.

## Transitional Access

Access associated with a previous role may be temporarily retained when required for a legitimate business transition.

Transitional access must:

- Have a documented business justification
- Be approved by the appropriate resource owner
- Be acknowledged or approved by the user's new management when appropriate
- Have a defined expiration date
- Follow the principle of least privilege
- Be reviewed for potential Segregation of Duties conflicts

Transitional access must expire by default unless an extension is approved before the expiration date.

## Segregation of Duties

Changes in responsibilities may introduce conflicts between existing and newly assigned permissions.

Potential conflicts must be evaluated before access is retained or provisioned.

Creating separate accounts does not automatically eliminate a Segregation of Duties conflict because multiple accounts may belong to the same identity.

When a temporary conflict cannot be avoided, the exception must be documented and appropriate compensating controls must be considered.

Examples include:

- Additional logging and monitoring
- Independent review of sensitive activities
- Restricting access to specific resources
- Preventing users from reviewing or approving their own activities
- Strict expiration of conflicting access

## Identity Record

The identity record must reflect the user's current organizational attributes and access state.

Historical information should be retained to support investigation and audit requirements.

Records should allow the organization to identify:

- Previous and current department
- Previous and current role
- Previous and current manager
- Current entitlements
- Temporary access
- Access expiration dates
- Previous lifecycle states
- Related access requests

## Audit Trail

Mover events must maintain sufficient evidence to identify:

- The authoritative source of the change
- Previous identity attributes
- New identity attributes
- Access added
- Access removed
- Access temporarily retained
- Business justification for exceptions
- Required approvals
- Compensating controls when applicable
- Provisioning and revocation timestamps
- Expiration dates
