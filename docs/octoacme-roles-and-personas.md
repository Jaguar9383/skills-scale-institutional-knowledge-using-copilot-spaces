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

## Scrum Master

### Role Summary
Scrum Masters facilitate Agile processes, remove blockers, and ensure the team follows agreed-upon practices. They coach the team on self-organization and continuous improvement while protecting them from distractions.

### Responsibilities
- Facilitate daily standups, sprint planning, and retrospectives
- Remove impediments and blockers that prevent team progress
- Coach the team on Agile practices and self-organization
- Shield the team from external interruptions and scope creep
- Track team velocity and help improve predictability
- Foster collaboration and psychological safety

### Goals
- Maximize team productivity and flow
- Improve sprint-over-sprint predictability
- Build a culture of continuous improvement and learning
- Ensure transparency in team processes and progress

### Typical Communication
- Daily standups and sprint ceremonies
- One-on-one coaching sessions with team members
- Sprint reports and velocity tracking
- Escalation of blockers to Project Managers or leadership

### Collaboration with Other Roles
- **With Project Managers**: Coordinate on timeline alignment, risk escalation, and cross-team dependencies
- **With Developers**: Remove blockers, facilitate estimation, and support technical decision-making
- **With Product Managers**: Ensure backlog readiness and clarify acceptance criteria
- **With UX Designers**: Facilitate design reviews and coordinate design handoffs during sprint planning
- **With Technical Writers**: Ensure documentation tasks are included in sprint scope and definition of done

---

## UX Designer

### Role Summary
UX Designers research user needs, create intuitive user experiences, and ensure designs meet accessibility and usability standards. They collaborate with Product Managers and Developers to deliver user-centered solutions.

### Responsibilities
- Conduct user research and usability testing
- Create wireframes, prototypes, and high-fidelity designs
- Ensure designs meet accessibility standards (WCAG, ARIA)
- Collaborate with developers during implementation
- Validate implemented features against design specifications
- Maintain and evolve design systems and component libraries

### Goals
- Create intuitive, accessible user experiences
- Reduce user friction and improve task completion rates
- Ensure brand consistency across all touchpoints
- Validate designs with real user feedback

### Typical Communication
- Design reviews and critique sessions
- User research findings and insights presentations
- Handoff documentation with specs and assets
- Iteration feedback during sprint reviews

### Collaboration with Other Roles
- **With Product Managers**: Translate product requirements into user flows and design solutions
- **With Developers**: Provide design specs, assets, and implementation guidance; validate final implementation
- **With Project Managers**: Estimate design work and coordinate design review milestones
- **With Scrum Master**: Participate in sprint planning to ensure design work is properly scoped
- **With Security Lead**: Ensure designs don't expose sensitive data or create security vulnerabilities

---

## Technical Writer

### Role Summary
Technical Writers create clear, accurate documentation for users, developers, and stakeholders. They ensure documentation is maintained, accessible, and aligned with product releases.

### Responsibilities
- Write and maintain user guides, API documentation, and release notes
- Collaborate with developers to document features and technical specifications
- Ensure documentation follows style guides and standards
- Create tutorials, how-to guides, and troubleshooting content
- Review and update documentation for accuracy with each release
- Manage documentation repositories and publishing workflows

### Goals
- Enable users to successfully adopt and use product features
- Reduce support burden through comprehensive self-service documentation
- Maintain accurate, up-to-date technical content
- Ensure documentation accessibility and searchability

### Typical Communication
- Documentation reviews with subject matter experts
- Release notes and changelog updates
- Style guide updates and documentation standards
- Feedback loops with support and customer success teams

### Collaboration with Other Roles
- **With Developers**: Gather technical details, review code comments, and validate technical accuracy
- **With Product Managers**: Understand feature intent and target audience for documentation
- **With Release Manager**: Coordinate documentation updates with release schedules
- **With UX Designers**: Ensure UI/UX documentation matches actual implementation
- **With Project Managers**: Track documentation tasks and report on completion status

---

## Release Manager

### Role Summary
Release Managers coordinate and oversee the release process from planning through deployment. They ensure releases are well-tested, properly documented, and deployed with minimal risk.

### Responsibilities
- Plan and coordinate release schedules across teams
- Manage release branches and version control strategy
- Oversee release testing, including smoke tests and validation
- Coordinate with stakeholders on release timing and communication
- Manage rollback procedures and incident response during releases
- Maintain release checklists and deployment runbooks

### Goals
- Deliver releases on schedule with high quality
- Minimize production incidents and deployment failures
- Ensure smooth coordination across engineering, QA, and operations
- Maintain clear release documentation and audit trails

### Typical Communication
- Release planning meetings and go/no-go decisions
- Release status updates to stakeholders
- Post-deployment reports and metrics
- Incident communications during rollbacks

### Collaboration with Other Roles
- **With Developers**: Coordinate code freeze, feature completion, and hotfix prioritization
- **With Project Managers**: Align release schedules with project timelines and milestones
- **With Technical Writers**: Ensure release notes and documentation are ready before deployment
- **With Security Lead**: Verify security scans pass and vulnerabilities are addressed
- **With QA/Testing**: Coordinate test execution and sign-off before release

---

## Security Lead

### Role Summary
Security Leads ensure security best practices are followed throughout the development lifecycle. They conduct security reviews, manage vulnerability assessments, and guide teams on secure coding practices.

### Responsibilities
- Conduct security reviews and threat modeling for new features
- Manage security scanning tools and vulnerability remediation
- Define and enforce secure coding standards and guidelines
- Respond to security incidents and coordinate remediation
- Perform security-focused code reviews on critical changes
- Educate teams on security best practices and emerging threats

### Goals
- Minimize security vulnerabilities in production systems
- Ensure compliance with security standards and regulations
- Build security awareness across engineering teams
- Respond rapidly to security incidents with minimal impact

### Typical Communication
- Security review findings and recommendations
- Vulnerability reports and remediation timelines
- Security incident post-mortems
- Security training and awareness sessions

### Collaboration with Other Roles
- **With Developers**: Provide secure coding guidance and review security-sensitive code
- **With Release Manager**: Verify security scans pass before releases and approve deployments
- **With Project Managers**: Estimate security work and communicate security risks
- **With UX Designers**: Review designs for security implications (e.g., data exposure, authentication flows)
- **With Product Managers**: Balance security requirements with product timelines and feature priorities

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

