# GOV-001 — Governance Baseline
**Status:** PROPOSED; source assessment exists, current live controls not re-verified.

## Principles
1. Least privilege and time-bounded access.
2. Separation of duties for author, reviewer, approver and deployer.
3. Evidence first: no change is successful without verifiable results.
4. Environment separation: development, staging and production.
5. No secrets in chat, issues, commits or documents.
6. Rollback readiness for high-impact changes.
7. Expiry and periodic review of delegated authority.
8. Paper approval does not bypass provider-enforced controls.

## Change classes
B0 read-only; B1 branch/PR; B2 merge; B3 production deployment; B4 database/schema/migration; B5 secrets/access; B6 security/governance; B7 billing/domain; B8 emergency/incident.

Each class requires defined approver, scope, environment, evidence, expiry and rollback plan as applicable.

## Approval boundary
The supplied approval packet distinguishes PR review/technical work from merge, production deployment, branch rulesets, permissions, secrets and database changes. Higher-impact actions require separate approval unless a valid company policy grants bounded authority.

## Minimum change record
Request ID, repository/project, target branch/environment, purpose, exact diff, risk, tests, approver, execution actor, timestamp, resulting commit/deployment/migration ID, rollback method and closure evidence.

## Open items
Confirm policy adoption, authorized roles, evidence retention, exception expiry and current provider controls.
