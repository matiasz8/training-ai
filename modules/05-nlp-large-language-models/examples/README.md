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

## Como usar estos ejemplos

```bash
python modules/05-nlp-large-language-models/examples/01_text_preprocessing_baseline.py
python modules/05-nlp-large-language-models/examples/02_embeddings_similarity_baseline.py
```

Recomendacion: cambiar oraciones de entrada y comparar como se mueve la similitud.

## Proximos pasos

1. Agregar ejemplo de prompting con evaluacion minima de calidad.
1. Agregar ejemplo de chunking para flujo RAG basico.
1. Documentar errores comunes de tokenizacion y vocabulario en `notes/README.md`.
