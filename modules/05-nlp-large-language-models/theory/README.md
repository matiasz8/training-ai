# Theory — NLP & Large Language Models

## 1) ¿Qué es NLP?
NLP (Natural Language Processing) permite que sistemas computacionales entiendan, procesen y generen lenguaje humano.

## 2) Pipeline clásico de NLP
- Recolección de texto.
- Limpieza (lowercase, puntuación, stopwords según caso).
- Tokenización.
- Representación numérica (BoW, TF-IDF, embeddings).
- Modelado y evaluación.

## 3) Conceptos clave
- Token: unidad mínima de texto.
- Embedding: representación vectorial de palabras/frases.
- Similitud semántica: cercanía de significado en espacio vectorial.

## 4) Tareas frecuentes
- Clasificación de texto (spam, intención, sentimiento).
- Extracción de entidades (NER).
- Búsqueda semántica.
- Resumen y generación.

## 5) LLMs: base conceptual
- Modelos grandes entrenados sobre enormes corpus textuales.
- Pueden generar texto, resumir, responder, clasificar y razonar de forma aproximada.
- No son infalibles: pueden alucinar.

## 6) Prompting y evaluación
- Prompt claro + contexto relevante + formato esperado.
- Evaluar calidad por:
	- Correctitud
	- Relevancia
	- Consistencia
	- Seguridad

## 7) Buenas prácticas
- Empezar por baseline clásico antes de saltar a LLM.
- Medir con métricas y ejemplos de error.
- Guardar prompts y resultados para comparar iteraciones.

## 8) Checklist de comprensión
- ¿Podés explicar diferencia entre TF-IDF y embeddings?
- ¿Sabés cuándo usar un modelo clásico vs LLM?
- ¿Podés diseñar un prompt con contexto y formato de salida?
