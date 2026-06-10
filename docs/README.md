# OctoAcme Project Management Docs

## Overview

This README provides a summary of the OctoAcme project management framework and links to all detailed process documents. OctoAcme project management emphasizes:

- **Customer-first delivery** and measured outcomes
- **Lightweight planning** and iterative execution
- **Clear roles, risk management, and improvement cycles**

## OctoAcme Project Management Process Summary

OctoAcme follows a structured, lifecycle-based project management approach that emphasizes customer value, iterative delivery, and clear ownership. The framework is built on five core principles: customer-first prioritization, incremental delivery of testable features, named accountability for Project Managers and Product Leads, data-informed decision-making, and psychological safety for team feedback. This approach applies consistently across all cross-functional projects that deliver product features, services, and integrations, with key artifacts including project charters, roadmaps, sprint backlogs, risk registers, and retrospective documentation to maintain transparency and alignment throughout the project lifecycle.

### Key Roles and Communication Cadence

OctoAcme defines clear role-based personas—Developers, Product Managers, and Project Managers—each with distinct responsibilities that prevent silos and promote collaboration. Developers implement features while writing tests and participating in design reviews; Product Managers define what should be built based on customer and business value; and Project Managers coordinate delivery, manage risks, and facilitate communication. The communication rhythm is structured with daily standups (15 minutes focused on progress and blockers), weekly delivery syncs between PM and Product Lead, twice-weekly standups for delivery teams, monthly stakeholder updates, and ad-hoc escalations. This multi-level escalation path (team-level → PM → Product Lead → Sponsor) ensures risks are surfaced and resolved at appropriate levels without bottlenecks.

### Execution, Quality, and Risk Management

Execution follows a project lifecycle spanning Initiation, Planning, Execution, Release, and Close & Retrospective phases. During execution, teams use GitHub Projects boards with standardized columns (Backlog, Ready, In Progress, In Review, QA, Done) and enforce small pull requests (≤400 lines) with automated testing and linting in CI before requiring at least one approval. Quality assurance is multi-layered, including unit tests for new logic, integration tests where applicable, end-to-end smoke tests for critical flows before release, security scanning in CI, and manual QA for feature acceptance when needed. Risk management is continuous: risks are captured in a risk register (with ID, description, impact, likelihood, owner, and mitigation plan), monitored at weekly syncs, and escalated through defined channels. Release processes are standardized with pre-release requirements, deployment checklists, smoke tests, rollback plans, and post-deploy verification to minimize production incidents and ensure observability.

### Continuous Improvement and Learning

OctoAcme institutionalizes learning through mandatory retrospectives held after each sprint, release, or important milestone using a structured format (what went well, what could improve, action items with owners and due dates). Retrospectives are timeboxed (45–75 minutes), use anonymous idea boards to encourage candor, and prioritize 2–3 top action items to avoid overload. Action items are added to the project backlog with clear owners, due dates, and success criteria, and their impact is tracked in weekly PM syncs. This continuous improvement culture, combined with clear documentation stored in the `docs/` folder and standardized issue templates in `.github/ISSUE_TEMPLATE/`, ensures tacit knowledge is converted into searchable, versioned artifacts that accelerate onboarding, reduce single-person dependencies, and enable consistent, repeatable project execution across the organization.

## Quick Start

OctoAcme follows a structured lifecycle for all cross-functional projects:

1. **Initiation** — Validate business need, align stakeholders, define success metrics
2. **Planning** — Break work into shippable increments, identify risks and dependencies
3. **Execution** — Build, test, and iterate using daily standups and weekly syncs
4. **Release** — Deploy to production with safety checks and rollback plans
5. **Close & Retrospective** — Capture learnings and drive continuous improvement

## Core Principles

- **Clear Ownership** — Every project has a named Project Manager and Product Lead
- **Data-Informed Decisions** — Measure impact and iterate based on evidence
- **Psychological Safety** — Encourage feedback and learning
- **Iterative Delivery** — Deliver small, testable increments continuously
- **Transparency** — Keep stakeholders informed through regular communication

## Key Roles

- **Project Manager** — Coordinates delivery, schedules, risks, and communications
- **Product Manager** — Defines outcomes, prioritizes backlog, measures success
- **Developers** — Implement features, collaborate on design and testability
- **QA/Testing** — Validate quality and acceptance criteria

## Process Docs Index

### Foundational
- [**Project Management Overview**](octoacme-project-management-overview.md) — Introduction to how OctoAcme runs projects, core roles, and key artifacts

### Project Lifecycle
- [**Project Initiation Guide**](octoacme-project-initiation.md) — Initial steps to validate work, align stakeholders, create lightweight plan
- [**Project Planning**](octoacme-project-planning.md) — Turn approved initiatives into actionable plans and prioritized backlogs
- [**Execution & Tracking**](octoacme-execution-and-tracking.md) — Day-to-day execution management, team rhythm, quality assurance, blocker escalation
- [**Release & Deployment Guide**](octoacme-release-and-deployment.md) — Standardized release process, pre-release requirements, rollback playbook

### Cross-Cutting Concerns
- [**Risk Management & Communication**](octoacme-risks-and-communication.md) — Identify and manage risks, stakeholder communication, escalation paths
- [**Retrospective & Continuous Improvement**](octoacme-retrospective-and-continuous-improvement.md) — Capture learnings, run retrospectives, drive actionable improvements

### Reference
- [**Roles & Personas**](octoacme-roles-and-personas.md) — Detailed responsibilities and communication patterns for Developers, Product Managers, and Project Managers

## Communication Cadence

- **Daily** — 15-minute standups focused on progress, blockers, and dependencies
- **Weekly** — Delivery syncs between PM and Product Lead; project status updates
- **Monthly** — Stakeholder briefings and roadmap alignment
- **As-Needed** — Ad-hoc escalations for risks and blockers

## How to Use These Docs

1. **For a new project** — Start with [Project Initiation Guide](octoacme-project-initiation.md)
2. **For planning** — Read [Project Planning](octoacme-project-planning.md)
3. **During execution** — Refer to [Execution & Tracking](octoacme-execution-and-tracking.md) and [Risk Management & Communication](octoacme-risks-and-communication.md)
4. **Before release** — Review [Release & Deployment Guide](octoacme-release-and-deployment.md)
5. **After project completion** — Run [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md)
6. **For role clarity** — Consult [Roles & Personas](octoacme-roles-and-personas.md)

## Key Artifacts

Every OctoAcme project maintains:

- **Project Charter / One-pager** — Problem, goal, success metrics, stakeholders, timeline
- **Roadmap and Release Plan** — Milestones and delivery increments
- **Sprint/Iteration Backlog** — Prioritized work with acceptance criteria
- **Risk Register** — Identified risks with mitigation plans and status
- **Retrospective Notes** — Learnings and action items for continuous improvement

## Tips for Success

- Keep the Project Charter updated in your project repo
- Add process-specific docs to `.copilot/` if you want Copilot Spaces to use them as context
- Use issue templates in `.github/ISSUE_TEMPLATE/` for process documentation updates
- Review and discuss these docs during project kickoffs to align your team
- Update these docs based on retrospective feedback and team learnings

---

**Last Updated:** 2026-06-10

For questions or suggestions about these processes, please open an issue using the [Add Content to Project Management Process Docs template](.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml).
