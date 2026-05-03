# OctoAcme — Role Interactions & Responsibilities Matrix

Purpose: document how roles collaborate, who makes which decisions, and escalation/hand-off points.

## Decision and Responsibility Summary
- Product direction: Product Manager (PdM) owns outcomes; Product Lead approves major direction.
- Delivery commitments: Project Manager (PM) owns schedule; Developers estimate work and commit scope.
- Quality gate: QA Lead signs off on releases; Release Engineer enforces deployment checklist.
- Release execution: Release Engineer runs deployment; PM communicates timing; on-call handles incidents.

## Example interaction flows

- Feature delivery
  - PdM writes one-pager and success metrics → PM schedules work and assigns owners → UX produces designs → Devs implement → QA validates → Release Engineer deploys → Data Analyst reports results.

- Incident / rollback
  - On-call detects incident → On-call and Release Engineer triage → PM and PdM notified → Rollback if needed → Post-incident retrospective assigned to owners.

## Role collaboration table (high level)
- PdM ⇄ PM: prioritization, scope tradeoffs
- PM ⇄ Developers: scheduling, blockers
- PM ⇄ Release Engineer: release schedule and risk mitigation
- PdM ⇄ UX: user needs and design validation
- Developers ⇄ QA Lead: testability, bug triage
- Data Analyst ⇄ PdM: metrics and success validation

## Escalation paths
1. Team-level (Scrum Master / daily standup)
2. PM escalation to Product Lead or dependent teams
3. Sponsor-level for business-impacting issues

## Where to find artifacts
- One-pager: project root / Project Charter
- Release checklist: docs/octoacme-release-checklist.md
- Role definitions: docs/octoacme-roles-and-personas.md
