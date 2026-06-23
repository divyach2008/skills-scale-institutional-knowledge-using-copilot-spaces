# OctoAcme — Incident Response & Communication Checklist

## Purpose
Provide a structured checklist for responding to production incidents, ensuring consistent communication, swift resolution, and effective post-incident learning.

## When to Use
- Production incidents affecting customer experience or service availability
- Security incidents or potential data breaches
- Major deployment failures or rollback scenarios
- Any issue escalated to critical severity

## Pre-Incident Preparation

### Team & Role Assignments
- [ ] Identify on-call rotation and escalation contacts
- [ ] Assign Incident Commander (IC) for large incidents
- [ ] Identify Technical Lead to coordinate engineering response
- [ ] Identify Communications Lead for stakeholder updates
- [ ] Identify SRE/DevOps lead for infrastructure and deployment
- [ ] Document escalation paths and contact information

### Documentation & Runbooks
- [ ] Maintain runbooks for common incidents (outages, data issues, security events)
- [ ] Document service dependencies and critical paths
- [ ] Maintain monitoring dashboards and alert definitions
- [ ] Document playbooks for rollback, failover, and emergency procedures
- [ ] Keep customer support playbooks for communication templates

### Infrastructure & Monitoring
- [ ] Ensure monitoring and alerting is comprehensive for critical services
- [ ] Verify dashboards are accessible and current
- [ ] Test backup and disaster recovery procedures regularly
- [ ] Document infrastructure access and credentials (secure storage)
- [ ] Establish communication channels for incident response (Slack, PagerDuty, etc.)

## Incident Response Phases

### Detection & Triage (0-5 minutes)
- [ ] Alert triggered or issue reported
- [ ] Page on-call engineer (SRE/DevOps)
- [ ] Acknowledge alert/ticket
- [ ] Quickly assess severity and scope
- [ ] Determine if incident or false alarm
- [ ] Document incident start time and initial observations

### Initial Assessment (5-15 minutes)
- [ ] Designate Incident Commander (for Sev1/critical incidents)
- [ ] Open war room or incident channel
- [ ] Gather initial telemetry and logs
- [ ] Identify affected services, features, or customer segments
- [ ] Estimate customer impact (number of users, transactions affected)
- [ ] Determine incident severity (Sev1/Critical, Sev2/High, Sev3/Medium, Sev4/Low)
- [ ] Notify relevant teams (engineering, SRE, product, support)

### Communication (ongoing)
- [ ] Send initial incident notification to stakeholders
- [ ] Provide regular status updates (every 15-30 min for Sev1, every 1-2 hours for Sev2)
- [ ] Update customer support with status and workarounds
- [ ] Communicate estimated time to resolution (if known)
- [ ] Be transparent about what is being investigated

### Investigation & Troubleshooting
- [ ] Gather logs and telemetry data
- [ ] Check recent deployments or changes
- [ ] Review monitoring dashboards for anomalies
- [ ] Check dependencies and external services
- [ ] Review error messages and stack traces
- [ ] Communicate progress and findings in war room
- [ ] Escalate if help is needed (call in other experts)

### Mitigation & Resolution
- [ ] Document potential solutions and trade-offs
- [ ] Implement quick fix or workaround if safe
- [ ] Roll back recent changes if identified as root cause
- [ ] Scale infrastructure if capacity is the issue
- [ ] Restart services if applicable
- [ ] Verify fix resolves the issue (monitor for 5-10 minutes)
- [ ] Confirm customer impact is resolved
- [ ] Document the resolution steps taken

### Validation & Stability Check
- [ ] Monitor key metrics for 15-30 minutes post-resolution
- [ ] Verify no cascading failures or side effects
- [ ] Confirm customer experience is back to normal
- [ ] Get sign-off from Incident Commander that incident is resolved
- [ ] Update incident record with resolution time

## Communication Templates

### Initial Incident Notification
```
⚠️ INCIDENT: [Service Name] - [Brief Description]
Severity: [Sev1/Critical | Sev2/High | Sev3/Medium]
Status: Investigating
Estimated Impact: [X customers, Y% of traffic, feature unavailable, etc.]
Started: [Time]
War Room: [Link/Channel]
Updates: Every 15 minutes
```

### Status Update
```
📊 INCIDENT UPDATE: [Service Name]
Status: [Investigating | Mitigating | Monitoring | Resolved]
Progress: [What we've found, what we're trying]
ETA: [If known]
Last Update: [Time]
Next Update: [Time]
```

### Resolution Notification
```
✅ INCIDENT RESOLVED: [Service Name]
Duration: [Start time] - [End time] (X minutes)
Root Cause: [Brief description]
Impact: [Customer impact summary]
Action: [What we did to resolve]
Post-Incident Review: Scheduled for [Date/Time]
```

## Post-Incident Checklist

### Immediate (same day)
- [ ] Close incident ticket and update status
- [ ] Send final incident notification to stakeholders
- [ ] Thank the team for their response
- [ ] Capture quick notes and timeline while fresh
- [ ] Document root cause findings
- [ ] Schedule post-incident review (within 24-48 hours)

### Post-Incident Review (1-2 days)
- [ ] Gather incident timeline and facts
- [ ] Review logs and telemetry data
- [ ] Conduct blameless retrospective with response team
- [ ] Identify root cause and contributing factors
- [ ] Document lessons learned
- [ ] Create action items to prevent recurrence
- [ ] Assign owners and target resolution dates for action items
- [ ] Share findings and action items with broader team

### Follow-up (1-4 weeks)
- [ ] Track progress on action items
- [ ] Update playbooks and runbooks based on learnings
- [ ] Improve monitoring and alerting if needed
- [ ] Share incident learnings with team (brown bag, wiki post, etc.)
- [ ] Close action items when complete

## Incident Severity Levels

### Sev1 / Critical
- Complete service outage affecting all customers
- Data loss or data breach
- Security incident requiring immediate action
- Major feature completely unavailable
- Response time: Page on-call immediately
- Communication: Continuous updates

### Sev2 / High
- Significant service degradation (>50% users affected or >50% performance degradation)
- Key features unavailable
- Response time: Page on-call within 5 minutes
- Communication: Updates every 15-30 minutes

### Sev3 / Medium
- Partial service degradation (<50% users affected)
- Non-critical features affected
- Response time: Page on-call within 30 minutes
- Communication: Updates every 1-2 hours

### Sev4 / Low
- Minor issues or cosmetic bugs
- No customer impact
- Response time: Create ticket, schedule for normal prioritization
- Communication: Updates in normal project channels

## Key Roles in Incident Response

### Incident Commander (IC)
- Owns overall incident coordination and communication
- Makes decisions on remediation strategies
- Escalates or deprioritizes based on impact
- Coordinates across teams
- Ensures post-incident review is scheduled and conducted

### Technical Lead / SRE
- Leads technical investigation and troubleshooting
- Proposes mitigation and resolution strategies
- Implements fixes
- Monitors for recurrence

### Communications Lead
- Manages stakeholder and customer communication
- Updates war room status
- Drafts status notifications
- Coordinates with support team

### Product Manager
- Provides business context on impact
- Helps prioritize customer communication
- Tracks customer feedback during incident

### Support Lead
- Communicates with customers
- Provides workarounds or guidance
- Escalates critical customer issues

## Related Documents
- OctoAcme Risk Management & Communication
- OctoAcme Execution & Tracking
- OctoAcme Release & Deployment
- Runbooks and playbooks (service-specific)
