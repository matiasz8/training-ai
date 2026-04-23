# Examples — NLP & Large Language Models

## Example 1 — Cleaning and tokenization

Preprocess text for classification tasks.

## Example 2 — TF-IDF plus classifier

Train a text-classification baseline.

## Example 3 — Embeddings and similarity

Compare sentences by semantic proximity.

## Example 4 — Basic LLM prompting

Design a structured prompt and evaluate the output.

## Rules

- Define the objective and success criteria for each example.
- Record errors and improvements in `notes/`.

## Ejemplos disponibles

### Executable scripts (phase-2 pilot)

1. `01_text_preprocessing_baseline.py`

   - Minimal normalization and tokenization pipeline.
   - Expected output: cleaned tokens per sentence.

1. `02_embeddings_similarity_baseline.py`

   - Semantic similarity with TF-IDF and cosine similarity.
   - Expected output: similarity A-B higher than similarity A-C.

1. `03_prompt_variants_quality.py`

   - Comparison of weak/medium/strong prompts with a simple rubric.
   - Expected output: prompt-quality score increases with prompt strength.

1. `04_chunking_strategies_rag.py`

   - Comparison of fixed-size versus sentence-based chunking for retrieval.
   - Expected output: score differences and a different top retrieved chunk.

1. `05_rag_minimal_eval.py`

   - Minimal exact-match evaluation over a simplified RAG flow.
   - Expected output: run-level `exact_match_avg`.

1. `06_llm_workflow_with_guardrails.py`

   - Workflow with input and output guardrails for sensitive prompts.
   - Expected output: one allowed case and one blocked case.

## Como usar estos ejemplos

```bash
python modules/05-nlp-large-language-models/examples/01_text_preprocessing_baseline.py
python modules/05-nlp-large-language-models/examples/02_embeddings_similarity_baseline.py
python modules/05-nlp-large-language-models/examples/03_prompt_variants_quality.py
python modules/05-nlp-large-language-models/examples/04_chunking_strategies_rag.py
python modules/05-nlp-large-language-models/examples/05_rag_minimal_eval.py
python modules/05-nlp-large-language-models/examples/06_llm_workflow_with_guardrails.py
```

Recommendation: change the input sentences and compare how the similarity shifts.

## Proximos pasos

1. Add an L4 example for output evaluation with an expanded rubric.
1. Integrate these examples with `guardrails` and `llm-evals` practices.
1. Document common tokenization and vocabulary issues in `notes/README.md`.
