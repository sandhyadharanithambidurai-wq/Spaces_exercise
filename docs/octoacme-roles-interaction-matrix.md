# OctoAcme Roles Interaction Matrix

## Purpose
This matrix clarifies how OctoAcme roles interact, communicate, and collaborate during project execution. Use this to understand dependencies, clarify decision authority, and ensure smooth handoffs.

---

## Role Interaction Overview

| **From ↓ / To →** | **Developer** | **QA/Testing Lead** | **Technical Lead** | **Product Manager** | **Project Manager** | **Stakeholder/Sponsor** | **Scrum Master** |
|---|---|---|---|---|---|---|---|
| **Developer** | Code review, pairing | Implement test feedback | Get design guidance | Clarify requirements | Report blockers | — | Ask for impediment help |
| **QA/Testing Lead** | Share test results, acceptance criteria | Coordinate test strategy | Collaborate on testability | Refine acceptance criteria | Report quality status | Escalate quality blocker | Escalate quality blocker |
| **Technical Lead** | Mentor, code review | Advise on testability | Align on architecture | Technical feasibility check | Escalate technical risks | Communicate trade-offs | — |
| **Product Manager** | Provide requirements | Define success metrics | Feasibility discussion | Prioritization, backlog | Status update | Business alignment | Backlog refinement |
| **Project Manager** | Schedule, resource | Schedule | Schedule | Sync on status | Coordinate cross-team | Escalate issues, reports | Coordinate ceremonies |
| **Stakeholder/Sponsor** | — | — | — | Roadmap approval | Sign-off, priority | Strategic alignment | — |
| **Scrum Master** | Facilitate planning | Facilitate ceremonies | Facilitate ceremonies | Facilitate ceremonies | Facilitate ceremonies | — | — |

---

## Key Communication Flows

### Backlog & Requirements
```
Stakeholder/Sponsor (defines objectives)
    ↓
Product Manager (prioritizes & adds acceptance criteria)
    ↓
QA/Testing Lead (refines test scenarios)
    ↓
Technical Lead (reviews feasibility)
    ↓
Developer (implements) + Scrum Master (facilitates planning)
```

### Quality & Testing
```
Developer (writes code)
    ↓
QA/Testing Lead (executes tests, identifies issues)
    ↓
Developer (fixes defects, works with QA)
    ↓
QA/Testing Lead (re-tests, signs off)
    ↓
Project Manager (reports quality status)
```

### Risk & Escalation
```
Developer / QA/Testing Lead (identifies issue)
    ↓
Technical Lead or Project Manager (triages)
    ↓
Project Manager (escalates if needed)
    ↓
Stakeholder/Sponsor (approves mitigation or trade-off)
```

### Release & Go-Live
```
QA/Testing Lead (quality sign-off)
    ↓
Technical Lead (technical readiness check)
    ↓
Project Manager (coordinates deployment window)
    ↓
Stakeholder/Sponsor (approves release)
    ↓
Team (executes deployment)
    ↓
Product Manager (announces to market/customers)
```

---

## Decision Authority by Role

| **Decision Type** | **Owner** | **Consulted** | **Informed** |
|---|---|---|---|
| What to build (roadmap priority) | Product Manager + Stakeholder/Sponsor | Project Manager, Technical Lead | Entire team |
| How to build (technical approach) | Technical Lead | Developers, QA Lead | Product Manager, Project Manager |
| Quality acceptance | QA/Testing Lead | Developers, Product Manager | Project Manager |
| Release approval | Stakeholder/Sponsor | Product Manager, Technical Lead | Entire team |
| Scope changes | Stakeholder/Sponsor + Product Manager | Project Manager, Technical Lead | Entire team |
| Process improvements | Scrum Master + Team | Project Manager | Stakeholder/Sponsor |
| Risk mitigation | Project Manager + Technical Lead | Developers, QA Lead | Stakeholder/Sponsor |

---

## Communication Frequency by Relationship

| **Relationship** | **Frequency** | **Format** | **Topics** |
|---|---|---|---|
| Developer ↔ QA Lead | Daily (as needed) | PR feedback, test results, chat | Test failures, acceptance criteria, edge cases |
| Developer ↔ Technical Lead | 2–3x per week | Design review, code review, chat | Architecture, patterns, technical debt |
| QA Lead ↔ Product Manager | 2x per week | Sprint planning, sync | Acceptance criteria, test scenarios, priorities |
| QA Lead ↔ Project Manager | Weekly | Execution sync | Quality metrics, blockers, release readiness |
| Technical Lead ↔ Project Manager | Weekly | Risk register review | Technical risks, dependencies, mitigation status |
| Project Manager ↔ Stakeholder/Sponsor | Weekly–Monthly | Status update | Progress, blockers, scope/timeline changes |
| Product Manager ↔ Stakeholder/Sponsor | Bi-weekly–Monthly | Roadmap sync, review | Priorities, market feedback, business alignment |
| Scrum Master ↔ Entire Team | Daily | Standups, ceremonies | Blockers, sprint health, process improvements |

---

## Handoff Checklist by Phase

### Project Initiation
- [ ] Stakeholder/Sponsor & Product Manager define objectives and success metrics
- [ ] Project Manager creates project plan with team input
- [ ] Technical Lead assesses feasibility and technical risks
- [ ] Scrum Master schedules ceremonies and introduces agile practices

### Planning
- [ ] Product Manager prioritizes backlog with input from Technical Lead
- [ ] QA Lead drafts test strategy aligned with acceptance criteria
- [ ] Developers estimate work with support from Technical Lead
- [ ] Project Manager communicates plan to Stakeholder/Sponsor

### Execution (Sprint/Iteration)
- [ ] Scrum Master facilitates daily standups and ceremonies
- [ ] Developers implement features with code review from Technical Lead
- [ ] QA Lead executes tests and reports results
- [ ] Project Manager tracks progress and escalates blockers

### Quality Gate & Release Prep
- [ ] QA Lead confirms all acceptance criteria met and tests pass
- [ ] Technical Lead reviews code quality and architecture compliance
- [ ] Product Manager confirms feature readiness
- [ ] Project Manager coordinates release schedule

### Go-Live
- [ ] Project Manager executes deployment with team support
- [ ] QA Lead runs post-deployment verification
- [ ] Product Manager announces release to stakeholders/customers
- [ ] Stakeholder/Sponsor receives go-live confirmation

### Retrospective
- [ ] Scrum Master facilitates retrospective with entire team
- [ ] Team captures learnings and action items
- [ ] Project Manager tracks action items to completion
- [ ] Stakeholder/Sponsor receives project close-out summary

---

## Tips for Smooth Collaboration

1. **Be explicit about decisions**: Use the Decision Authority table to clarify who owns each decision
2. **Communicate across role boundaries**: Don't assume someone knows—communicate across the matrix
3. **Escalate early**: If a decision is blocking progress, escalate immediately rather than waiting
4. **Share context**: When handing off work, include relevant background, assumptions, and constraints
5. **Use this matrix in kickoffs**: Walk through the matrix with the team to set expectations for how roles will interact
6. **Update as needed**: If the team finds a different interaction pattern works better, update this matrix and share learnings
