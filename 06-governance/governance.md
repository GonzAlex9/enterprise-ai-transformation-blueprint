# Governance

## Objective

Governance should accelerate safe delivery by making decision rights explicit.

It should answer:

- who owns the business outcome;
- who owns the technical system;
- what risk tier applies;
- what evidence is required before release;
- who can stop or roll back the system.

## Risk tiers

### Tier 1 — Assistive

Examples: summarization, drafting and retrieval.

Controls:

- access control;
- grounding evals;
- privacy review;
- monitoring.

### Tier 2 — Workflow influence

Examples: classification, recommendation, routing and pre-filling operational actions.

Controls:

- Tier 1 controls;
- deterministic validation;
- action-safety evals;
- audit;
- human override;
- stronger release gates.

### Tier 3 — High-impact execution

Examples: financial commitments, permission changes and irreversible external actions.

Controls:

- explicit authorization;
- segregation of duties;
- human approval where appropriate;
- strict audit;
- security review;
- kill switch / rollback;
- zero-tolerance failure classes.

## Lifecycle

```text
Idea
 ↓
Discovery
 ↓
Risk classification
 ↓
Prototype
 ↓
Offline eval
 ↓
Security / privacy review
 ↓
Pilot
 ↓
Production gate
 ↓
Monitoring
 ↓
Scale / redesign / retire
```

## RACI example

| Decision | Business Owner | AI/Product | Engineering | Security/Privacy |
|---|---|---|---|---|
| Problem definition | A/R | C | C | I |
| Architecture | C | A | R | C |
| Risk tier | C | R | C | A |
| Pilot acceptance | A | R | C | C |
| Production release | A | R | R | C |
| Kill / rollback | A | R | R | R |

A = Accountable, R = Responsible, C = Consulted, I = Informed.

## Minimum evidence before scaling

- baseline established;
- target KPI defined;
- representative eval dataset;
- critical failure modes tested;
- privacy/security review complete;
- production owner assigned;
- cost model understood;
- rollback path defined.

## Governance principle

Do not create an AI committee that owns every decision.

Keep accountability with business and technical owners while central governance provides shared standards, risk controls and reusable platform patterns.
