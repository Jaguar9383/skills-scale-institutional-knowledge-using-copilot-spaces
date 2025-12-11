# OctoAcme Project Management Process

This README provides a concise overview of OctoAcme's project management processes, enabling new contributors and teammates to quickly understand our approach to delivering high-quality products. Our processes are designed to support customer-first, iterative delivery with clear ownership, data-informed decisions, and psychological safety across all cross-functional projects.

## Principles and Core Roles

**Key Principles:**
- **Customer-first**: Prioritize customer value and usability in all decisions
- **Iterative delivery**: Ship small, testable increments to gather feedback early
- **Clear ownership**: Every project has a named Project Manager (PM) and Product Manager (PdM)
- **Data-informed decisions**: Measure impact and iterate based on evidence
- **Psychological safety**: Encourage feedback, learning, and continuous improvement

**Core Roles:**
- **Project Manager (PM)**: Coordinates delivery, schedules, risk management, and communications
- **Product Manager (PdM)**: Defines outcomes, prioritizes the backlog, and measures success
- **Developers**: Implement features, collaborate on design, and ensure testability
- **QA/Testing**: Validate quality standards and acceptance criteria

## Project Lifecycle

Our projects follow a structured lifecycle that ensures alignment, quality, and continuous learning:

1. **Initiation**: Validate business need, identify stakeholders, create a project one-pager with problem statement, goals, success metrics, and initial risk assessment. ([Details](./octoacme-project-initiation.md))

2. **Planning**: Break work into shippable increments, define the prioritized backlog with acceptance criteria, estimate scope, identify dependencies, and create a release plan. ([Details](./octoacme-project-planning.md))

3. **Execution**: Build and test features iteratively using daily standups, weekly syncs, PR workflows, and continuous integration while tracking progress on project boards. ([Details](./octoacme-execution-and-tracking.md))

4. **Release**: Deploy to production following pre-release requirements, run smoke tests, execute deployment checklist, and announce to stakeholders with release notes. ([Details](./octoacme-release-and-deployment.md))

5. **Close & Retrospective**: Capture learnings through retrospectives, document what went well and what could improve, and create actionable improvement items with clear owners. ([Details](./octoacme-retrospective-and-continuous-improvement.md))

## Key Workflows & Artifacts

Our standardized workflows and artifacts ensure consistency and quality across all projects:

- **Project Charter / One-pager**: Problem statement, goals, success metrics, stakeholders, and timeline ([Template](./octoacme-project-initiation.md#project-one-pager-template))
- **Prioritized Backlog**: User stories with acceptance criteria, estimates, and priorities ([Details](./octoacme-project-planning.md#backlog-item-template))
- **Definition of Done**: Clear criteria for considering work complete ([Planning guide](./octoacme-project-planning.md))
- **Pull Request Workflow**: Small PRs with issue links, automated tests, linting, and required approvals ([Execution guide](./octoacme-execution-and-tracking.md#workflows))
- **Risk Register**: Track risks with impact, likelihood, owner, and mitigation plans ([Risk management](./octoacme-risks-and-communication.md#risk-register))
- **Release Checklist**: Pre-deployment requirements, smoke tests, and post-deploy verifications ([Release guide](./octoacme-release-and-deployment.md#deployment-checklist))
- **Retrospective Notes**: Action items with owners and due dates for continuous improvement ([Retrospective guide](./octoacme-retrospective-and-continuous-improvement.md))

For more details on roles and responsibilities, see [OctoAcme Roles and Personas](./octoacme-roles-and-personas.md). For communication strategies and stakeholder updates, refer to [Risk Management & Communication](./octoacme-risks-and-communication.md).

## Execution Checklist

Use this checklist during the execution phase to ensure all critical activities are complete:

- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly

For the complete execution framework including team rhythm, quality standards, and escalation procedures, see the [Execution & Tracking guide](./octoacme-execution-and-tracking.md).

## How to Request Changes to These Process Docs

If you have suggestions for improving these process documents or need to add new guidance, please open an issue using our standard template:

1. Navigate to the [Issues page](../../issues)
2. Click "New Issue"
3. Select the **"Add Content to Project Management Process Docs"** template
4. Fill out the template with your proposed changes and rationale

You can also access the issue template directly at `.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml` in this repository.

---

**Need more details?** Each section above links to comprehensive guides covering specific phases and practices. Start with the [Project Management Overview](./octoacme-project-management-overview.md) for a complete introduction to our approach.
