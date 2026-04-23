# Examples — MLOps & AI in Production

## Ejemplo 1 — Pipeline reproducible

Versionar datos, entrenamiento y artefactos.

## Ejemplo 2 — Serving básico

Exponer modelo vía API o proceso batch.

## Ejemplo 3 — Monitoreo inicial

Registrar métricas de latencia y calidad.

## Ejemplo 4 — Simulación de drift

Detectar degradación y activar alerta.

## Reglas

- Cada ejemplo debe indicar objetivo operacional.
- Documentar supuestos de infraestructura.

## Ejemplos disponibles

### Executable scripts (phase-2 continuation)

1. `01_reproducible_pipeline_manifest.py`

   - Builds a lightweight manifest for reproducible training runs.
   - Expected output: deterministic version/asset metadata.

1. `02_batch_vs_realtime_serving.py`

   - Chooses serving mode from latency and volume constraints.
   - Expected output: realtime, batch, or hybrid decision.

1. `03_latency_monitoring_baseline.py`

   - Summarizes latency metrics and raises a simple alert.
   - Expected output: average/min/max latency and alert flag.

1. `04_drift_detection_demo.py`

   - Detects simple feature drift from reference vs production means.
   - Expected output: drift score and alert status.

1. `05_canary_rollout_decision.py`

   - Decides whether a canary model should be promoted.
   - Expected output: boolean rollout decision.

1. `06_reproducible_mlops_runbook.py`

   - Produces deterministic runbook metadata using a fixed seed.
   - Expected output: repeated runs with `same_result=True`.

## Como usar estos ejemplos

```bash
python modules/12-mlops-ai-in-production/examples/01_reproducible_pipeline_manifest.py
python modules/12-mlops-ai-in-production/examples/02_batch_vs_realtime_serving.py
python modules/12-mlops-ai-in-production/examples/03_latency_monitoring_baseline.py
python modules/12-mlops-ai-in-production/examples/04_drift_detection_demo.py
python modules/12-mlops-ai-in-production/examples/05_canary_rollout_decision.py
python modules/12-mlops-ai-in-production/examples/06_reproducible_mlops_runbook.py
```

Recommended order: manifest -> serving -> latency -> drift -> canary -> reproducibility.

## Proximos pasos

1. Add a lightweight incident escalation example.
1. Add an offline/online metric comparison example.
1. Record rollout lessons in `notes/README.md`.
