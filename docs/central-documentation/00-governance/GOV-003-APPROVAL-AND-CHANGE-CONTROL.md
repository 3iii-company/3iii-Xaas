# GOV-003 — Approval and Change Control
**Source:** 3i-XaaS project approval packet, dated 27 October 2569 (2026).

## Source-defined approval tiers
B0 read-only; B1 branch/PR; B2 merge; B3 production deployment; B4 database/migration; B5 secrets/access; B6 security/governance; B7 billing/domain; B8 incident/emergency.

## Mandatory safeguards
- Scope approval to exact repository, project, branch and environment.
- Do not infer merge or production deployment approval from approval to edit code.
- Do not change branch rulesets, required checks, bypass actors, access permissions, secrets or production data without explicit authority.
- Do not use another person's private key, password, token or session.
- Record commit SHA, signature verification, CI/test results, review evidence and deployment evidence where applicable.
- For data/schema changes, retain migration diff, backup evidence, test results and rollback plan.
- For security/access changes, record target identity, permission diff, justification and audit evidence.

## Source caveat
The supplied packet is a draft/approval form and describes recommended future governance. It does not automatically alter provider permissions or prove formal policy adoption.
