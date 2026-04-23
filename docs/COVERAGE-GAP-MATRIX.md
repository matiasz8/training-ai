# Matriz de Cobertura y Brechas (Fase 1)

## Objetivo

Establecer una matriz objetiva de cobertura tema-subtema-modulo y priorizar brechas con P0/P1/P2 para guiar la ejecucion del plan.

## Metodo y evidencia

Fuente curricular base:

- `docs/init-path/content/*.md` (12 temas core).
- `docs/LEARNING-PATH.md` (secuencia oficial de estudio).

Snapshot tecnico (2026-04-23):

- Modulos core con ejemplos Python ejecutables: 0 en 12/12 modulos.
- Modulos core con ejemplos Markdown: 3 por modulo.
- Placeholders en core (`Pendiente de completar este apartado.`): 121.
- Placeholders en extras: 36.
- Ejemplos Python por extra:
  - `agents`: 3
  - `ai-observability`: 4
  - `guardrails`: 3
  - `llm-evals`: 4
  - `multimodal`: 4
  - `synthetic-data`: 3

## Matriz Tema -> Modulo -> Estado

| Tema (init-path)                          | Modulo destino                                      | Estado actual | Prioridad | Accion principal                                                |
| ----------------------------------------- | --------------------------------------------------- | ------------- | --------- | --------------------------------------------------------------- |
| Programming & Math for ML                 | `modules/01-programming-math-for-ml`                | Parcial       | P0        | Migrar ejemplos clave a `.py` ejecutables + salidas esperadas   |
| Data Collection, Cleaning & Visualization | `modules/02-data-collection-cleaning-visualization` | Parcial       | P0        | Ejemplos ejecutables de limpieza + EDA reproducible             |
| Machine Learning Fundamentals             | `modules/03-machine-learning-fundamentals`          | Parcial       | P0        | Baselines de clasificacion/regresion con metricas y comparacion |
| Deep Learning Basics                      | `modules/04-deep-learning-basics`                   | Parcial       | P0        | Entrenamiento minimo reproducible (MLP/CNN) con overfit checks  |
| NLP & Large Language Models               | `modules/05-nlp-large-language-models`              | Parcial       | P0        | Pipeline NLP/LLM ejecutable (prompting + eval minima)           |
| Computer Vision                           | `modules/06-computer-vision`                        | Parcial       | P0        | Ejemplos ejecutables CV con inferencia y validacion basica      |
| Time Series & Anomaly Detection           | `modules/07-time-series-anomaly-detection`          | Parcial       | P0        | Forecast + deteccion de anomalias con metricas temporales       |
| Recommender Systems                       | `modules/08-recommender-systems`                    | Parcial       | P0        | CF baseline + ranking metrics reproducibles                     |
| Generative AI & Prompt Engineering        | `modules/09-generative-ai-prompt-engineering`       | Parcial       | P0        | Ejemplos de prompting y evaluacion de calidad por casos         |
| Ethics, Bias & Explainability             | `modules/10-ethics-bias-explainability`             | Parcial       | P1        | Ejemplos guiados de fairness y SHAP/LIME aplicados              |
| Data Privacy & Security                   | `modules/11-data-privacy-security`                  | Parcial       | P1        | Ejemplos de redaccion, anonimizado y controles minimos          |
| MLOps & AI in Production                  | `modules/12-mlops-ai-in-production`                 | Parcial       | P0        | Ejemplos ejecutables de serving, monitoreo y rollback           |

## Brechas transversales priorizadas

### P0 (bloqueantes para aprendizaje ejecutable)

1. Core sin scripts `.py` ejecutables en `examples/` (12/12 modulos).
1. Alto volumen de placeholders en modulos core (121).
1. Falta de salida esperada explicita por ejemplo en la mayoria del core.

### P1 (impacto alto, no bloqueante inmediato)

1. Extras por debajo del objetivo de densidad (target 4-6): `agents`, `guardrails`, `synthetic-data` tienen 3.
1. Placeholders residuales en extras (36).
1. Desalineacion narrativa: documentos que hablan de 100% completo vs evidencia de parcialidad ejecutable.

### P2 (expansion de cobertura avanzada)

1. RL aplicado para producto.
1. Causal ML introductorio.
1. Graph ML introductorio.
1. Evals avanzadas y red-teaming sistematico.
1. Optimizacion de inferencia (quantization/distillation/serving).

## Backlog inicial recomendado (orden de ejecucion)

1. Completar placeholders P0 en modulos 03 y 05 (piloto).
1. Publicar 6-8 ejemplos ejecutables en modulo 03.
1. Publicar 6-8 ejemplos ejecutables en modulo 05.
1. Definir rubrica de salida esperada y errores comunes para todo ejemplo nuevo.
1. Escalar el patron a olas A/B/C del core.

## Criterio de cierre de Fase 1

1. Matriz publicada y versionada (este documento).
1. Brechas P0/P1/P2 acordadas.
1. Piloto de ejecucion definido (M03 y M05).
