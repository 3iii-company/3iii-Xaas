# CORE-001 — Core Platform Blueprint
**Status:** PROPOSED architecture; not proof of deployed implementation.

## Shared capabilities proposed
Identity/profile and account lifecycle; organization/membership context; app/module/feature registry; role and permission management; audit trail/security events; event/outbox foundation; notifications; shared API/integration boundary; AI gateway and usage governance.

## Identity model (proposed)
Use the authentication provider's immutable user UUID as the authentication principal. Business-facing identifiers (e.g. 3i ID) are display/business identifiers and must not replace authentication identity or authorization checks.

## Authorization model (proposed)
Permission convention: `{app}.{resource}.{action}`. Evaluate authenticated identity, organization membership, application access and specific permission. Enforce server-side and in database policies; do not trust client-supplied role claims.

## Service boundaries
Financial posting, escrow transitions, access changes and other high-impact operations must execute through narrowly scoped server-side functions with idempotency, authorization and audit evidence.

## MVP sequencing
1. Environment and migration conventions.
2. Identity and profile.
3. Organization and application registry.
4. IAM/permissions.
5. Audit and event outbox.
6. Domain-specific services after approved app requirements.
7. Notifications and AI gateway.
8. Production hardening.

## Open decisions
SSO across apps/projects, organization hierarchy, role inheritance, admin break-glass model, audit retention and shared-service ownership.
