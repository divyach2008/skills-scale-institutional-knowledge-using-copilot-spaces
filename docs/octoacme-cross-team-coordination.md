# OctoAcme — Cross-Team Coordination Checklist

## Purpose
Provide a practical checklist for coordinating work across multiple teams, ensuring handoffs are clear and dependencies are managed effectively.

## When to Use
- Multi-team projects or initiatives
- Projects with cross-team dependencies
- During planning phase to identify integration points
- During execution to track handoff readiness

## Pre-Planning Checklist

### Stakeholder & Role Identification
- [ ] Identify all teams involved in the project
- [ ] Map primary owner for each team (usually an Engineering Manager or Tech Lead)
- [ ] Designate a Technical Program Manager (TPM) or DRI for cross-team coordination
- [ ] Confirm Product Manager (PdM) and Project Manager (PM) are assigned
- [ ] Identify Security Engineer and SRE points of contact for early involvement

### Dependency Mapping
- [ ] Document technical dependencies between teams
- [ ] Identify shared services, APIs, or infrastructure that will be used
- [ ] List integration points and data flows between systems
- [ ] Note any shared data or configuration changes needed
- [ ] Flag external system dependencies or third-party integrations

### Timeline & Milestones
- [ ] Define critical path and sequential vs. parallel work streams
- [ ] Establish hand-off milestones (e.g., API contract defined, alpha integration, beta launch)
- [ ] Identify any hard constraints (e.g., compliance deadlines, infrastructure limits)
- [ ] Schedule dependency-driven reviews or gating ceremonies
- [ ] Build in buffer time for integration and testing

## Planning Phase Checklist

### Design & Specification
- [ ] Conduct technical design review with all team representatives
- [ ] Document API contracts and integration interfaces
- [ ] Define data schemas and integration protocols
- [ ] Agree on error handling and failure modes
- [ ] Document version compatibility and backward compatibility requirements
- [ ] Security & Compliance signoff on design

### Acceptance Criteria & Testing
- [ ] Define end-to-end acceptance criteria that span teams
- [ ] Plan integration testing strategy (who, when, where)
- [ ] Identify data fixtures or test environments needed
- [ ] Plan smoke tests for post-deployment verification
- [ ] Document rollback and mitigation procedures

### Risk Identification
- [ ] Identify technical risks and mitigation plans
- [ ] Flag resource or capacity risks (e.g., shared infrastructure, key person dependencies)
- [ ] Note schedule risks and dependency chain risks
- [ ] Assign owners and target resolution dates for high-risk items
- [ ] Document escalation paths if risks materialize

### Communication Plan
- [ ] Schedule kickoff meeting with all teams
- [ ] Establish regular cross-team sync cadence (weekly recommended)
- [ ] Create central artifact location (e.g., GitHub project, wiki, shared doc)
- [ ] Define escalation channels for blockers
- [ ] Agree on status update format and reporting cadence

## Execution Phase Checklist

### Weekly Coordination Sync
- [ ] Review progress on each team's work stream
- [ ] Check blockers and dependencies from last week
- [ ] Identify new blockers or risks that emerged
- [ ] Confirm upcoming hand-off readiness and timelines
- [ ] Update shared project status and risk register
- [ ] Escalate unresolved issues to PM/PdM/sponsors

### Integration Checkpoints
- [ ] Confirm API contracts are finalized and tested
- [ ] Verify staging environment readiness for integration testing
- [ ] Test integration with shared services or infrastructure
- [ ] Validate data flows and error handling
- [ ] Confirm all teams' CI/CD pipelines are working
- [ ] Review security and compliance checklist

### Handoff Readiness
- [ ] Confirm code is merged to main/release branch
- [ ] Verify all tests pass (unit, integration, end-to-end)
- [ ] Confirm documentation is complete and up-to-date
- [ ] Validate runbooks and monitoring are in place
- [ ] Get sign-off from QA, Security, and SRE
- [ ] Confirm release notes are drafted

### Communication & Transparency
- [ ] Update stakeholders on progress and timeline
- [ ] Communicate any timeline changes or risks proactively
- [ ] Share release plan and go/no-go criteria with all teams
- [ ] Prepare customer/support communication if needed
- [ ] Schedule release window and communicate to all teams

## Release & Deployment Checklist

### Pre-Deployment
- [ ] Confirm all acceptance criteria are met
- [ ] Complete security and compliance reviews
- [ ] Verify monitoring and alerts are configured
- [ ] Confirm SRE has validated deployment procedures
- [ ] Schedule communication and status update channels
- [ ] Identify rollback owner and rollback procedures

### Deployment Execution
- [ ] Deploy to staging and run smoke tests
- [ ] Coordinate deployment order if there are dependencies
- [ ] Verify all services are healthy post-deployment
- [ ] Monitor key metrics and error rates
- [ ] Maintain open communication channels during deployment
- [ ] Confirm post-deployment verification is complete

### Post-Deployment
- [ ] Announce successful deployment to stakeholders
- [ ] Monitor metrics and customer impact for 24-48 hours
- [ ] Document any issues encountered and how they were resolved
- [ ] Gather feedback from teams on coordination and handoffs
- [ ] Schedule retrospective with all team representatives

## Retrospective & Learning Checklist

### Retrospective Meeting
- [ ] Schedule within 1-2 weeks of deployment
- [ ] Invite representatives from all teams
- [ ] Review what went well and what could improve
- [ ] Document lessons learned on coordination and handoffs
- [ ] Identify action items to improve future cross-team work

### Action Items & Follow-up
- [ ] Assign owners and due dates to action items
- [ ] Track action items in the project backlog
- [ ] Review progress on action items in weekly sync for 4 weeks post-project
- [ ] Update process documentation based on learnings

## Key Roles & Responsibilities in Cross-Team Coordination

### Technical Program Manager (TPM)
- Owns overall cross-team coordination
- Facilitates weekly syncs and removes blockers
- Maintains dependency map and critical path
- Escalates risks and timeline impacts

### Product Manager (PM) / Project Manager
- Ensures scope and timeline alignment
- Communicates with stakeholders
- Makes prioritization decisions on trade-offs
- Coordinates release communication

### Engineering Manager (EM) per team
- Commits team capacity and resources
- Removes internal team blockers
- Ensures design and code quality standards
- Communicates team status and risks

### Security Engineer
- Reviews integration points for security risks
- Provides security approval before release
- Ensures compliance with security standards

### Site Reliability Engineer (SRE) / DevOps
- Validates operational readiness
- Ensures CI/CD pipeline reliability
- Owns deployment and rollback procedures
- Monitors production systems

## Common Pitfalls to Avoid

- **Unclear Ownership**: Ensure one owner per component/team; avoid "everyone owns it"
- **Late Integration Testing**: Start integration testing early (staging environment)
- **Poor Communication**: Over-communicate status, risks, and changes
- **Missing Acceptance Criteria**: Define end-to-end acceptance criteria, not just per-team
- **No Rollback Plan**: Always have a documented, tested rollback procedure
- **Skipping Retrospectives**: Capture learnings to improve future cross-team efforts
- **Inadequate Monitoring**: Ensure observability is built in, not added at the end

## Related Documents
- OctoAcme Project Planning
- OctoAcme Execution & Tracking
- OctoAcme Roles & Personas
- OctoAcme Risk Management & Communication
