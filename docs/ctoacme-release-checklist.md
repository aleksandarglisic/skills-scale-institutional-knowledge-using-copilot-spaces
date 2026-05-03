# OctoAcme — Release Checklist

Purpose: A concrete, repeatable checklist used before any production release.

Pre-release
- [ ] All acceptance criteria completed and linked to PRs
- [ ] All PRs have required approvals and passing CI
- [ ] Security scanning completed and no critical findings blocking release
- [ ] Migration scripts reviewed and tested (if applicable)
- [ ] Release notes drafted (PdM / PM)

Staging
- [ ] Deploy to staging using release pipeline
- [ ] Run smoke tests and key end-to-end flows
- [ ] Stakeholder / product demo (if required)

Production
- [ ] Schedule deployment window and notify stakeholders/support
- [ ] Run pre-deploy checklist (backups, feature flags)
- [ ] Deploy via automated pipeline
- [ ] Run post-deploy smoke tests and verification
- [ ] Monitor dashboards/alerts for 15–60 minutes (team-defined)
- [ ] Announce release and update status

Rollback / Incident
- [ ] Rollback plan ready and tested
- [ ] Incident owner and on-call notified
- [ ] Post-incident retrospective and action items captured

Ownership
- Release owner: Release Engineer (coordinates), PdM (product sign-off), PM (communication)
