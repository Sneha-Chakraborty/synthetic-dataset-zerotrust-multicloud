# synthetic-dataset-zerotrust-multicloud
Privacy-safe synthetic multi-cloud Zero Trust dataset for benchmarking detection accuracy, FPR, and response time in Research Proposed Work.

Synthetic (privacy-safe) multi-cloud Zero Trust telemetry and security-event dataset with ground-truth labels, created to support the experiments and baseline comparisons in the **AFO-ZT (Analytics-First Orchestration for Zero Trust) in Multi-Cloud** conference paper.

> ✅ **No real user, device, or organizational data is included.**  
> All identities, IPs, timestamps, and events are artificially generated for reproducible research evaluation.

---

## Contents

This repository contains synthetic event logs representing a multi-cloud environment (e.g., AWS/Azure/GCP-style telemetry) covering:

- Authentication and authorization events (SSO/MFA outcomes, policy decisions)
- Device posture/context signals (managed/unmanaged, compliance, risk context)
- Network/API access patterns (resource requests, access attempts)
- Security-relevant behaviors (benign + malicious attempts)
- Ground-truth labels for evaluation (attack vs benign), enabling metrics like:
  - Detection Accuracy
  - False Positive Rate (FPR)
  - Average Response Time (end-to-end decision/mitigation pipeline)

---
## How the Data Was Generated (Method Summary)

The synthetic generator creates multi-cloud log streams by simulating:

1. **Benign user behavior** (normal login → access → session flows)
2. **Context signals** (device posture, geo, time-of-day, risk context)
3. **Policy decisions** (Zero Trust allow/deny/step-up behavior)
4. **Attack injections** (controlled malicious sequences inserted with labels)
5. **Telemetry normalization** into a unified schema for AFO-ZT evaluation

This supports reproducible experiments for analytics-driven policy decisioning and orchestration pipelines.
---
#### This dataset is synthetic and intended for research benchmarking.

