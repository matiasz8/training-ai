# Examples — Data Privacy & Security

## Ejemplo 1 — Clasificación de datos

Etiquetar columnas según nivel de sensibilidad.

## Ejemplo 2 — Anonimización básica

Aplicar técnicas simples de enmascaramiento o pseudonimización.

## Ejemplo 3 — Matriz de acceso

Definir roles y permisos mínimos.

## Ejemplo 4 — Checklist de seguridad en pipeline

Revisar puntos críticos de exposición de datos.

## Reglas

- Priorizar controles prácticos y verificables.
- Documentar supuestos y límites.

## Ejemplos disponibles

### Executable scripts (phase-2 continuation)

1. `01_data_classification_matrix.py`

   - Classifies columns by practical sensitivity level.
   - Expected output: mapping from column name to security tier.

1. `02_basic_masking_pseudonymization.py`

   - Demonstrates masking and deterministic pseudonymization.
   - Expected output: masked email and pseudonymized identifier.

1. `03_access_control_matrix.py`

   - Checks role-based access decisions for critical resources.
   - Expected output: allow/deny decisions by role.

1. `04_pipeline_security_checklist.py`

   - Scores a lightweight pipeline security checklist.
   - Expected output: passed checks count over total.

1. `05_prompt_injection_risk_demo.py`

   - Classifies prompt injection risk from suspicious patterns.
   - Expected output: low/medium/high risk labels.

1. `06_reproducible_privacy_audit_pipeline.py`

   - Runs a deterministic privacy audit summary with fixed seed.
   - Expected output: `same_result=True` across repeated runs.

## Como usar estos ejemplos

```bash
python modules/11-data-privacy-security/examples/01_data_classification_matrix.py
python modules/11-data-privacy-security/examples/02_basic_masking_pseudonymization.py
python modules/11-data-privacy-security/examples/03_access_control_matrix.py
python modules/11-data-privacy-security/examples/04_pipeline_security_checklist.py
python modules/11-data-privacy-security/examples/05_prompt_injection_risk_demo.py
python modules/11-data-privacy-security/examples/06_reproducible_privacy_audit_pipeline.py
```

Recommended order: classification -> masking -> access control -> checklist -> prompt injection -> reproducibility.

## Proximos pasos

1. Add a lightweight data-retention enforcement example.
1. Add a secrets-scanning example for config files.
1. Document operational limitations in `notes/README.md`.
