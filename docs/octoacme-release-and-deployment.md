# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- Passing CI and security scans
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared

## Release Coordination Process
The Release Manager coordinates with all roles to ensure readiness:

### Release Coordination Checklist
- [ ] **Development Complete**: All features merged and CI passing (Developer sign-off)
- [ ] **Quality Verification**: QA Lead sign-off confirming:
  - [ ] All test plans executed
  - [ ] Critical path testing completed
  - [ ] No P0/P1 defects outstanding
  - [ ] Regression testing passed
- [ ] **Security Review**: Security Lead sign-off confirming:
  - [ ] Security scans completed with no critical vulnerabilities
  - [ ] Security review completed for new features
  - [ ] Security incident response plan reviewed
- [ ] **Stakeholder Approval**: Stakeholder Representative confirms:
  - [ ] Release timing acceptable to business
  - [ ] Communication plan in place
  - [ ] Support teams notified and prepared
- [ ] **Release Manager Verification**:
  - [ ] Release notes reviewed and approved
  - [ ] Rollback procedure tested and documented
  - [ ] Deployment runbook updated
  - [ ] Monitoring and alerting configured
  - [ ] On-call rotation confirmed

### Cross-Team Handoff Process
1. **Development → QA**: Developer signals feature complete, provides test guidance
2. **QA → Security**: QA Lead confirms functionality testing complete
3. **Security → Release Manager**: Security Lead provides security clearance
4. **Release Manager → Stakeholders**: Release Manager requests business approval
5. **All → Release Manager**: Final go/no-go meeting 24 hours before deployment

## Deployment Checklist
- [ ] Deployment window scheduled (if needed)
- [ ] Backup or snapshot (if applicable)
- [ ] Deploy to staging and run smoke tests
- [ ] Deploy to production (automated pipeline preferred)
- [ ] Run post-deploy verifications
- [ ] Announce release to stakeholders and support

## Rollback & Incident Playbook
If a deployment fails or causes a critical issue, follow this procedure:

### Rollback Decision Criteria
Initiate immediate rollback if ANY of these conditions are met:
- **Critical functionality broken**: Core user workflows failing
- **Data integrity risk**: Risk of data loss or corruption
- **Security vulnerability**: Active security threat in production
- **Performance degradation**: >50% increase in errors or latency
- **Business impact**: Revenue or SLA-impacting issues

### Rollback Procedure
1. **Declare Incident** (Release Manager):
   - Notify on-call team and incident response channel
   - Page Security Lead if security-related
   - Alert Stakeholder Representative of user impact

2. **Assess Situation** (within 15 minutes):
   - Release Manager leads rapid triage with available engineers
   - Determine: Can issue be hotfixed quickly (<30 min) or require rollback?
   - QA Lead validates rollback target if rollback chosen

3. **Execute Rollback** (Release Manager coordinates):
   - [ ] Announce rollback decision to team and stakeholders
   - [ ] Execute automated rollback to last known-good release
   - [ ] Run post-rollback smoke tests (QA Lead validates)
   - [ ] Verify monitoring shows healthy state
   - [ ] Update status page and notify stakeholders

4. **Post-Rollback Actions**:
   - [ ] Release Manager captures timeline and impact
   - [ ] Schedule blameless post-mortem within 48 hours
   - [ ] Create action items for prevention
   - [ ] Update deployment checklist if gaps identified
   - [ ] Security Lead reviews if security-related

### Rollback Authority
- **Release Manager**: Primary authority for rollback decision
- **Security Lead**: Can mandate immediate rollback for security issues
- **On-call Engineer**: Can initiate rollback if Release Manager unavailable
- **Escalation**: If disagreement, escalate to Product Lead within 10 minutes

### Incident Communication Template
**Initial Alert** (within 5 minutes):
- Incident summary: [brief description]
- Impact: [user/business impact]
- Status: [investigating/rolling back/mitigating]
- Response team: [who is responding]
- Next update: [time]

**Resolution Notice**:
- Incident resolved: [date/time]
- Root cause: [brief summary]
- Actions taken: [rollback/hotfix/etc]
- Post-mortem scheduled: [date/time]
- Contact: [Release Manager]

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
