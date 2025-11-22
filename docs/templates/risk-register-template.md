# Risk Register: [Project Name]

**Project:** [Project Name]  
**Last Updated:** [Date]  
**Owner:** [Project Manager Name]

---

## How to Use This Risk Register

1. **Identify risks** during planning and throughout execution
2. **Assess** each risk's impact and likelihood
3. **Assign** an owner responsible for monitoring and mitigation
4. **Define** mitigation strategies and contingency plans
5. **Review** and update weekly during project syncs
6. **Close** risks when they are resolved or no longer applicable

### Risk Severity Guide

**Impact Levels:**
- **High**: Could cause project failure, major delays, or significant cost overruns
- **Medium**: Could cause moderate delays or require replanning
- **Low**: Minor inconvenience, easily addressed

**Likelihood Levels:**
- **High**: Very likely to occur (>60% probability)
- **Medium**: Might occur (30-60% probability)
- **Low**: Unlikely to occur (<30% probability)

**Priority Calculation:** Impact × Likelihood = Risk Priority
- High Impact + High Likelihood = **CRITICAL** (immediate action required)
- High Impact + Medium Likelihood or Medium Impact + High Likelihood = **HIGH** (proactive mitigation needed)
- All others = **MEDIUM** or **LOW** (monitor regularly)

---

## Active Risks

| ID | Description | Impact | Likelihood | Priority | Owner | Mitigation Strategy | Status | Last Updated |
|----|-------------|--------|------------|----------|-------|-------------------|--------|--------------|
| R-001 | [Example: Dependency on Team X's API completion] | High | High | CRITICAL | [PM Name] | [Early engagement with Team X, parallel mockup development] | Active | [Date] |
| R-002 | [Example: Key developer may be unavailable in Sprint 3] | Medium | Medium | HIGH | [PM Name] | [Cross-training in Sprint 1-2, backup resource identified] | Active | [Date] |
| R-003 | [Example: Third-party library has known security vulnerabilities] | High | Low | MEDIUM | [Tech Lead] | [Evaluate alternatives, monitor vendor patches] | Active | [Date] |
| R-004 | | | | | | | | |
| R-005 | | | | | | | | |

---

## Closed/Resolved Risks

| ID | Description | Impact | Likelihood | Resolution | Date Closed |
|----|-------------|--------|------------|------------|-------------|
| R-XXX | [Example: Uncertainty about cloud budget approval] | Medium | High | [Budget approved by Finance on MM/DD] | [Date] |

---

## Risk Categories (for reference)

Use these categories to help identify risks:

- **Technical**: Architecture complexity, technology constraints, integration challenges
- **Resource**: Team availability, skill gaps, dependencies on other teams
- **Schedule**: Tight deadlines, external dependencies, scope creep
- **External**: Vendor delays, regulatory changes, market shifts
- **Quality**: Testing coverage, performance requirements, accessibility compliance
- **Security**: Data privacy, authentication, vulnerability management
- **Organizational**: Stakeholder alignment, priority shifts, budget constraints

---

## Escalation Process

- **Low/Medium Priority Risks**: Managed by PM, reviewed weekly in team syncs
- **High Priority Risks**: Escalated to Product Lead and Sponsor, reviewed twice weekly
- **Critical Risks**: Immediate escalation to Sponsor, daily monitoring, mitigation plan required within 24 hours

---

## Notes & Best Practices

- Review this register at every weekly sync and update status
- Don't wait for risks to become issues—proactive mitigation is key
- Archive resolved risks for retrospective learnings
- Use this template in conjunction with the [Risk Management & Communication](../octoacme-risks-and-communication.md) process doc
- Keep mitigation strategies actionable and assign clear owners
- Document assumptions alongside risks (e.g., "Assuming vendor delivers on time")

---

## Template Instructions

1. Copy this template to your project repository
2. Rename to `risk-register-[project-name].md`
3. Fill in the project details at the top
4. Add identified risks to the Active Risks table
5. Update weekly and move resolved risks to the Closed section
6. Reference this register in weekly status updates
