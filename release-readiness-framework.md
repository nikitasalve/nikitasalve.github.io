---
layout: default
title: Go/No-Go Decision Gatekeeping Matrix
---

# CI/CD Release Promotion & Go/No-Go Gatekeeping Matrix
**Author:** Nikita Salve | Lead Release & Technical Program Manager

---

## 🎯 Purpose & Scope
This framework defines the automated and manual quality, security, and operational criteria required for a release candidate to transition from **UAT/Staging to Production** in enterprise delivery environments.

---

## 🚦 Gatekeeping Decision Criteria

| Evaluation Dimension | Threshold for "GO" | "NO-GO" Blocker Condition | Evidence Required |
| :--- | :--- | :--- | :--- |
| **Functional QA** | 100% test case execution; >98% pass rate | Any open P1 or P2 blocker defect | Jira / TestRail execution report |
| **Regression Suite** | 100% automated regression passing | Any unanalyzed flaky/failed critical test | Azure DevOps Pipeline summary |
| **Security & Compliance** | Zero critical/high CVEs; ISO 27001 scan clear | Critical vulnerability with no remediation waiver | SonarQube / SAST / DAST logs |
| **Performance Testing** | Response time within SLA ($<200\text{ms}$ at peak load) | Latency degradation $>15\%$ vs baseline | JMeter / Locust report |
| **Operational Readiness** | Deployment runbook approved; Rollback tested | Missing rollback plan or missing DBA backup | Cutover Runbook & CAB Record |
| **Stakeholder Sign-offs** | Product Owner, QA Lead, Engineering Lead, Ops | Any single functional lead objection | Formal sign-off thread / Jira ticket |

---

## 📋 Go/No-Go Meeting Agenda (30-Minute Format)

1. **Pipeline & Build Verification (05 mins):** Confirm build version, artifact hash, and change delta.
2. **Defect & Risk Review (10 mins):** Review any P3/P4 known issues; verify zero P1/P2 defects.
3. **Rollback & Cutover Plan (05 mins):** Reconfirm execution window, on-call bridge, and fallback triggers.
4. **Final Stakeholder Poll (05 mins):**
   * *QA Lead:* "GO" / "NO-GO"
   * *Engineering Lead:* "GO" / "NO-GO"
   * *Operations/Sec Lead:* "GO" / "NO-GO"
   * *Product Manager:* "GO" / "NO-GO"
5. **Decision Sign-off (05 mins):** Release Lead logs decision in ServiceNow/Jira and announces release window to all channels.
