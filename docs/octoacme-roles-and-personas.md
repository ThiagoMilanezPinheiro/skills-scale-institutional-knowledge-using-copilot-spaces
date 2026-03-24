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
The Scrum Master facilitates Agile ceremonies, removes impediments, and coaches the team and stakeholders on Agile best practices. They act as a servant leader, protecting the team's focus and enabling continuous improvement.

### Responsibilities
- Guide the team in Scrum adoption and continuous improvement
- Facilitate standups, sprint planning, sprint reviews, and retrospectives
- Remove blockers and help resolve team impediments
- Protect the team from unplanned interruptions and scope creep
- Ensure Scrum artifacts (backlog, sprint board, Definition of Done) are visible and kept up-to-date
- Coach Project Managers and Product Managers on Agile principles

### Goals
- Maximize team velocity and delivery predictability
- Foster a culture of transparency, inspection, and adaptation
- Reduce cycle time and minimize process waste

### Typical Communication
- Daily standups and sprint ceremonies
- Impediment logs and escalation to Project Manager when needed
- Retrospective action items and improvement tracking

### Interactions with Existing Roles
- **Developers**: Facilitates all sprint ceremonies, removes technical and organizational blockers, and supports the team in meeting the Definition of Done.
- **Product Managers (PdM)**: Collaborates on backlog refinement sessions to ensure stories have clear acceptance criteria before sprint planning; helps PdM understand team capacity and velocity for roadmap forecasting.
- **Project Managers (PM)**: Partners on cross-team dependencies and milestone tracking; escalates blockers that cannot be resolved at the team level; participates in weekly PM syncs and shares sprint progress against the project plan. Handoffs happen when delivery risks are identified in the sprint that may affect the broader project timeline.

---

## UX Designer

### Role Summary
UX Designers advocate for user-centric design, conduct user research, prototype solutions, and ensure interfaces meet usability principles. They bridge the gap between user needs and technical implementation.

### Responsibilities
- Conduct user interviews, usability tests, and competitive analysis
- Create wireframes, prototypes, and user flow diagrams
- Define and maintain design system standards and accessibility guidelines
- Document design decisions and rationale in design specs
- Validate designs against acceptance criteria and user feedback

### Goals
- Ensure products are intuitive, accessible, and aligned with user needs
- Reduce rework by surfacing usability issues before development begins
- Improve feature adoption and customer satisfaction through informed design

### Typical Communication
- Design reviews and critique sessions with Developers and Product Managers
- Usability test reports and research summaries
- Annotated mockups and design specs shared via design tooling (e.g., Figma)

### Interactions with Existing Roles
- **Developers**: Collaborates during sprint planning and execution to align on implementation feasibility; provides annotated specs and is available for design Q&A during development. Handoffs occur when a story moves from backlog refinement to active development—the UX Designer ensures the spec is complete and acceptance criteria include UX acceptance before the story is pulled.
- **Product Managers (PdM)**: Works closely with PdM during the discovery phase to translate user research into problem statements and acceptance criteria; participates in backlog prioritization to ensure UX work is sequenced ahead of development. Collaborates on the Project Charter's user impact sections.
- **Project Managers (PM)**: Provides visibility into design milestone progress; flags timeline risks when user research reveals scope changes; participates in planning meetings to estimate design effort in alignment with the overall project timeline and Risk Register.

---

## Data Analyst

### Role Summary
Data Analysts ensure that product and project decisions are data-informed by generating actionable insights and reporting on key metrics. They connect raw data to business outcomes and support evidence-based iteration.

### Responsibilities
- Define and track success metrics aligned to project goals and OKRs
- Build dashboards and visualizations to monitor product health and delivery KPIs
- Conduct ad-hoc analysis to answer specific product or project questions
- Identify data instrumentation needs and coordinate with Developers to implement tracking
- Provide analysis to inform sprint retrospectives, release reviews, and planning sessions
- Validate hypotheses and A/B test results for Product Managers

### Goals
- Enable data-driven prioritization and decision-making across all roles
- Reduce time to insight for product and project questions
- Maintain data quality and a shared understanding of key metrics

### Typical Communication
- Weekly metrics digests shared with Product Managers and Project Managers
- Dashboard links and annotations in sprint review notes
- Ad-hoc analysis reports delivered as GitHub issues or shared documents

### Interactions with Existing Roles
- **Developers**: Partners with Developers to identify and implement data instrumentation (event tracking, logging) needed to measure feature success; reviews instrumentation in code reviews to ensure accuracy. Handoffs happen when a feature is ready for release—the Data Analyst confirms tracking is in place before the release checklist is signed off.
- **Product Managers (PdM)**: Collaborates during planning to define measurable success criteria for features; delivers post-release analysis to validate whether acceptance criteria translated to real-world impact; supports PdM in backlog prioritization with usage data and funnel analysis.
- **Project Managers (PM)**: Provides delivery KPI reports (velocity, defect rates, on-time completion) to support status updates and stakeholder briefings; contributes data-driven risk assessments to the Risk Register; participates in retrospectives to surface quantitative evidence for improvement opportunities.

---

## Interaction Map — Quick Reference

The table below shows primary ownership (O), active contribution (C), and informed/consulted (I) for each lifecycle phase across all roles.

| Phase | Developers | Product Manager (PdM) | Project Manager (PM) | Scrum Master | UX Designer | Data Analyst |
|---|---|---|---|---|---|---|
| **Initiation** | I | O | C | I | C | C |
| **Planning** | C | O | O | C | C | C |
| **Execution** | O | C | C | O | C | C |
| **Release** | O | C | O | C | I | C |
| **Retrospective** | C | C | O | O | I | C |

**Key artifacts by phase:**
- **Initiation**: Project Charter / One-pager — owned by PM/PdM; UX Designer contributes user impact statement; Data Analyst contributes baseline metrics.
- **Planning**: Backlog & acceptance criteria — owned by PdM; Scrum Master facilitates kickoff; UX Designer provides wireframes/specs; PM maintains Risk Register and timeline.
- **Execution**: Sprint board & Definition of Done (DoD) — facilitated by Scrum Master; Developers implement; UX Designer reviews implementation; Data Analyst confirms instrumentation.
- **Release**: Release plan & deployment checklist — coordinated by PM; Developers deploy; Data Analyst verifies tracking is live.
- **Retrospective**: Retrospective notes & action items — facilitated by Scrum Master; PM tracks follow-through; Data Analyst provides quantitative summary of the sprint/release.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

