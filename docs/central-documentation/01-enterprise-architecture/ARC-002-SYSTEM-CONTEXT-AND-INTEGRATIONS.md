# ARC-002 — System Context and Integrations
**Status:** PROPOSED; live integration status UNVERIFIED.

| System | Intended responsibility | Evidence needed |
|---|---|---|
| GitHub | Source control, PR review, rulesets and CI workflows | Repository identity, branch, ruleset export, workflow runs |
| Supabase | Auth, PostgreSQL, storage and server-side functions | Project inventory, exposed schemas, migrations, RLS/grants |
| Vercel | Web hosting, preview/production deployments | Project IDs, linked repositories, environment mapping |
| AI Builders | Accelerate app prototyping/build handoff | Approved builder list, ownership, security and acceptance workflow |

## Integration rules
- Use least-privilege service identities and scoped credentials.
- Keep secrets in provider-managed secret stores, never in this documentation.
- Version API and event contracts.
- Use webhook signature validation, replay protection and idempotency.
- Separate development, preview/staging and production environments.
- Record system-of-record ownership for each business entity.

## Current-state caution
The supplied files describe intended integrations and a Supabase project reference, but do not prove that all connections are configured or healthy.
