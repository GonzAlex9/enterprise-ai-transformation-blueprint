# Process Discovery

## Why discovery comes first

AI can make a bad process faster without making it better.

Before selecting technology, map actors, decisions, handoffs, systems, delays, exceptions, rework, control points and data availability.

## Process classification

### Deterministic rule
Thresholds, permissions, calculations, validations.

**Default:** normal code or policy engine.

### Repetitive workflow
Routing, copying data, task creation, notifications.

**Default:** workflow automation.

### Prediction
Forecasts, anomaly scores, probabilities.

**Default:** analytics / ML when justified.

### Language or ambiguity
Summarization, intent extraction, document search, evidence synthesis.

**Default:** consider generative AI.

## Discovery output

```text
Process map
   ↓
Pain points
   ↓
Decision points
   ↓
Data + systems
   ↓
Control requirements
   ↓
Candidate interventions
```

Technology selection comes after this sequence.

## Example: customer support

Current:

```text
Ticket → read → search docs → check CRM → draft → escalate
```

Potential:

```text
Ticket
  ↓
AI classification + retrieval
  ↓
CRM read tool
  ↓
Draft with citations
  ↓
Human review for higher-risk categories
  ↓
Send
```

The model can help with language and retrieval without owning refund authority or customer permissions.
