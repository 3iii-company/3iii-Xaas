# DATA-001 — Supabase Production Blueprint
**Source:** `Blueprint ฉบับปรับปรุงสำหรับ Production_261022_100420.txt`
**Status:** PROPOSED design; current schema and deployment state UNVERIFIED.

## Source-defined scope
The blueprint proposes phases for environment setup, identity/SSO/3i ID, organization and IAM, wallet/double-entry ledger, transfer/escrow/COD/settlement, audit/event center/notifications, AI center, storage/Edge Functions/API boundary and production hardening.

## Proposed logical schemas
`core`, `iam`, `wallet`, `audit`, `event_center`, `ai`, `notification`, plus a non-exposed/private area where appropriate. Schema names alone do not guarantee isolation; exposed-schema configuration, GRANTs, RLS and function EXECUTE privileges must be verified.

## Financial-domain safeguards proposed
- Immutable posted ledger; corrections via reversal entries.
- Positive monetary amounts and currency-aware balancing.
- Idempotency keys for retry-safe commands.
- Atomic posting and balance updates.
- Concurrency control to prevent invalid negative balances.
- Explicit escrow state transitions and audit records.
- Reconciliation of cached balances against ledger entries.

## Security and operations proposed
RLS on exposed tables, explicit grants, restricted SECURITY DEFINER functions, server-only secrets, private storage buckets for sensitive evidence, webhook signature validation, backup/restore tests, monitoring and incident runbooks.

## Required before implementation
Confirm business/regulatory model; review accounting invariants and transaction isolation; define tenant boundaries and policy tests; inspect live schemas/migrations/RLS/grants/functions/storage policies; verify backup/PITR and restore; obtain explicit production-impacting change approval.

## Sensitive source handling
Project identifiers and key/token strings are intentionally omitted. Never add service-role keys, database passwords or private credentials.
