# AI Use-Case Portfolio

## Principle

Do not force every opportunity into generative AI.

| Use case | Primary pattern | Why |
|---|---|---|
| Customer support copilot | RAG + read-only tools | Unstructured knowledge + live customer context |
| Invoice exception triage | Rules + workflow + optional AI extraction | Repetitive process with structured controls |
| Sales proposal assistant | Retrieval + CRM tools + generation | Synthesis across product/customer context |
| Supplier risk assistant | Tools + retrieval + deterministic policy | Structured supplier data + policies |
| Demand forecasting | Analytics / ML | Prediction problem |
| Employee policy assistant | RAG | Large unstructured policy corpus |
| Management reporting | Data pipeline + BI + narrative generation | Facts should come from governed metrics |
| Autonomous purchase approval | **Do not prioritize** | High authority; controlled workflow captures value with less risk |

## Use-case card

Each candidate should define:

- business problem and user;
- baseline and desired outcome;
- AI contribution;
- non-AI components;
- systems of record;
- data classification;
- permissions;
- human-control point;
- failure modes;
- success metrics;
- delivery effort.

## Example: support copilot

AI contributes classification, knowledge retrieval, interaction summarization and response drafting.

Normal software remains responsible for authentication, authorization, CRM truth, refund thresholds, ticket state and audit.

Scale only when quality, adoption, latency, cost and critical-risk thresholds are all acceptable.

## Anti-use-case

"Put an LLM in every workflow" is rejected.

Some problems need normal code, some need workflow automation, and some need predictive ML. Transformation quality is demonstrated by technology-selection discipline, not LLM volume.
