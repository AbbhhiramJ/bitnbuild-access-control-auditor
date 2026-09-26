# Web Application Access-Control Auditor

A controlled, demo-first authorization test bench that checks role and resource permissions against an explicit access policy.

## MVP
- Seeded access-control records and authorization scenarios
- Search and filtering for review
- Demo-only policy correction simulation
- Six-case authorization matrix with expected-versus-actual outcomes
- CSV export of the demo data

## Live demo
https://bitnbuild-access-control-auditor.vercel.app

## Demo walkthrough
1. Review the seeded authorization records and filter/search as needed.
2. Open a record to inspect its context.
3. Run the authorization matrix to see baseline outcomes.
4. Apply the demo policy correction and rerun the matrix.
5. Compare expected and actual results; export the sample data if needed.

## Scope and limitations
The demo uses synthetic records and local browser state. It does not scan arbitrary websites, call a real application API, or modify real access policies or permissions. The correction is simulated against seeded cases.

## Local run
Open `index.html` in a modern browser. No backend is required.

See [project brief](docs/PROJECT_BRIEF.md).
