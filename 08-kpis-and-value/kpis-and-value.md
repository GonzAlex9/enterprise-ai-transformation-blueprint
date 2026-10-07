# KPIs and Value

## Measurement principle

An AI system can score well on model quality and still fail as a product.

Measure five layers together.

## 1. Business KPIs

Examples:

- cycle-time reduction;
- cost per case;
- throughput;
- backlog reduction;
- first-contact resolution;
- conversion, where relevant.

## 2. User / adoption KPIs

Examples:

- weekly active users;
- feature adoption;
- task completion;
- acceptance rate;
- human override / correction;
- user satisfaction.

## 3. AI quality KPIs

Examples:

- grounded response rate;
- task success;
- retrieval hit rate;
- citation accuracy;
- action safety;
- policy fidelity.

## 4. Operational KPIs

Examples:

- p50 / p95 latency;
- error rate;
- tool failure rate;
- tokens per task;
- cost per task;
- availability.

## 5. Risk KPIs

Examples:

- unauthorized-action attempts;
- privacy incidents;
- critical hallucinations;
- policy violations;
- escalation rate.

## Example: support copilot scorecard

| Layer | Metric | Pilot principle |
|---|---|---|
| Business | Median handling time | Improve vs measured baseline |
| Adoption | Weekly agent usage | Sustained real use |
| Quality | Grounded-answer rate | Meet eval threshold |
| Operations | p95 latency | Within agreed SLO |
| Cost | Cost per assisted case | Within business case |
| Risk | Critical data disclosure | **0** |

Exact numeric targets should be set from real baseline data rather than invented before discovery.

## Value equation

```text
Annual value
=
time saved
× task volume
× loaded labor cost
× realized adoption
-
technology cost
-
change cost
-
operating cost
```

Include revenue and risk effects where relevant.

## Avoid vanity metrics

Weak:

- prompts sent;
- number of users invited;
- models tested;
- token volume.

Stronger:

- successful tasks;
- cycle-time reduction;
- quality;
- adoption;
- cost per outcome;
- controlled risk.

## Scale criterion

Scale only when:

> **business value + adoption + quality + operational viability + risk**

are jointly acceptable.
