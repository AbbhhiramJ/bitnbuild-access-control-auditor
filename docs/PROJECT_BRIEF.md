# Project brief — Web Application Access-Control Auditor

## User and problem
**Primary user:** a web developer, QA engineer, or application-security tester validating authorization before release.

A recurring testing challenge is that a user may be authenticated but still access another user's object or a function beyond their role. UI hiding alone does not enforce server-side authorization.

## Product promise
Make authorization expectations explicit and repeatable: map principals, resources, and actions; test expected allow/deny outcomes; show evidence; then re-run after remediation.

## MVP workflow
1. Select a bundled demo scenario with multiple users and roles.
2. Review its declared access policy.
3. Generate horizontal and vertical authorization cases.
4. Execute cases against the local demo API.
5. Inspect failures, apply a policy fix, and re-run the same tests.

## Acceptance criteria
- Matrix covers role-level function access and object ownership checks.
- Every finding includes principal, action, target resource, expected result, actual result, and test evidence.
- Tests are repeatable and safe; no external target is scanned by default.
- Demo visibly changes from failing checks to passing checks after a fix.

## Boundaries
Only the intentionally vulnerable bundled lab is in scope by default. Require explicit authorization and target confirmation before adding any external-target testing.

## Research leads
- OWASP Web Security Testing Guide — IDOR testing objectives and method: https://github.com/OWASP/www-project-web-security-testing-guide/blob/master/v42/4-Web_Application_Security_Testing/05-Authorization_Testing/04-Testing_for_Insecure_Direct_Object_References.md
- OWASP Authorization Regression Testing Cheat Sheet: https://cheatsheetseries.owasp.org/cheatsheets/Authorization_Regression_Testing_Cheat_Sheet.html
- Community discussion on checking object ownership and server-side authorization: https://www.reddit.com/r/Bard/comments/1tvce33/day_1_what_is_idor/
