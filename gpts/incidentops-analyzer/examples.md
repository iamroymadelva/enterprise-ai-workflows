# Workflow Examples

This document contains example operational workflows and structured incident analysis patterns for IncidentOps Analyzer.

The examples demonstrate how the workflow system handles staged troubleshooting, escalation readiness, and RCA-oriented operational analysis.

---

# Example 1 — Authentication Incident

## Incident Intake

```text id="6j79g2"
Users unable to access Microsoft 365 services after MFA rollout.

Affected systems:
- Microsoft 365
- Azure AD

Impact:
- Multiple users unable to authenticate
- Service Desk ticket spike

Troubleshooting performed:
- Password resets
- MFA reset attempts
- User unlock attempts
```

---

## Workflow Progression

```text id="i7j8qe"
Incident Intake
      ↓
Authentication Workflow Classification
      ↓
Severity Validation
      ↓
Evidence Review
      ↓
Hypothesis Analysis
      ↓
Escalation Assessment
      ↓
Structured Incident Summary
```

---

## Operational Findings

### Probable Hypotheses

| Hypothesis                      | Probability |
| ------------------------------- | ----------- |
| Conditional Access policy issue | High        |
| MFA synchronization delay       | Medium      |
| Identity federation outage      | Low         |

---

## Missing Validation

* Azure AD sign-in logs
* Conditional Access evaluation results
* MFA policy deployment timeline

---

## Workflow Characteristics

This workflow demonstrates:

* staged troubleshooting
* hypothesis-driven analysis
* escalation readiness validation
* structured operational output

---

# Example 2 — Infrastructure Degradation

## Incident Intake

```text id="zcjlwm"
Production application experiencing intermittent latency spikes.

Affected services:
- API gateway
- Internal authentication service

Impact:
- Increased response times
- Elevated support volume
- SLA degradation risk

Recent changes:
- Infrastructure patch deployment 2 hours before degradation
```

---

## Workflow Progression

```text id="mvbl2x"
Infrastructure Incident
      ↓
Operational Context Collection
      ↓
Severity Assessment
      ↓
Change Correlation Analysis
      ↓
Operational Risk Evaluation
      ↓
Escalation Guidance
```

---

## Operational Analysis

### Key Findings

* Incident correlates with recent infrastructure changes
* Latency patterns affect multiple dependent services
* Monitoring alerts indicate elevated API response times

---

## Escalation Readiness Review

| Area                | Status     |
| ------------------- | ---------- |
| Monitoring Evidence | Available  |
| Timeline Clarity    | Partial    |
| Change Correlation  | Identified |
| Infrastructure Logs | Missing    |
| Rollback Validation | Pending    |

---

## Workflow Notes

This workflow demonstrates:

* infrastructure incident analysis
* change correlation logic
* escalation readiness evaluation
* operational impact assessment

---

# Example 3 — API Integration Failure

## Incident Intake

```text id="jlwm9v"
Third-party API integration returning intermittent 502 errors.

Affected systems:
- Payment integration
- Customer checkout flow

Impact:
- Failed transactions
- Customer-facing degradation

Troubleshooting performed:
- API retries validated
- Internal service health confirmed
```

---

## Workflow Lifecycle

```text id="jlwm8u"
API Failure
      ↓
Integration Workflow Routing
      ↓
Evidence Collection
      ↓
Dependency Evaluation
      ↓
Operational Assessment
      ↓
Structured Incident Output
```

---

## Hypothesis Matrix

| Hypothesis                     | Probability | Supporting Evidence              |
| ------------------------------ | ----------- | -------------------------------- |
| Third-party API instability    | High        | External API latency spikes      |
| Internal timeout configuration | Medium      | Retry threshold reached          |
| DNS routing issue              | Low         | No broader connectivity failures |

---

## Missing Validation

* Third-party provider status confirmation
* API gateway trace logs
* Request timing metrics

---

## Workflow Characteristics

This workflow demonstrates:

* dependency-aware troubleshooting
* evidence-based reasoning
* structured hypothesis analysis
* operational escalation preparation

---

# Example 4 — Monitoring Alert Escalation

## Incident Intake

```text id="jlwm7t"
Multiple monitoring alerts triggered across production systems.

Affected areas:
- Database latency
- API response time
- Authentication service health

Severity:
- High

Current concern:
- Possible cascading service degradation
```

---

## Workflow Progression

```text id="jlwm6s"
Monitoring Alerts
      ↓
Severity Validation
      ↓
Operational Correlation
      ↓
Impact Assessment
      ↓
Escalation Evaluation
      ↓
Incident Coordination
```

---

## Operational Assessment

### Current Indicators

* Multiple dependent services impacted
* Escalation threshold reached
* Elevated production risk
* Increased operational load

---

## Recommended Workflow Focus

* confirm degradation scope
* validate infrastructure dependencies
* collect service correlation evidence
* evaluate rollback requirements
* prepare escalation summary

---

# Example 5 — RCA Preparation Workflow

## Incident Context

```text id="jlwm5r"
Major production outage resolved after infrastructure rollback.

Incident duration:
- 47 minutes

Impact:
- Customer authentication failures
- Elevated support ticket volume
- Partial service interruption
```

---

## RCA Workflow

```text id="jlwm4q"
Incident Timeline
      ↓
Evidence Review
      ↓
Root Cause Hypotheses
      ↓
Validation Assessment
      ↓
Contributing Factors
      ↓
RCA Draft Preparation
```

---

## RCA Analysis Areas

* timeline reconstruction
* operational impact analysis
* change correlation
* escalation delays
* contributing factors
* recovery actions

---

## Workflow Characteristics

This workflow demonstrates:

* structured RCA preparation
* incident continuity
* operational reconstruction
* evidence-aware analysis

---

# Workflow Example Summary

The examples throughout this document demonstrate how IncidentOps Analyzer supports:

* structured incident workflows
* escalation-oriented analysis
* staged troubleshooting
* operational continuity
* reusable RCA workflows
* evidence-aware operational reasoning

The workflow system prioritizes operational realism, troubleshooting discipline, and structured incident analysis instead of generic troubleshooting interactions.
