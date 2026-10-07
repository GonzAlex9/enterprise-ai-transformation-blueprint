# AI Risk Register

## Purpose

A risk register turns vague concern into explicit ownership, mitigation and evidence.

| Risk | Failure mode | Mitigation | Signal |
|---|---|---|---|
| Hallucination | Unsupported answer presented as fact | Grounding, citations, deterministic sources, evals | Unsupported-claim rate |
| Prompt injection | Retrieved/user content changes behavior | Capability limits, instruction/data separation, adversarial evals | Attack-suite results |
| Data leakage | Sensitive data reaches wrong user/model/log | Authz, tenant filtering, minimization, redaction | Access tests, incidents |
| Excessive authority | Model causes high-impact side effect | Least privilege, read/write separation, approvals | Capability review |
| Stale knowledge | Outdated policy used | Versioning, freshness controls, source metadata | Content age |
| Tool failure | Timeout/bad response treated as truth | Explicit errors, retries, fail-closed behavior | Tool error rate |
| Cost runaway | Long loops or excessive context | Token/turn limits, budgets, cost telemetry | Cost/task |
| Low adoption | Users bypass system | Co-design, workflow integration, training | Usage, feedback |
| Automation bias | Humans rubber-stamp poor outputs | Better UX, evidence, sampling | Override/error analysis |
| Model regression | New version degrades behavior | Versioning, regression evals, canary | Eval delta |
| Shadow AI | Ungoverned tool usage | Approved platform, clear policy, fast intake | Tool inventory |

## Risk treatment

For each material risk define:

- probability;
- impact;
- owner;
- mitigation;
- detection signal;
- residual risk;
- review date.

## Important distinction

A model-quality problem and a security-boundary problem are different.

Example:

> The model incorrectly claims that a purchase is approved.

That is a model/action-safety failure.

If the model has no capability to execute that approval, the architecture can still prevent the business effect.

Both layers should be tested.

## Risk principle

> **Design the system so model failure does not automatically become business failure.**
