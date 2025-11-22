# Release Readiness Checklist

Use this checklist to ensure your release is production-ready and minimize deployment risks.

---

## Pre-Release Preparation (1-2 Weeks Before)

### Product & Planning

- [ ] All acceptance criteria met for release scope
- [ ] Product Manager sign-off on features and functionality
- [ ] Release notes drafted (see template below)
- [ ] User documentation updated (if applicable)
- [ ] Support team briefed on new features and changes
- [ ] Marketing/communications plan in place (if needed)

### Development

- [ ] All feature PRs merged to main/release branch
- [ ] Code freeze initiated (if applicable)
- [ ] Feature flags configured for gradual rollout (if applicable)
- [ ] Database migration scripts reviewed and tested
- [ ] Configuration changes documented
- [ ] Dependencies updated and security-scanned

### Quality Assurance

- [ ] All planned test cases executed and passed
- [ ] Regression testing complete
- [ ] Performance testing complete (load, stress tests)
- [ ] Accessibility testing complete (if applicable)
- [ ] Security scanning passed (SAST, DAST, dependency scans)
- [ ] Known issues documented with workarounds
- [ ] Test environment mirrors production environment

### Infrastructure & DevOps

- [ ] CI/CD pipeline green for release candidate
- [ ] Deployment scripts tested and validated
- [ ] Rollback plan documented and tested
- [ ] Monitoring and alerting configured for new features
- [ ] Capacity planning reviewed (expected load, scaling)
- [ ] Backup and disaster recovery plan verified

---

## Release Day Preparation (1-3 Days Before)

### Communication

- [ ] Release window scheduled and communicated to stakeholders
- [ ] On-call rotation confirmed for release window
- [ ] Incident response team identified and on standby
- [ ] Stakeholders notified of deployment timeline
- [ ] Customer-facing teams alerted (support, sales, etc.)

### Final Verification

- [ ] Staging deployment successful with smoke tests passed
- [ ] Production deployment runbook reviewed
- [ ] Rollback criteria defined and agreed upon
- [ ] Post-deployment verification plan documented
- [ ] Deployment checklist printed/accessible (this document!)

### Environment Readiness

- [ ] Production environment health check passed
- [ ] Database backup completed and verified
- [ ] Monitoring dashboards prepared for release tracking
- [ ] Log aggregation and alerting confirmed operational

---

## Deployment Day Checklist

### Pre-Deployment (T-minus 30 minutes)

- [ ] Final go/no-go decision with PM, Tech Lead, and on-call
- [ ] All team members on standby and available
- [ ] Communication channels open (Slack, Teams, etc.)
- [ ] Deployment window start announced to stakeholders
- [ ] Maintenance page deployed (if applicable)

### During Deployment

- [ ] Deployment initiated via automated pipeline (preferred) or manual process
- [ ] Deployment progress monitored in real-time
- [ ] Key metrics monitored (error rates, latency, throughput)
- [ ] Smoke tests executed as components deploy
- [ ] Database migrations applied successfully
- [ ] Configuration changes applied and verified

### Immediate Post-Deployment (First 30 Minutes)

- [ ] Application health checks passed
- [ ] Critical user flows tested manually (smoke tests)
- [ ] Monitoring dashboards show normal metrics
- [ ] Error rates within expected thresholds
- [ ] No critical alerts triggered
- [ ] Feature flags enabled (if gradual rollout)
- [ ] Maintenance page removed (if applicable)

---

## Post-Deployment Verification (First 24-48 Hours)

### Monitoring & Validation

- [ ] User traffic patterns normal
- [ ] Application performance metrics within SLAs
- [ ] No spike in error rates or exceptions
- [ ] Database performance and queries optimized
- [ ] No unexpected user reports or support tickets
- [ ] Key business metrics tracked (conversions, engagement, etc.)

### Communication & Documentation

- [ ] Deployment success announced to stakeholders
- [ ] Release notes published and shared
- [ ] Support team updated with any known issues
- [ ] Post-deployment summary documented
- [ ] Lessons learned captured for retrospective

---

## Rollback Decision Criteria

**Consider rollback if:**

- [ ] Critical functionality is broken or unavailable
- [ ] Error rates exceed 5% (or agreed threshold)
- [ ] Performance degradation >50% from baseline
- [ ] Data integrity issues detected
- [ ] Security vulnerability introduced
- [ ] Rollback can be completed within acceptable downtime window

**Rollback Process:**

1. Announce rollback decision to stakeholders
2. Execute rollback runbook
3. Verify system returns to stable state
4. Communicate status and next steps
5. Schedule post-mortem to identify root cause

---

## Release Notes Template

```markdown
## Release: [Version/Name] - [Date]

### Summary
[Brief overview of the release purpose and key changes]

### New Features
- [Feature 1]: [Description]
- [Feature 2]: [Description]

### Improvements
- [Improvement 1]
- [Improvement 2]

### Bug Fixes
- [Fix 1]
- [Fix 2]

### Known Issues
- [Issue 1]: [Workaround]

### Breaking Changes (if any)
- [Change 1]: [Migration steps]

### Deployment Notes
- [Any special deployment considerations]
- [Configuration changes required]
```

---

## Related Process Documents

- [Release & Deployment Guide](../octoacme-release-and-deployment.md)
- [Execution & Tracking](../octoacme-execution-and-tracking.md)
- [Risk Management & Communication](../octoacme-risks-and-communication.md)

---

**Last Updated:** [Date]  
**Owner:** [Project Manager / Release Manager]
