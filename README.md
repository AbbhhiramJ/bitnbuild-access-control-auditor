# Web Application Access-Control Auditor

A controlled, demo-first authorization test bench that checks role and resource permissions against an explicit access policy.

## MVP
- Define users, roles, resources, and allowed actions
- Generate a role/resource/action test matrix
- Run tests only against the included local demo API
- Report denied/allowed mismatches with reproducible evidence
- Re-test after a policy fix

## Scope
The initial target is the bundled demo application, not arbitrary websites. See [project brief](docs/PROJECT_BRIEF.md).
