# OctoAcme Project Management Documentation

## Overview

OctoAcme uses a structured project management approach designed for cross-functional teams delivering product features, services, and integrations. Our methodology emphasizes customer value, iterative delivery, clear ownership, and data-informed decisions with a focus on psychological safety and continuous improvement.

This documentation serves as the central index and reference guide for all OctoAcme project management processes, helping team members understand our framework, navigate to relevant guidance, and maintain consistent execution across projects.

## Core Principles

- **Customer-first**: Prioritize customer value and usability in all delivery decisions
- **Iterative delivery**: Deliver small, testable increments to gather feedback and reduce risk
- **Clear ownership**: Each project has named PM and Product Lead roles with explicit accountability
- **Data-informed decisions**: Measure impact and iterate based on evidence and metrics
- **Psychological safety**: Encourage feedback, learning, and blameless retrospectives

## OctoAcme Project Management Processes

OctoAcme's project management operates through a structured lifecycle that ensures alignment, quality, and continuous improvement at every stage.

### Key Workflows and Execution Model

OctoAcme projects follow a five-phase lifecycle: initiation, planning, execution, release, and close/retrospective. Each phase has clear checkpoints and deliverables to ensure work stays aligned with business objectives and team capacity.

**Initiation** begins by validating the business need through a lightweight project one-pager that confirms success metrics, identifies stakeholders, and makes a go/no-go decision before committing to planning. Once approved, the **Planning** phase turns the initiative into an actionable backlog with prioritized work, clear milestones, dependencies, risks, and an agreed definition of done.

During **Execution**, the team manages day-to-day delivery through structured communication rhythms: daily standups (15 min) focus on progress and blockers, weekly delivery syncs review updates and health, and demo/review sessions surface progress. Work is tracked on a project board with columns such as Backlog, Ready, In Progress, In Review, QA, and Done. Pull requests are expected to be small (≤400 lines when possible), linked to issues, and accompanied by acceptance criteria.

**Release** standardizes how features move to production. Before deployment, the team verifies that acceptance criteria are met, CI/security scans pass, release notes are drafted, and rollback plans exist. After release, the team runs post-deploy verifications and announces the release to stakeholders.

Finally, **Retrospectives** capture lessons learned after sprints, releases, or milestones, converting insights into actionable improvements that feed back into future planning cycles.

### Roles and Personas

OctoAcme operates with clear role definitions to ensure accountability and collaboration:

- **Project Manager (PM)**: Coordinates delivery, manages schedules, risks, and communications. Ensures transparency and escalates blockers.
- **Product Manager (PdM)**: Defines outcomes, prioritizes the backlog, and measures success. Owns product vision and customer/business alignment.
- **Developers**: Implement features, collaborate on design and testability, contribute to quality standards, and identify technical risks.
- **QA/Testing**: Validates quality against acceptance criteria and confirms Definition of Done before production.
- **Stakeholders**: Provide inputs, approvals, and business context; receive regular updates and participate in decision gates.

For detailed responsibilities and communication patterns, see [OctoAcme Personas](./octoacme-roles-and-personas.md).

### Communication Cadence and Quality Assurance

Consistent, predictable communication keeps projects aligned and risks visible:

- **Daily standup** (15 min): Progress, blockers, dependencies
- **Weekly PM + PdM sync**: Delivery status, risks, decisions
- **Twice-weekly team standup**: Execution updates (or as agreed)
- **Weekly stakeholder updates**: Status, risks, escalations
- **Sprint/milestone review**: Demo and feedback on completed work

Quality is built into execution, not added at the end. New logic requires unit tests; integration tests are used where applicable; end-to-end smoke tests run on critical flows; security scanning executes in CI; and manual QA validates real-world acceptance. Automated linting and testing run in CI before PR approval, with a requirement for at least one approval before merge. Small PRs reduce review burden and defect risk.

### Risk Management and Escalation

Risks are captured in a simple register with ID, description, impact, likelihood, owner, mitigation plan, and status. Risks are reviewed weekly during syncs and updated as conditions change. Escalation follows a clear path: team-level triage in daily standup → PM escalates to Product Lead and dependent teams → sponsor-level escalation for business-impacting issues.

---

## Project Lifecycle & Process Docs

### 1. [Project Initiation Guide](./octoacme-project-initiation.md)
**When**: When a new project idea or feature proposal is ready to be explored  
**Purpose**: Validate business need, identify stakeholders, define success criteria, and make a go/no-go decision  
**Key deliverables**: Project one-pager, stakeholder list, initial timeline, risk list, resource needs

### 2. [Project Planning](./octoacme-project-planning.md)
**When**: After initiation approval  
**Purpose**: Turn an approved initiative into an actionable plan with prioritized backlog and milestones  
**Key deliverables**: Prioritized backlog with acceptance criteria, release plan, definition of done, risk register

### 3. [Execution & Tracking](./octoacme-execution-and-tracking.md)
**When**: During active delivery  
**Purpose**: Manage day-to-day execution, track progress toward milestones, and escalate risks  
**Key practices**: Daily standups (15 min), weekly delivery syncs, small PRs (≤400 lines), automated testing in CI, blocker escalation

### 4. [Release & Deployment Guide](./octoacme-release-and-deployment.md)
**When**: When ready to ship to production  
**Purpose**: Standardize release types, pre-release requirements, and deployment procedures  
**Key practices**: Release types (patch, minor, major), pre-release checklist, smoke tests, rollback plans, incident playbooks

### 5. [Risk Management & Communication](./octoacme-risks-and-communication.md)
**When**: Throughout the project lifecycle  
**Purpose**: Identify, assess, and mitigate risks; maintain stakeholder alignment  
**Key practices**: Risk register (ID, description, impact, likelihood, owner, mitigation), escalation paths, stakeholder status templates

### 6. [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)
**When**: After sprints, releases, or important milestones  
**Purpose**: Capture learnings and convert them into actionable improvements  
**Key practices**: Structured retrospectives (45–75 min), action item tracking, impact measurement

### 7. [Project Management Overview](./octoacme-project-management-overview.md)
**Quick reference**: High-level introduction to OctoAcme approach, roles, key artifacts, and communication cadence

## Getting Started

**New to OctoAcme?**
1. Start with [Project Management Overview](./octoacme-project-management-overview.md) for a concise 5-minute introduction
2. Review [OctoAcme Personas](./octoacme-roles-and-personas.md) to understand your role and responsibilities

**Starting a new project?**
1. Follow the [Project Initiation Guide](./octoacme-project-initiation.md)
2. Once approved, move to [Project Planning](./octoacme-project-planning.md)
3. Use the Project One-pager template as your charter document

**Managing execution on an active project?**
1. Refer to [Execution & Tracking](./octoacme-execution-and-tracking.md) for day-to-day practices
2. Use [Risk Management & Communication](./octoacme-risks-and-communication.md) to maintain stakeholder alignment
3. Review the weekly sync template for status reporting

**Preparing for release?**
1. See [Release & Deployment Guide](./octoacme-release-and-deployment.md)
2. Complete the pre-release checklist
3. Prepare release notes and rollback plans

**Capturing learnings?**
1. Schedule a retrospective per [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)
2. Convert action items into issues or backlog work items
3. Track improvements in the weekly PM sync

## How Copilot Spaces Uses This Documentation

These process documents are structured to be attached to Copilot Spaces, providing AI-assisted guidance for:
- Project managers planning and executing projects
- Product managers defining scope and success metrics
- Developers understanding quality standards and delivery practices
- New team members onboarding to OctoAcme methodology

To use OctoAcme processes in Copilot Spaces, attach the relevant process docs from this folder. Copilot will provide context-aware guidance aligned with our established practices and principles.

## Contributing to OctoAcme Process Docs

To suggest updates or additions to process documentation:
1. Create an issue using the [Add Content to Process Docs](../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) template
2. Include a summary of the proposed change and rationale
3. Reference which process doc should be updated
4. Participate in review and refinement
5. Once approved, submit a PR with your changes

## Questions or Need Help?

- **New to the framework?** Start with the [Project Management Overview](./octoacme-project-management-overview.md)
- **Stuck on a phase?** Refer to the specific phase document or reach out to your Project Manager
- **Want to propose a process improvement?** Use the [Add Content to Process Docs](../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) issue template
