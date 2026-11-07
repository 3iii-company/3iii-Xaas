# AF-001 — App Factory Operating Model
**Status:** PROPOSED.

## Purpose
Provide a repeatable path for taking an approved business requirement through specification, design, implementation, testing, security review and release.

## Standard workflow
1. Intake: business owner, problem, target users, outcomes and constraints.
2. Discovery: process map, data classification, integrations and dependencies.
3. Product brief: PRD, user journeys, acceptance criteria and non-goals.
4. Architecture: app boundary, data ownership, API/events, auth and threat model.
5. UX/UI: design system, responsive states, accessibility and motion guidance.
6. Build handoff: builder-specific instructions, repository structure, contracts and guardrails.
7. Implementation: branch/PR, tests, review and evidence.
8. Release: staging validation, explicit production approval, deployment and rollback.
9. Operations: owner, runbook, monitoring, support and periodic review.

## AI Builder handoff package
APP-BRIEF, PRD, UX-FLOWS, UI-SYSTEM, ARCHITECTURE, DATA-MODEL, API-CONTRACTS, SECURITY-REQUIREMENTS, ACCEPTANCE-TESTS and DEPLOYMENT-RUNBOOK.

## Builder guardrails
Builders may generate implementation proposals within approved scope. They must not invent business rules, change shared schemas, expose secrets, bypass tests or deploy production without explicit approval.
