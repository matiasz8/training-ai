# Examples — Ethics, Bias & Explainability

## Ejemplo 1 — Detección de sesgo básico

Revisar distribución por grupos y posibles desbalances.

## Ejemplo 2 — Métrica de fairness

Calcular una métrica de equidad y compararla entre grupos.

## Ejemplo 3 — Explicación local

Usar SHAP/LIME para explicar predicción individual.

## Ejemplo 4 — Reporte de riesgo

Documentar riesgos y mitigaciones en formato breve.

## Reglas

- Evitar conclusiones sin evidencia cuantitativa.
- Registrar supuestos explícitamente.

## Ejemplos disponibles

### Executable scripts (phase-2 continuation)

1. `01_group_distribution_bias_check.py`

   - Checks positive-rate distribution by group.
   - Expected output: group rates and maximum disparity gap.

1. `02_demographic_parity_metric.py`

   - Computes demographic parity difference between groups.
   - Expected output: positive rate per group and DP gap.

1. `03_counterfactual_fairness_check.py`

   - Measures score sensitivity under protected-attribute perturbation.
   - Expected output: factual vs counterfactual score delta.

1. `04_local_explanation_feature_contributions.py`

   - Builds a local explanation via feature contribution breakdown.
   - Expected output: per-feature contributions and final prediction.

1. `05_risk_report_generator.py`

   - Produces a concise model risk report from fairness indicators.
   - Expected output: dictionary-style risk summary.

1. `06_reproducible_ethics_audit_pipeline.py`

   - Runs deterministic ethics audit pipeline with fixed seed.
   - Expected output: identical group rates across repeated runs.

## Como usar estos ejemplos

```bash
python modules/10-ethics-bias-explainability/examples/01_group_distribution_bias_check.py
python modules/10-ethics-bias-explainability/examples/02_demographic_parity_metric.py
python modules/10-ethics-bias-explainability/examples/03_counterfactual_fairness_check.py
python modules/10-ethics-bias-explainability/examples/04_local_explanation_feature_contributions.py
python modules/10-ethics-bias-explainability/examples/05_risk_report_generator.py
python modules/10-ethics-bias-explainability/examples/06_reproducible_ethics_audit_pipeline.py
```

Recommended order: distribution -> fairness metric -> counterfactual -> explanation -> risk report -> reproducibility.

## Proximos pasos

1. Add equalized-odds style checks for classification pipelines.
1. Add a lightweight mitigation demo (thresholding or reweighting).
1. Document governance checklist outcomes in `notes/README.md`.
