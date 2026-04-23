# Examples — Recommender Systems

## Ejemplo 1 — Baseline por popularidad

Construir recomendador simple con top-N global.

## Ejemplo 2 — Item-based colaborativo

Calcular similitud entre ítems y recomendar vecinos.

## Ejemplo 3 — User-based colaborativo

Encontrar usuarios similares y sugerir ítems.

## Ejemplo 4 — Evaluación @K

Calcular Precision@K y Recall@K sobre conjunto de test.

## Reglas

- Cada ejemplo debe incluir entrada, salida esperada y conclusión.
- Registrar hallazgos en `notes/`.

## Ejemplos disponibles

### Executable scripts (phase-2 continuation)

1. `01_popularity_baseline_recommender.py`

   - Builds a top-N baseline using item popularity.
   - Expected output: popularity dictionary and top-3 recommendations.

1. `02_item_similarity_recommender.py`

   - Recommends neighbors from item-to-item cosine similarity.
   - Expected output: ranked neighbor list for a target item.

1. `03_user_similarity_recommender.py`

   - Uses nearest-user logic for user-based recommendations.
   - Expected output: recommendation list for target user.

1. `04_precision_recall_at_k.py`

   - Evaluates recommendation quality at different cutoff values.
   - Expected output: precision@k and recall@k for k in 1..3.

1. `05_cold_start_fallbacks.py`

   - Shows fallback strategies for users with no history.
   - Expected output: popularity-based and tag-based fallback lists.

1. `06_reproducible_recommender_pipeline.py`

   - Runs a deterministic mini pipeline with fixed seed.
   - Expected output: `same_result=True` across repeated runs.

## Como usar estos ejemplos

```bash
python modules/08-recommender-systems/examples/01_popularity_baseline_recommender.py
python modules/08-recommender-systems/examples/02_item_similarity_recommender.py
python modules/08-recommender-systems/examples/03_user_similarity_recommender.py
python modules/08-recommender-systems/examples/04_precision_recall_at_k.py
python modules/08-recommender-systems/examples/05_cold_start_fallbacks.py
python modules/08-recommender-systems/examples/06_reproducible_recommender_pipeline.py
```

Recommended order: run from baseline (`01`) to evaluation (`04`) and then fallback/reproducibility (`05-06`).

## Proximos pasos

1. Add ranking-focused metrics such as NDCG for deeper evaluation.
1. Add a lightweight hybrid recommender demo (content + collaborative).
1. Document practical trade-offs in `notes/README.md`.
