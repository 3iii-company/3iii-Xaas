# DEV-001 — Repository and CI/CD Baseline
**Status:** Source assessment reports CI/CD operational and ruleset implemented; live status UNVERIFIED.

## Source-reported baseline
The supplied Executive Governance Assessment records Gate 0 as approved with conditions and identifies independent review remediation, formal required status checks, bypass actor review and governance issue closure as conditions.

## Proposed repository layout
`apps/`, `packages/`, `supabase/migrations/`, `contracts/`, `scripts/`, `tests/`, `docs/`.

## CI stages (proposed)
1. Format/lint/type checks.
2. Unit tests.
3. Integration tests using isolated test services and non-production credentials.
4. Dependency and secret scanning.
5. Build and artifact validation.
6. Preview deployment checks where applicable.
7. Required review and protected-branch policy.

## Release safety
No CI workflow may silently bypass required checks or deploy production as an incidental side effect of a documentation or code PR.

## Live verification required
Repository full name, default branch, branch ruleset, required checks, bypass actors, workflow definitions, latest successful runs, CODEOWNERS and environment protection rules.
