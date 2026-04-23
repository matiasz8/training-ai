# Examples — Generative AI & Prompt Engineering

## Example 1 — Baseline prompt

Design an initial prompt for a summarization task.

## Example 2 — Structured prompt

Add an output format and explicit constraints.

## Example 3 — Guided iteration

Improve the prompt with feedback about errors.

## Example 4 — Basic guardrails

Include validations for safe and useful responses.

## Rules

- Record the prompt version and the obtained result.
- Compare quality across iterations.

## Ejemplos disponibles

### Executable scripts (phase-2 continuation)

1. `01_prompt_baseline_quality.py`

   - Scores weak vs improved prompts with simple quality heuristics.
   - Expected output: improved prompt should score higher.

1. `02_structured_prompt_constraints.py`

   - Builds a structured prompt with task, context, constraints, and output format.
   - Expected output: deterministic template-ready prompt text.

1. `03_prompt_iteration_feedback_loop.py`

   - Runs iterative prompt refinement with feedback rounds.
   - Expected output: quality score increases across iterations.

1. `04_guardrails_input_output.py`

   - Applies input/output guardrails for sensitive terms.
   - Expected output: safe prompt allowed, unsafe prompt blocked.

1. `05_rag_prompt_pipeline_demo.py`

   - Demonstrates retrieval plus context-injected prompt building.
   - Expected output: selected context and preview of RAG prompt.

1. `06_reproducible_prompt_evaluation.py`

   - Runs deterministic prompt evaluation using a fixed seed.
   - Expected output: repeated runs produce identical score values.

## Como usar estos ejemplos

```bash
python modules/09-generative-ai-prompt-engineering/examples/01_prompt_baseline_quality.py
python modules/09-generative-ai-prompt-engineering/examples/02_structured_prompt_constraints.py
python modules/09-generative-ai-prompt-engineering/examples/03_prompt_iteration_feedback_loop.py
python modules/09-generative-ai-prompt-engineering/examples/04_guardrails_input_output.py
python modules/09-generative-ai-prompt-engineering/examples/05_rag_prompt_pipeline_demo.py
python modules/09-generative-ai-prompt-engineering/examples/06_reproducible_prompt_evaluation.py
```

Recommended order: baseline -> structure -> iteration -> guardrails -> RAG -> reproducibility.

## Proximos pasos

1. Add a lightweight prompt regression test harness.
1. Add side-by-side prompt variants for cost/latency trade-off analysis.
1. Document practical prompt anti-patterns in `notes/README.md`.
