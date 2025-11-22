# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

## Reporting & Metrics

### Key Metrics to Track

**Delivery Metrics:**
- **Velocity**: Story points or tasks completed per sprint
- **Burndown**: Work remaining vs. time in sprint
- **Cycle Time**: Time from work started to deployed
- **Lead Time**: Time from request to deployment
- **Deployment Frequency**: How often code is deployed to production

**Quality Metrics:**
- **Change Failure Rate**: % of deployments causing issues
- **Mean Time to Recovery (MTTR)**: Time to restore service after incident
- **Code Review Time**: Time from PR opened to merged
- **Test Coverage**: % of code covered by automated tests
- **Bug Escape Rate**: Bugs found in production vs. caught in testing

**Business Metrics:**
- Monitor success metrics identified in the Project Charter
- User engagement and adoption rates
- Performance SLAs (uptime, latency, throughput)
- Customer satisfaction scores (NPS, CSAT)

### Dashboard Recommendations
- Use dashboards for key signals: errors, latency, usage, deployment status
- Set up alerts for threshold breaches (error rate >5%, latency >500ms, etc.)
- Make dashboards accessible to entire team for transparency
- Review metrics weekly in team syncs and monthly with stakeholders

## Blocker Escalation

### Escalation Levels & Timeframes

**Level 1: Team-Level Triage**
- **When**: Blockers identified in daily standup
- **Timeframe**: Resolve within 24 hours
- **Owner**: Team members collaborate to resolve
- **Action**: Pair programming, quick technical discussions, reassignment of tasks

**Level 2: PM/Lead Escalation**
- **When**: Blocker not resolved after 24 hours, or cross-team dependency identified
- **Timeframe**: Escalate within 1 business day, resolve within 48 hours
- **Owner**: PM escalates to Product Lead and dependent teams
- **Action**: Schedule sync meetings, negotiate priorities, adjust sprint scope

**Level 3: Sponsor/Executive Escalation**
- **When**: Business-impacting issues, budget/resource constraints, critical timeline risks
- **Timeframe**: Escalate immediately, resolution plan within 24 hours
- **Owner**: PM or Product Lead escalates to Executive Sponsor
- **Action**: Executive decision-making, resource reallocation, timeline adjustments

### Escalation Best Practices
- Document blockers clearly with impact assessment
- Include proposed solutions or alternatives when escalating
- Communicate escalation status to all stakeholders
- Track resolution in project tracking tool and risk register

## Execution Checklist
- [ ] Branching and PR conventions documented in repo
- [ ] CI configured for tests and lint
- [ ] Regular demos scheduled
- [ ] Risk register updated weekly
