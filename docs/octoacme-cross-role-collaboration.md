# OctoAcme — Cross-Role Collaboration Guide

## Purpose
Define clear handoffs, responsibilities, and collaboration patterns between roles to ensure smooth project delivery and minimize gaps or bottlenecks.

## Principles
- **Clear handoffs**: Every deliverable has a defined owner and recipient
- **Shared accountability**: Teams collaborate to ensure quality across all touchpoints
- **Transparent communication**: Handoffs include clear acceptance criteria and timelines
- **Continuous feedback**: Regular checkpoints to identify and resolve collaboration issues

---

## Release Management Handoffs

### Pre-Release Handoff (Development → Release Manager)
**When**: At code freeze or feature-complete milestone

**Developer Responsibilities**:
- [ ] All acceptance criteria met and PRs merged to release branch
- [ ] CI/CD pipeline passing (tests, linting, security scans)
- [ ] Known issues documented with severity and workarounds
- [ ] Database migrations tested and documented (if applicable)
- [ ] Feature flags configured correctly for staged rollout

**Release Manager Acceptance**:
- [ ] Verify all required PRs merged and tagged
- [ ] Confirm CI/CD green status
- [ ] Review release notes for completeness
- [ ] Validate smoke test plan covers critical paths

### Documentation Handoff (Technical Writer → Release Manager)
**When**: 2 days before scheduled release

**Technical Writer Responsibilities**:
- [ ] Release notes drafted and reviewed
- [ ] User-facing documentation updated
- [ ] API documentation reflects new endpoints or changes
- [ ] Migration guides prepared (if breaking changes)
- [ ] Known issues and workarounds documented

**Release Manager Acceptance**:
- [ ] Release notes approved by Product Manager
- [ ] Documentation links validated and accessible
- [ ] Support team notified and briefed on changes

### Security Handoff (Security Lead → Release Manager)
**When**: Before deployment to production

**Security Lead Responsibilities**:
- [ ] Security scans completed (SAST, dependency scanning)
- [ ] Vulnerabilities assessed and critical issues resolved
- [ ] Security review completed for high-risk features
- [ ] Compliance requirements validated
- [ ] Incident response plan reviewed if needed

**Release Manager Acceptance**:
- [ ] No critical or high-severity vulnerabilities unresolved
- [ ] Security sign-off documented
- [ ] Any accepted risks logged with justification

### Post-Release Handoff (Release Manager → Product/Project Manager)
**When**: After successful deployment

**Release Manager Responsibilities**:
- [ ] Deployment verification completed
- [ ] Smoke tests passed
- [ ] Monitoring and alerts configured
- [ ] Rollback plan tested and ready
- [ ] Stakeholders notified of successful release

**Product/Project Manager Acceptance**:
- [ ] Success metrics being tracked
- [ ] Support team briefed on new features
- [ ] Customer communications sent
- [ ] Post-release retrospective scheduled

---

## UX Review Handoffs

### Design Handoff (UX Designer → Developers)
**When**: Before sprint/iteration begins

**UX Designer Responsibilities**:
- [ ] Wireframes or high-fidelity designs completed
- [ ] Design specs documented (spacing, colors, fonts, interactions)
- [ ] Assets exported and accessible (icons, images, etc.)
- [ ] Accessibility requirements specified (ARIA labels, keyboard navigation)
- [ ] Edge cases and responsive behavior defined
- [ ] Interactive prototype available for complex flows

**Developer Acceptance**:
- [ ] Design files accessible and reviewed
- [ ] Clarifying questions addressed
- [ ] Technical feasibility confirmed
- [ ] Design included in sprint scope with estimates

### Implementation Review (Developer → UX Designer)
**When**: During PR review or before feature completion

**Developer Responsibilities**:
- [ ] Implementation matches design specifications
- [ ] Responsive behavior implemented across breakpoints
- [ ] Accessibility attributes added per design requirements
- [ ] Interactive states implemented (hover, focus, disabled, etc.)
- [ ] Staging/preview link provided for UX review

**UX Designer Acceptance**:
- [ ] Visual implementation matches design
- [ ] Interactions and animations work as intended
- [ ] Accessibility requirements met
- [ ] Edge cases handled appropriately
- [ ] Sign-off provided or change requests logged

### User Research Handoff (UX Designer → Product Manager)
**When**: After research synthesis

**UX Designer Responsibilities**:
- [ ] Research findings synthesized and documented
- [ ] User pain points and opportunities identified
- [ ] Recommendations prioritized by impact
- [ ] Supporting data and quotes included
- [ ] Presentation or report prepared

**Product Manager Acceptance**:
- [ ] Findings incorporated into product backlog
- [ ] Priorities adjusted based on user insights
- [ ] Follow-up research needs identified

---

## Documentation Responsibilities

### Feature Documentation (Developer → Technical Writer)
**When**: Feature development complete, before code freeze

**Developer Responsibilities**:
- [ ] Feature overview and intended use cases provided
- [ ] API changes documented (endpoints, parameters, responses)
- [ ] Code examples or sample requests provided
- [ ] Configuration options and defaults listed
- [ ] Known limitations or caveats identified

**Technical Writer Acceptance**:
- [ ] Sufficient detail to write user-facing documentation
- [ ] Technical accuracy validated
- [ ] Questions addressed
- [ ] Draft documentation reviewed by developer

### Documentation Review (Technical Writer → Product Manager)
**When**: Before release or major documentation update

**Technical Writer Responsibilities**:
- [ ] Documentation written and formatted
- [ ] Content reviewed for accuracy and clarity
- [ ] Cross-references and links validated
- [ ] Screenshots updated (if applicable)
- [ ] SEO and discoverability optimized

**Product Manager Acceptance**:
- [ ] Content aligns with product messaging
- [ ] Target audience needs addressed
- [ ] Release timing coordinated

### Code Documentation (Developer → Developer)
**When**: Ongoing during development

**Developer Responsibilities**:
- [ ] Code comments explain "why" not "what"
- [ ] Complex logic documented inline
- [ ] README updated with setup instructions
- [ ] Architecture decisions documented (ADRs)
- [ ] API contracts documented (OpenAPI, etc.)

**Team Acceptance**:
- [ ] Code review includes documentation check
- [ ] Documentation sufficient for future maintainers
- [ ] Onboarding friction reduced

---

## Security Review Handoffs

### Feature Security Review (Developer → Security Lead)
**When**: Design phase or before implementation of security-sensitive features

**Developer Responsibilities**:
- [ ] Feature description and data flows provided
- [ ] Authentication/authorization approach documented
- [ ] Data sensitivity classified (PII, credentials, etc.)
- [ ] Threat model completed for high-risk features
- [ ] Security questions identified early

**Security Lead Acceptance**:
- [ ] Review completed and feedback provided
- [ ] Security requirements defined (encryption, access controls, etc.)
- [ ] Implementation guidance provided
- [ ] Follow-up review scheduled if needed

### Code Security Review (Developer → Security Lead)
**When**: PR ready for review (for security-sensitive changes)

**Developer Responsibilities**:
- [ ] Security-focused code changes clearly marked
- [ ] Input validation and sanitization implemented
- [ ] Secrets management handled properly (no hardcoded credentials)
- [ ] Dependency updates reviewed for known vulnerabilities
- [ ] Security test cases added

**Security Lead Acceptance**:
- [ ] Code review completed with security lens
- [ ] Vulnerabilities identified and remediated
- [ ] Secure coding standards followed
- [ ] Approval provided or issues logged

### Vulnerability Remediation (Security Lead → Developer)
**When**: After security scan or vulnerability disclosure

**Security Lead Responsibilities**:
- [ ] Vulnerability details and severity provided
- [ ] Remediation guidance or recommendations included
- [ ] Timeline for fix established based on severity
- [ ] Workarounds identified if immediate fix not possible

**Developer Acceptance**:
- [ ] Vulnerability understood and reproducible
- [ ] Remediation plan agreed upon
- [ ] Fix implemented and verified by Security Lead
- [ ] Regression tests added to prevent reintroduction

### Security Sign-off (Security Lead → Release Manager)
**When**: Before production deployment

**Security Lead Responsibilities**:
- [ ] All critical and high-severity issues resolved
- [ ] Security scans completed and passing
- [ ] Compliance requirements validated
- [ ] Risk assessment documented for any accepted issues
- [ ] Incident response plan reviewed if needed

**Release Manager Acceptance**:
- [ ] Security clearance documented
- [ ] Any residual risks communicated to stakeholders
- [ ] Release approved from security perspective

---

## Cross-Role Collaboration Best Practices

### Communication Channels
- **Synchronous**: Daily standups, sprint planning, design reviews, release meetings
- **Asynchronous**: PR comments, documentation updates, project board updates, Slack/Teams channels
- **Escalation**: Use defined escalation paths when handoffs are blocked or unclear

### Handoff Templates
Each handoff should include:
- **What**: Deliverable or artifact being handed off
- **When**: Expected timing and deadline
- **Who**: Owner and recipient clearly defined
- **Acceptance Criteria**: Clear checklist of what "done" means
- **Format**: Where the artifact lives (GitHub, Figma, Confluence, etc.)

### Collaboration Tools
- **GitHub Projects**: Track cross-team dependencies and handoffs
- **Pull Requests**: Central hub for code review and approval workflows
- **Documentation Repos**: Single source of truth for process docs and runbooks
- **Design Tools** (Figma, Sketch): Shared design libraries and handoff specs
- **Communication Platforms**: Slack, Teams for real-time coordination

### Avoiding Collaboration Pitfalls
- **Unclear ownership**: Always designate a DRI (Directly Responsible Individual) for each handoff
- **Missing context**: Include links to related issues, designs, or documentation
- **Bottlenecks**: Identify dependencies early and schedule handoffs in advance
- **Silent failures**: Proactively communicate when handoffs can't be completed on time

---

## Collaboration Checklist for Project Kick-off

Use this checklist at project initiation to ensure all collaboration touchpoints are defined:

- [ ] All required roles identified and assigned
- [ ] Handoff schedule created and communicated
- [ ] Communication channels established (Slack, GitHub, etc.)
- [ ] Shared artifacts locations defined (GitHub, Figma, Drive, etc.)
- [ ] Review and approval workflows documented
- [ ] Escalation paths defined for blockers
- [ ] Collaboration expectations added to Definition of Done
- [ ] Regular sync meetings scheduled across roles

---

## Related Documentation
- [OctoAcme Roles and Personas](./octoacme-roles-and-personas.md) — detailed role definitions
- [Execution & Tracking](./octoacme-execution-and-tracking.md) — workflows and quality standards
- [Release & Deployment](./octoacme-release-and-deployment.md) — release process details
- [Risk Management & Communication](./octoacme-risks-and-communication.md) — escalation and status updates
