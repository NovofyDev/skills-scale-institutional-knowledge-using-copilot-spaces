# OctoAcme — Risk Management & Communication

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner
- Mitigation plan
- Status

## Risk Lifecycle
- Identify: during planning and ongoing execution
- Assess: estimate impact and likelihood
- Mitigate: reduced via actions, contingency plans
- Monitor: review at weekly syncs and update status

## Stakeholder Communication

### Identifying Stakeholders
Stakeholder groups and their communication needs:

| Stakeholder Group | Primary Contact | Communication Frequency | Channel |
|------------------|----------------|------------------------|---------|
| Engineering Team | Project Manager | Daily | Standup, Slack |
| Product Leadership | Product Manager | Weekly | Status meeting |
| Sales Team | Stakeholder Rep | Milestone-based | Email updates |
| Support Team | Stakeholder Rep | Per release | Release notes |
| Executive Sponsors | Project Manager | Monthly | Executive summary |
| Customers/Users | Stakeholder Rep | Per release | Product announcements |

### Stakeholder Communication Plan
- **Establish Early**: Identify stakeholders during project initiation
- **Tailor Messages**: Customize content and detail level per audience
- **Be Proactive**: Don't wait for stakeholders to ask for updates
- **Use Single Source of Truth**: Maintain status in project README or dashboard
- **Set Expectations**: Define update frequency and format upfront

### Stakeholder Feedback Loop Process
1. **Gather Feedback**:
   - Stakeholder Representative collects input from stakeholder groups
   - QA Lead coordinates user acceptance testing
   - Product Manager conducts user research and validation
   
2. **Consolidate & Prioritize** (weekly):
   - Stakeholder Representative presents feedback in planning meeting
   - Product Manager assesses impact and priority
   - Project Manager tracks feedback items
   
3. **Act & Communicate**:
   - Team addresses high-priority feedback
   - Stakeholder Representative communicates decisions back to stakeholders
   - Close the loop: "Here's what we heard and what we're doing about it"
   
4. **Measure Effectiveness**:
   - Track feedback response time
   - Monitor stakeholder satisfaction
   - Review feedback loop in retrospectives

## Communication Templates

### Weekly Status Template
**Project**: [Project name]  
**Week**: [Date range]  
**Status**: 🟢 On Track / 🟡 At Risk / 🔴 Blocked

**Progress this week**:
- [Completed items with links to PRs/issues]
- [Key milestones achieved]

**Next steps**:
- [Planned work for next week]
- [Upcoming milestones]

**Risks & blockers**:
- [Current risks with mitigation status]
- [Active blockers and who is working on them]

**Metrics**:
- Velocity: [current vs target]
- Test coverage: [percentage]
- Critical bugs: [count]

**Ask / decisions needed**:
- [Questions for stakeholders]
- [Decisions required and by when]

---

### Milestone Update Template
**Milestone**: [Name]  
**Target Date**: [Date]  
**Status**: 🟢 On Track / 🟡 At Risk / 🔴 Delayed

**Completed**:
- [List of completed features/work]

**In Progress**:
- [Current work with % complete]

**Remaining**:
- [Outstanding work items]

**Confidence**: [High/Medium/Low] that we'll hit target date

**Changes from Last Update**:
- [What's different since last report]

**Stakeholder Impact**:
- [How this affects stakeholders/users]

---

### Stakeholder Feedback Summary Template
**Feedback Period**: [Date range]  
**Stakeholder Groups**: [Sales, Support, Customers, etc.]

**Key Themes**:
1. [Theme 1]: [Summary of feedback]
   - Impact: [High/Medium/Low]
   - Action: [What we're doing about it]
   
2. [Theme 2]: [Summary of feedback]
   - Impact: [High/Medium/Low]
   - Action: [What we're doing about it]

**Top Requests**:
- [Request 1]: [Status - Planned/In Progress/Completed/Not Planned]
- [Request 2]: [Status]
- [Request 3]: [Status]

**Feedback Response Rate**: [X% of feedback items addressed]

**Next Steps**:
- [How we'll incorporate feedback]

---

### Release Communication Template
**Release**: [Version/Name]  
**Release Date**: [Date and time]  
**Type**: Major / Minor / Patch

**What's New**:
- [User-facing feature 1]
- [User-facing feature 2]
- [Key improvements]

**What's Fixed**:
- [Bug fixes that impact users]

**Action Required** (if any):
- [Steps users need to take]
- [Migration instructions]

**Known Issues**:
- [Any limitations or known bugs]

**Support Resources**:
- Documentation: [link]
- Support contact: [contact info]
- Feedback: [how to provide feedback]

**Rollout Plan**:
- [Phased rollout details if applicable]

---

### Incident Communication

**Initial Alert** (within 15 minutes of detection):
- **Incident ID**: [Unique ID]
- **Severity**: SEV-1 / SEV-2 / SEV-3 / SEV-4
- **Impact**: [What's affected and how many users]
- **Status**: Investigating / Identified / Monitoring / Resolved
- **Current Actions**: [What response team is doing]
- **Next Update**: [Specific time]
- **Incident Lead**: [Name and contact]

**Progress Update** (every 30-60 minutes for SEV-1/2):
- **Time**: [Timestamp]
- **Status Update**: [What's changed]
- **Current Actions**: [What's happening now]
- **ETA**: [Expected resolution time if known]
- **Next Update**: [Specific time]

**Resolution Notice**:
- **Incident ID**: [Unique ID]
- **Resolution Time**: [Date/time]
- **Root Cause**: [Brief summary]
- **Actions Taken**: [How it was resolved]
- **User Impact**: [How many users affected, for how long]
- **Prevention**: [What we're doing to prevent recurrence]
- **Post-mortem**: [Scheduled date/time and link]
- **Contact**: [For questions]

---

### Risk Escalation Communication
**Risk ID**: [ID from risk register]  
**Risk**: [Description]  
**Impact**: High / Medium / Low  
**Likelihood**: High / Medium / Low  

**Why Escalating**:
- [Reason for escalation - increased likelihood, failed mitigation, etc.]

**Current Mitigation**:
- [What's been tried]
- [Why it's not sufficient]

**Decision Needed**:
- [What decision is required]
- [Options available]
- [Deadline for decision]

**Impact of Inaction**:
- [What happens if we don't address this]

**Recommendation**:
- [Proposed course of action]

## Escalation Paths

### Standard Escalation Levels
**Level 1 - Team Escalation**:
- **When**: Issues team can resolve independently
- **Process**: Raised in daily standup, assigned owner
- **Timeline**: Resolve within sprint
- **Escalate if**: Not resolved in 3 days or impacts sprint goal

**Level 2 - Project Management Escalation**:
- **When**: Cross-team dependencies, resource conflicts, missed deadlines
- **Owner**: Project Manager coordinates resolution
- **Involves**: Product Manager for priority decisions
- **Timeline**: Decision within 2 business days
- **Escalate if**: Impacts release timeline or requires executive decision

**Level 3 - Leadership Escalation**:
- **When**: Business-impacting decisions, significant delays, budget needs
- **Owner**: Product Lead coordinates with stakeholders
- **Involves**: Executive sponsor, relevant VPs
- **Timeline**: Decision within 1 week
- **Escalate if**: Requires board approval or affects company commitments

### Security Incident Escalation
- **Security Issues**: Follow security incident runbook (see octoacme-security-processes.md)
- **Point of Contact**: Security Lead (primary), on-call engineer (backup)
- **Immediate Escalation**: Critical vulnerabilities or active breaches go directly to Security Lead
- **After Hours**: Page Security on-call immediately for SEV-1/SEV-2 incidents

### Quality Escalation
- **Quality Gates Failed**: QA Lead blocks release, escalates to Release Manager
- **Critical Defects**: QA Lead escalates to Project Manager and Product Manager
- **Release Decision**: If disagreement on release readiness, Release Manager escalates to Product Lead

### Cross-Functional Escalation Matrix

| Issue Type | First Contact | Escalate To | Final Authority |
|-----------|--------------|-------------|----------------|
| Technical blocker | Developer lead | Project Manager | Product Lead |
| Quality concern | QA Lead | Release Manager | Product Lead |
| Security issue | Security Lead | Product Lead | CISO/Executive |
| Dependency delay | Project Manager | Product Manager | Product Lead |
| Resource conflict | Project Manager | Product Lead | Executive Sponsor |
| Stakeholder conflict | Stakeholder Rep | Product Manager | Product Lead |
| Release decision | Release Manager | Product Lead | Executive Sponsor |
| Scope change | Product Manager | Product Lead | Executive Sponsor |

### Escalation Best Practices
- **Document First**: Capture the issue, impact, and options before escalating
- **Provide Context**: Include timeline, stakeholders affected, and decision deadline
- **Propose Solutions**: Come with recommendations, not just problems
- **Be Timely**: Don't wait until last minute to escalate
- **Follow Up**: After escalation decision, communicate outcome to all affected parties
- **Track Patterns**: Review escalations in retrospectives to improve processes
