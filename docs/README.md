# OctoAcme Project Management Documentation

Welcome to the OctoAcme project management knowledge base. This documentation centralizes our proven approaches to running successful, customer-focused projects.

## Quick Start

- **New to OctoAcme projects?** Start with [Project Management Overview](./octoacme-project-management-overview.md)
- **Starting a new project?** Follow the [Project Initiation Guide](./octoacme-project-initiation.md)
- **Ready to plan execution?** See [Project Planning](./octoacme-project-planning.md)
- **Running a project now?** Check [Execution & Tracking](./octoacme-execution-and-tracking.md)

## Core Principles

- **Customer-first**: Prioritize customer value and usability
- **Iterative delivery**: Deliver small, testable increments
- **Clear ownership**: Each project has named PM and Product Lead
- **Data-informed decisions**: Measure impact and iterate based on evidence
- **Psychological safety**: Encourage feedback and learning

## OctoAcme Project Management Overview

OctoAcme follows a structured, iterative project management approach designed around customer-first delivery, clear ownership, and data-informed decisions. The organization operates with defined roles—Project Managers (PMs) coordinate delivery and timelines, Product Managers define outcomes and prioritize work, and Developers implement features with quality standards. Projects progress through five key lifecycle phases: **Initiation** (validating business need and stakeholder alignment), **Planning** (breaking work into shippable increments with acceptance criteria), **Execution** (day-to-day build and delivery), **Release** (standardized deployment to production), and **Close & Retrospective** (capturing learnings).

### Execution & Quality Workflows

During execution, teams maintain a consistent rhythm of **daily standups (15 minutes)**, **weekly delivery syncs**, and **sprint demos**, using GitHub Projects with workflow columns (Backlog → Ready → In Progress → In Review → QA → Done). Pull requests follow strict conventions—limited to ≤400 lines when possible, requiring issue links and acceptance criteria in descriptions, automated testing/linting via CI, and at least one approval before merge. Quality assurance is embedded throughout: unit tests for new logic, integration and end-to-end smoke tests for critical flows, security scanning in CI, and manual QA for feature acceptance. Blockers are triaged in a three-level escalation model: team-level triage in standups, PM escalation to Product Leads and dependent teams, and sponsor-level escalation for business-impacting issues. Teams track velocity, burndown, and key success metrics using dashboards to maintain visibility.

### Risk Management & Communication

OctoAcme maintains a formal **Risk Register** updated weekly with ID, description, impact/likelihood, owner, mitigation plan, and status. Risks are identified during planning and ongoing execution, assessed for priority, and monitored through regular syncs. Communication is structured around stakeholder groups with regular updates (weekly or milestone-based) from a single source of truth—typically the project README or release documentation. Templates standardize communication: weekly status updates highlight progress, next steps, risks, and decisions needed; incident communications include triage summaries, expected timelines, and post-incident retrospectives. Release deployment follows a documented checklist including acceptance criteria verification, CI/security scan passing, smoke test preparation, rollback plans, and staged deployment (staging → production) with post-deploy verification and stakeholder announcements.

### Continuous Improvement & Learning Culture

Retrospectives occur after each sprint, release, or significant milestone, structured around what went well, what could improve, and 2–3 prioritized action items with clear owners and due dates. These action items feed back into the project backlog or GitHub issues, ensuring accountability and measurement of impact. This continuous improvement cycle—combined with psychological safety that encourages feedback—enables teams to iteratively refine processes, reduce single-person dependency risks, and accelerate onboarding through well-documented, versioned artifacts stored in the repository's `docs/` folder and Copilot Spaces context.

## Documentation Index

### Foundational
- [Project Management Overview](./octoacme-project-management-overview.md) — High-level introduction to OctoAcme's approach, roles, and key artifacts
- [Roles & Personas](./octoacme-roles-and-personas.md) — Definitions of typical roles and responsibilities

### Project Lifecycle
- [Project Initiation](./octoacme-project-initiation.md) — Validate business need and authorize work
- [Project Planning](./octoacme-project-planning.md) — Turn approved initiatives into actionable plans
- [Execution & Tracking](./octoacme-execution-and-tracking.md) — Manage day-to-day execution and track progress
- [Release & Deployment](./octoacme-release-and-deployment.md) — Standardize releases to production
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) — Capture learnings and drive improvements

### Cross-Cutting Concerns
- [Risk Management & Communication](./octoacme-risks-and-communication.md) — Identify, manage, and communicate risks and dependencies

## How to Use This Documentation

- Keep documents updated as processes evolve
- Link to specific sections when discussing projects
- Use as a reference during project kickoffs and team onboarding
- Contribute improvements through the [Add Content to Process Docs](../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) issue template

## Quick Navigation by Role

### For Developers
Start with [Roles & Personas](./octoacme-roles-and-personas.md) to understand your responsibilities, then review:
- [Execution & Tracking](./octoacme-execution-and-tracking.md) — PR workflows, testing, and quality standards
- [Release & Deployment](./octoacme-release-and-deployment.md) — Deployment processes and incident response

### For Product Managers
Begin with [Project Management Overview](./octoacme-project-management-overview.md), then focus on:
- [Project Initiation](./octoacme-project-initiation.md) — Creating project charters and one-pagers
- [Project Planning](./octoacme-project-planning.md) — Building backlogs and defining success metrics
- [Risk Management & Communication](./octoacme-risks-and-communication.md) — Stakeholder alignment and risk tracking

### For Project Managers
Review [Project Management Overview](./octoacme-project-management-overview.md) first, then explore:
- [Project Initiation](./octoacme-project-initiation.md) — Kickoff and stakeholder alignment
- [Project Planning](./octoacme-project-planning.md) — Timeline and milestone management
- [Execution & Tracking](./octoacme-execution-and-tracking.md) — Team rhythm and blocker escalation
- [Risk Management & Communication](./octoacme-risks-and-communication.md) — Risk registers and status updates
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) — Post-project learning and action items

## Contributing to OctoAcme Documentation

To propose updates or add new process documentation:

1. Use the [Add Content to Project Management Process Docs](../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) issue template
2. Provide a summary of the change, rationale, and suggested content
3. Ensure alignment with existing processes and team feedback
4. Updates are reviewed and merged to maintain documentation quality

---

**Last updated**: July 2026  
**Maintainer**: OctoAcme Project Management Team
