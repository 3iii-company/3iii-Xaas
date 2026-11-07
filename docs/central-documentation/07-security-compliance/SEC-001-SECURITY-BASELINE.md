# SEC-001 — Security Baseline
**Status:** PROPOSED; requires Security Lead review.

## Minimum controls
- Least privilege for human and machine identities.
- MFA and secure account recovery for privileged access.
- Separate development, staging and production credentials.
- Secrets only in approved secret managers; never in source, logs or documentation.
- RLS plus explicit grants and server-side authorization.
- Branch protection, required reviews and CI status checks.
- Dependency and secret scanning in CI.
- Audit logs for privileged actions and sensitive data access.
- Data classification, retention, deletion and privacy controls.
- Incident response, credential rotation and recovery exercises.

## Threat areas to assess
Tenant boundary bypass, privilege escalation, insecure SECURITY DEFINER functions, exposed storage objects, leaked credentials, webhook replay, duplicate financial commands, supply-chain compromise and unsafe AI actions.

## Compliance boundary
Applicable laws, licensing, AML/KYC, tax, privacy and financial-services obligations depend on jurisdictions and actual operations. This pack does not certify compliance or legal readiness.

## Open actions
Threat model, data inventory, privacy impact assessment, security owner sign-off, penetration testing scope and incident escalation contacts.
