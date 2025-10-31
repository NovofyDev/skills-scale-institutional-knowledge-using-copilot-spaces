# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## Release Manager

### Role Summary
Release Managers coordinate and orchestrate software releases from staging to production. They ensure releases meet quality standards, coordinate cross-functional teams, and manage the deployment lifecycle including rollback decisions.

### Responsibilities
- Plan and schedule release windows in coordination with stakeholders
- Verify all pre-release requirements are met (tests, security scans, approvals)
- Coordinate deployment activities across engineering, QA, and operations
- Execute or oversee deployment to production environments
- Monitor post-deployment health metrics and coordinate rollback if needed
- Maintain release documentation and post-mortems
- Communicate release status to stakeholders and leadership

### Goals
- Ensure reliable, low-risk releases to production
- Minimize deployment-related incidents and downtime
- Maintain clear deployment runbooks and rollback procedures
- Enable rapid, confident deployments with minimal manual intervention

### Typical Communication
- Release planning meetings with engineering and QA leads
- Go/no-go decision meetings before production deployment
- Release notes and deployment announcements to stakeholders
- Post-deployment status updates and incident coordination

### Interactions with Other Roles
- **Developers**: Receives feature completion status, coordinates merge timelines
- **QA Lead**: Confirms testing sign-off before release approval
- **Security Lead**: Ensures security reviews completed and vulnerabilities addressed
- **Project Managers**: Aligns release schedule with project milestones
- **Stakeholder Representative**: Communicates release timing and impacts

---

## QA Lead

### Role Summary
QA Leads own quality strategy and testing processes across the project lifecycle. They define testing standards, coordinate test execution, and provide final quality sign-off before releases.

### Responsibilities
- Define and maintain test strategy and quality standards
- Coordinate test planning and resource allocation
- Review test coverage and identify quality gaps
- Execute or oversee integration and end-to-end testing
- Provide quality sign-off for releases
- Track and report on quality metrics and defect trends
- Collaborate with developers on test automation and quality tooling
- Coordinate user acceptance testing with stakeholders

### Goals
- Ensure high-quality deliverables that meet acceptance criteria
- Catch defects early in the development cycle
- Maintain comprehensive test coverage for critical paths
- Enable fast, confident releases through effective testing

### Typical Communication
- Test plan reviews with developers and project managers
- Quality gate discussions with release managers
- Defect triage meetings with development team
- Test status reports in weekly delivery syncs

### Interactions with Other Roles
- **Developers**: Collaborates on test automation, reports defects, validates fixes
- **Release Manager**: Provides quality sign-off and test results before deployment
- **Product Managers**: Validates acceptance criteria and user experience
- **Project Managers**: Reports testing progress and quality risks
- **Stakeholder Representative**: Coordinates acceptance testing and feedback

---

## Security Lead

### Role Summary
Security Leads ensure security requirements are integrated throughout the development lifecycle. They conduct security reviews, respond to vulnerabilities, coordinate incident response, and maintain security standards.

### Responsibilities
- Define and enforce security standards and best practices
- Review designs and code for security vulnerabilities
- Coordinate security testing and penetration testing
- Manage vulnerability remediation and tracking
- Lead security incident response and coordination
- Conduct security training and awareness programs
- Maintain security documentation and runbooks
- Ensure compliance with security policies and regulations

### Goals
- Minimize security vulnerabilities in production systems
- Ensure rapid detection and response to security incidents
- Build security awareness across the team
- Maintain compliance with security standards and policies

### Typical Communication
- Security reviews during design and code review phases
- Vulnerability reports and remediation tracking
- Incident response coordination during security events
- Security status updates to leadership and stakeholders

### Interactions with Other Roles
- **Developers**: Conducts security reviews, provides secure coding guidance
- **Release Manager**: Blocks releases with critical security issues, approves security readiness
- **QA Lead**: Collaborates on security testing requirements
- **Project Managers**: Reports security risks and remediation timelines
- **Stakeholder Representative**: Communicates security posture and incidents

---

## Stakeholder Representative

### Role Summary
Stakeholder Representatives act as the voice of key stakeholders (customers, business units, support teams) in project decision-making. They ensure stakeholder needs are understood, provide feedback, and facilitate alignment between project teams and business objectives.

### Responsibilities
- Represent stakeholder interests and requirements in planning
- Provide timely feedback on features and releases
- Facilitate communication between project team and stakeholders
- Validate that deliverables meet stakeholder expectations
- Escalate stakeholder concerns and blockers
- Participate in release planning and go/no-go decisions
- Conduct user acceptance testing or coordinate stakeholder validation
- Gather and communicate stakeholder feedback for continuous improvement

### Goals
- Ensure project outcomes align with stakeholder needs
- Enable rapid feedback loops between team and stakeholders
- Minimize surprises and misalignment on delivery
- Advocate for user experience and business value

### Typical Communication
- Weekly stakeholder updates and feedback sessions
- Participation in sprint reviews and demonstrations
- Release readiness reviews and acceptance sign-off
- Escalation of stakeholder concerns to project leadership

### Interactions with Other Roles
- **Product Managers**: Provides stakeholder feedback on priorities and requirements
- **QA Lead**: Participates in acceptance testing and validation
- **Release Manager**: Provides input on release timing and communication
- **Project Managers**: Communicates stakeholder concerns and dependencies
- **Developers**: Validates features meet stakeholder expectations

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

