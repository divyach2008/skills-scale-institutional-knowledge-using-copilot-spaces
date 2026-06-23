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

## Engineering Manager

### Role Summary
Engineering Managers own people management, capacity planning, and career growth for engineering team members. They ensure the team follows engineering best practices, maintains code quality, and delivers on commitments efficiently.

### Responsibilities
- Own people management, career development, and performance feedback
- Ensure the team follows engineering best practices and maintains code quality standards
- Plan and manage team capacity across projects and ongoing work
- Remove impediments and unblock technical bottlenecks
- Coordinate with other teams for resource constraints and dependencies
- Foster psychological safety and continuous learning culture

### Goals
- Develop high-performing, engaged engineering teams
- Deliver reliable, maintainable code at sustainable pace
- Reduce technical debt and improve team productivity

### Interactions
- Works with PM to ensure realistic team commitments and resource allocation
- Partners with PdM on prioritization trade-offs when capacity is constrained
- Collaborates with Developers and QA on technical debt decisions and release readiness
- Coordinates with other EMs on cross-team dependencies

### Typical Communication
- 1-on-1s with direct reports and team sync meetings
- Capacity planning and sprint commitment discussions
- Technical debt and prioritization trade-off conversations
- Cross-team coordination meetings

---

## Technical Program Manager

### Role Summary
Technical Program Managers coordinate cross-team technical dependencies, schedules, and integration work. They track progress on multi-team milestones and facilitate hand-offs between teams.

### Responsibilities
- Coordinate technical dependencies and integration work across teams
- Track progress on multi-team milestones and release timelines
- Run technical gating and hand-off ceremonies to ensure readiness
- Maintain the technical risk register and help escalate/unblock integration issues
- Document technical architecture decisions and integration points
- Monitor and communicate cross-team blockers and dependencies

### Goals
- Ensure on-time delivery of multi-team initiatives
- Reduce integration friction and rework
- Improve visibility into cross-team progress and risks

### Interactions
- Works with PM/PdM to align timelines, scope, and dependencies across teams
- Liaises with Engineering Managers and Tech Leads to ensure integration work is planned and tracked
- Coordinates with SREs on operational readiness and deployment coordination
- Partners with QA on end-to-end testing and acceptance criteria across teams

### Typical Communication
- Weekly cross-team dependency and integration sync meetings
- Technical design reviews and architecture decision docs
- Risk and blocker escalation reports
- Milestone tracking and hand-off ceremonies

---

## Site Reliability Engineer / DevOps

### Role Summary
Site Reliability Engineers (SREs) / DevOps engineers define and maintain production reliability standards, monitoring, and deployment safety. They own CI/CD pipeline reliability and participate in incident response.

### Responsibilities
- Define and maintain runbooks, Service Level Objectives (SLOs), and alerts for services
- Own CI/CD pipeline reliability, automated testing, and deployment automation
- Implement and monitor production observability (logs, metrics, traces)
- Establish and enforce deployment safety checks and automated rollback capabilities
- Participate in incident response, triage, and post-incident reviews
- Work on capacity planning and infrastructure scalability

### Goals
- Maintain high service availability and performance for production systems
- Reduce deployment risk and enable rapid, safe releases
- Improve mean-time-to-detection (MTTD) and mean-time-to-recovery (MTTR) for incidents

### Interactions
- Works with Developers and Engineering Managers on capacity, resiliency, and observability work
- Coordinates with PM on release windows, deployment schedules, and operational readiness criteria
- Partners with Security Engineers on compliance monitoring and security observability
- Collaborates with QA on smoke tests and post-deployment verification

### Typical Communication
- On-call rotations and incident response channels
- Deployment coordination and release readiness reviews
- Infrastructure and observability design discussions
- Post-incident retrospectives and action item tracking

---

## UX Researcher / Designer

### Role Summary
UX Researchers and Designers lead user research, usability testing, and design validation for features. They produce UX artifacts and ensure acceptance criteria reflect user experience requirements.

### Responsibilities
- Lead user research, interviews, and usability testing
- Create design artifacts (wireframes, prototypes, design systems)
- Validate designs through user research and iterative testing
- Define UX-related acceptance criteria and design specifications
- Document design decisions and patterns for consistency
- Participate in design reviews and provide design feedback

### Goals
- Deliver user-centered, accessible, and delightful product experiences
- Reduce rework and improve design quality through early validation
- Build consistent, reusable design patterns

### Interactions
- Works with PdM to shape product decisions based on research insights and user feedback
- Collaborates with Developers and QA to ensure design fidelity and usability acceptance
- Participates in sprint planning to communicate design constraints and opportunities
- Partners with Developers on design system and component implementation

### Typical Communication
- Design reviews and critique sessions
- User research findings and recommendations
- Design specs and component documentation
- Sprint planning and design refinement discussions

---

## Security Engineer

### Role Summary
Security Engineers provide security reviews, threat modeling, and approval gates for releases. They own security findings remediation and ensure compliance with security standards.

### Responsibilities
- Conduct security reviews and threat modeling for new features and system changes
- Provide security approval gates before releases to production
- Track and prioritize security findings and vulnerabilities
- Develop and maintain security playbooks and runbooks
- Provide security guidance and best practices to development teams
- Conduct security training and raise security awareness

### Goals
- Prevent security incidents and data breaches
- Integrate security early in the development process (shift-left)
- Maintain compliance with security standards and regulations

### Interactions
- Coordinates with PM/PdM and Engineering Managers to ensure security signoff prior to release
- Works with Developers to remediate vulnerabilities and incorporate secure design practices
- Partners with SREs on security monitoring and incident response
- Collaborates with Data Engineers on data security and privacy controls

### Typical Communication
- Security review meetings and threat modeling sessions
- Vulnerability tracking and remediation status updates
- Security training and awareness sessions
- Incident response and security incident playbooks

---

## Data Analyst / Data Engineer

### Role Summary
Data Analysts and Data Engineers define key metrics, instrument telemetry, and own data quality for product metrics. They build dashboards and provide analysis to drive data-informed decision-making.

### Responsibilities
- Define key metrics and success indicators aligned with business and product goals
- Design and implement telemetry instrumentation across products and services
- Build and maintain dashboards, reports, and analytical models
- Ensure data quality, accuracy, and timeliness
- Provide data analysis and insights to support decision-making
- Document data pipelines and maintain data lineage

### Goals
- Enable data-driven decision-making across the organization
- Provide accurate, timely insights into product performance and customer behavior
- Build scalable, reliable data infrastructure

### Interactions
- Partners with PdM to define success metrics and with PM to include metrics in project one-pagers
- Works with Developers to implement instrumentation and event logging
- Collaborates with QA to validate data pipelines and metric accuracy
- Partners with Product Managers on analysis and insights for retrospectives

### Typical Communication
- Metrics definition and instrumentation planning meetings
- Dashboard reviews and metric deep-dives
- Data quality and pipeline status updates
- Analysis presentations and insights sharing

---

## Customer Support / Success Lead

### Role Summary
Customer Support and Success Leads capture customer-reported issues and trends, own customer communication, and escalate high-impact issues. They provide critical context during incident response.

### Responsibilities
- Capture and triage customer-reported issues, bugs, and feature requests
- Track customer impact and prioritization of issues
- Communicate with customers about status, workarounds, and resolutions
- Escalate high-impact incidents and provide customer context during triage
- Identify patterns and trends in customer issues for prioritization
- Serve as voice of the customer in product and engineering discussions

### Goals
- Deliver excellent customer experience and satisfaction
- Reduce customer-impacting issues through early escalation and communication
- Drive product improvements based on customer feedback and trends

### Interactions
- Works with PM and SRE during incidents to provide customer impact context and communicate status
- Partners with PdM on customer-impacting prioritization and feature decisions
- Shares recurring issues and customer feedback to drive backlog prioritization
- Collaborates with Developers on issue reproduction and root cause analysis

### Typical Communication
- Customer issue tickets and escalation channels
- Customer communication and status updates
- Incident response and post-incident reviews
- Product and engineering feedback channels

---

## Role Interactions & Handoffs

### Project Initiation
- PdM defines problem and goals
- PM creates project charter and stakeholder plan
- EM ensures team availability and capacity

### Planning & Design
- PdM and Designers collaborate on user research and design
- PM works with EM on team capacity and resource allocation
- TPM (for multi-team efforts) maps dependencies and timelines

### Execution
- Developers implement features
- Designers review implementation for design fidelity
- SREs ensure CI/CD pipeline supports fast, safe releases
- Data Engineers instrument telemetry

### Quality & Release
- QA validates acceptance criteria
- Security Engineer approves security readiness
- SRE ensures operational readiness
- PM/PdM coordinate release and stakeholder communication

### Production & Monitoring
- SREs monitor production systems and alert on issues
- Data Analysts track key metrics and product health
- Support Lead communicates customer impact during incidents
- Engineers respond to and triage issues

### Learning & Improvement
- Retrospectives capture learnings across all roles
- Data Analysts provide metrics on project outcomes
- Support Lead shares customer feedback
- Action items drive continuous improvement

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- Refer to this document when documenting processes to ensure clarity about role ownership and handoffs.
