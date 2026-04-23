# Guardrails — Safety and Control for LLMs

## Ejemplos disponibles

- `01-input-validation.py`

  - Blocks prompt-injection and SQL-injection style inputs.
  - Expected output: clear allow/deny decisions with reasons.

- `02-output-filtering.py`

  - Applies output filtering for PII redaction, toxicity, and policy checks.
  - Expected output: safe output or blocked response with issue list.

- `03-nemo-guardrails-demo.py`

  - Conceptual NeMo Guardrails flow with input/output rails.
  - Expected output: stage-aware blocking (`input` or `output`) when a rail is triggered.

- `04_reproducible_guardrail_audit.py`

  - Deterministic guardrail audit over a small test set.
  - Expected output: repeated runs produce `same_result=True`.

## Como usar estos ejemplos

```bash
python trends-extras/guardrails/examples/01-input-validation.py
python trends-extras/guardrails/examples/02-output-filtering.py
python trends-extras/guardrails/examples/03-nemo-guardrails-demo.py
python trends-extras/guardrails/examples/04_reproducible_guardrail_audit.py
```

Recommended order: validation (`01`) -> filtering (`02`) -> orchestration (`03`)
-> reproducible audit (`04`).

## Proximos pasos

1. Add a threshold-tuning example for false-positive/false-negative trade-offs.
1. Add a policy versioning example with changelog-driven tests.
1. Convert one script into a guided practice in `practices/`.
