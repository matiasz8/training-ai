# Examples — NLP & Large Language Models

## Ejemplo 1 — Limpieza y tokenización

Preprocesar texto para tareas de clasificación.

## Ejemplo 2 — TF-IDF + clasificador

Entrenar un baseline de clasificación textual.

## Ejemplo 3 — Embeddings y similitud

Comparar frases por cercanía semántica.

## Ejemplo 4 — Prompting básico con LLM

Diseñar prompt estructurado y evaluar salida.

## Reglas

- Definir objetivo y criterio de éxito por ejemplo.
- Registrar errores y mejoras en `notes/`.

## Ejemplos disponibles

### Scripts ejecutables (piloto Fase 2)

1. `01_text_preprocessing_baseline.py`

   - Pipeline minimo de normalizacion y tokenizacion.
   - Salida esperada: tokens limpios por frase.

1. `02_embeddings_similarity_baseline.py`

   - Similitud semantica con TF-IDF y cosine similarity.
   - Salida esperada: similitud A-B mayor que similitud A-C.

1. `03_prompt_variants_quality.py`

   - Comparacion de prompts weak/medium/strong con rubrica simple.
   - Salida esperada: score creciente de calidad de prompt.

1. `04_chunking_strategies_rag.py`

   - Comparacion de chunking fijo vs por oraciones para recuperacion.
   - Salida esperada: diferencias de score y chunk top recuperado.

1. `05_rag_minimal_eval.py`

   - Evaluacion minima tipo exact-match sobre flujo RAG simplificado.
   - Salida esperada: `exact_match_avg` de la corrida.

1. `06_llm_workflow_with_guardrails.py`

   - Flujo con guardrails de entrada y salida para prompts sensibles.
   - Salida esperada: caso permitido y caso bloqueado.

## Como usar estos ejemplos

```bash
python modules/05-nlp-large-language-models/examples/01_text_preprocessing_baseline.py
python modules/05-nlp-large-language-models/examples/02_embeddings_similarity_baseline.py
python modules/05-nlp-large-language-models/examples/03_prompt_variants_quality.py
python modules/05-nlp-large-language-models/examples/04_chunking_strategies_rag.py
python modules/05-nlp-large-language-models/examples/05_rag_minimal_eval.py
python modules/05-nlp-large-language-models/examples/06_llm_workflow_with_guardrails.py
```

Recomendacion: cambiar oraciones de entrada y comparar como se mueve la similitud.

## Proximos pasos

1. Agregar un ejemplo L4 de evaluacion de salida con rubrica ampliada.
1. Integrar estos ejemplos con practicas de `guardrails` y `llm-evals`.
1. Documentar errores comunes de tokenizacion y vocabulario en `notes/README.md`.
