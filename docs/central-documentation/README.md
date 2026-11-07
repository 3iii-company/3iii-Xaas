# 3i-XaaS Central Documentation System
**Parent workspace:** `3iii BUSINESS OS`
**Baseline:** `0.1.0-draft` · **Prepared:** 7 November 2026
**Status:** INITIAL CONSOLIDATED DRAFT — NOT APPROVED FOR PRODUCTION

This directory is the GitHub mirror for critical governance and architecture documents. Dropbox is the primary documentation workspace; GitHub retains the critical, version-controlled subset.

## Status vocabulary
- `CONFIRMED`: explicitly supported by a supplied source.
- `PROPOSED`: recommended design, not proof of implementation.
- `PENDING`: decision or evidence still required.
- `UNVERIFIED`: not independently checked against a live system.

Do not treat proposed designs as deployed capabilities. Update the relevant document and the master register together. Record material decisions in `decisions/` and retain evidence in the primary workspace.

## Scope
Governance, enterprise architecture, Core Platform, App Factory, Supabase data blueprint, security, CI/CD and architecture decisions.

## Safety boundary
This documentation PR does not change application code, Supabase, Vercel, production data, secrets, permissions, branch rules, deployments or billing. Production implementation requires separate approvals and evidence.
