# Backlog de Ejemplos Ejecutables (Piloto Fase 2)

## Objetivo del piloto

Validar esfuerzo real y claridad didactica con dos modulos de alto impacto:

1. `modules/03-machine-learning-fundamentals`
1. `modules/05-nlp-large-language-models`

Meta por modulo en piloto:

- 6 ejemplos `.py` ejecutables.
- README de ejemplo con salida esperada.
- 1 variacion sugerida + 1 bloque de errores comunes por ejemplo.

## Modulo 03 - Machine Learning Fundamentals

### L1 (baseline guiado)

1. `examples/01_train_test_split_baseline.py`
1. `examples/02_linear_vs_logistic_baseline.py`

### L2 (variaciones controladas)

1. `examples/03_regularization_tradeoffs.py`
1. `examples/04_tree_depth_vs_overfitting.py`

### L3 (caso realista + metricas)

1. `examples/05_model_comparison_metrics.py`

### L4 (extension de mantenibilidad)

1. `examples/06_reproducible_ml_pipeline.py`

## Modulo 05 - NLP & Large Language Models

### L1 (baseline guiado)

1. `examples/01_text_preprocessing_baseline.py`
1. `examples/02_embeddings_similarity_baseline.py`

### L2 (variaciones controladas)

1. `examples/03_prompt_variants_quality.py`
1. `examples/04_chunking_strategies_rag.py`

### L3 (caso realista + metricas)

1. `examples/05_rag_minimal_eval.py`

### L4 (extension de mantenibilidad)

1. `examples/06_llm_workflow_with_guardrails.py`

## Definition of Done del piloto

1. Cada ejemplo ejecuta con un comando unico.
1. Cada ejemplo documenta salida esperada minima.
1. Cada ejemplo incluye una variacion controlada.
1. Cada ejemplo incluye errores comunes y debug rapido.
1. Pre-commit en verde para archivos nuevos.
1. Validacion de contrato en verde.
