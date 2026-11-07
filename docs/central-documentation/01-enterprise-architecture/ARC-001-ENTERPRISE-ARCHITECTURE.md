# ARC-001 — Enterprise Architecture Overview
**Status:** PROPOSED baseline assembled from available project context.

## Architectural intent
3i-XaaS is being organized as a shared platform with reusable core capabilities and a portfolio of business applications. The intended operating model separates platform foundation, application factory and application portfolio.

## Logical layers (proposed)
1. Experience: web/mobile applications, workspaces and role-specific interfaces.
2. Application: business apps and domain workflows.
3. Core platform: identity, organization/tenant context, app registry, authorization, audit, eventing and shared services.
4. Data: PostgreSQL/Supabase, storage and domain-specific boundaries.
5. Integration: APIs, webhooks, event contracts and external providers.
6. Delivery/operations: GitHub, CI/CD, Vercel, monitoring, backup and incident response.
7. Governance: approvals, evidence, ownership, security and lifecycle controls.

## Proposed repository model
A monorepo is a candidate, not confirmed current layout: `apps/`, `packages/`, `supabase/migrations/`, `contracts/`, `tests/`, `docs/`.

## Unresolved decisions
Canonical app inventory, tenancy model, SSO scope, deployment topology, API boundary, shared vs app-owned data and repository strategy.
