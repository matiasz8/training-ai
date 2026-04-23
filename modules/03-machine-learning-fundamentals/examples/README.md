# Examples — Machine Learning Fundamentals

## Ejemplo 1 — Baseline de regresión

Entrenar regresión lineal y medir MAE/MSE.

## Ejemplo 2 — Clasificación binaria

Entrenar un clasificador simple y evaluar matriz de confusión.

## Ejemplo 3 — Validación cruzada

Comparar performance usando `KFold`.

## Ejemplo 4 — Tuning básico

Aplicar `GridSearchCV` sobre hiperparámetros mínimos.

## Reglas

- Cada ejemplo debe explicar entrada, salida y criterio de éxito.
- Guardar observaciones en `notes/`.

## Ejemplos disponibles

### Scripts ejecutables (piloto Fase 2)

1. `01_train_test_split_baseline.py`

   - Baseline de clasificacion binaria con `train_test_split` reproducible.
   - Salida esperada: `Accuracy` y `F1 score` mayores a 0.90.

1. `02_linear_vs_logistic_baseline.py`

   - Comparacion de baseline de regresion y baseline de clasificacion.
   - Salida esperada: `MAE` para diabetes + `Accuracy` para breast_cancer.

## Como usar estos ejemplos

```bash
python modules/03-machine-learning-fundamentals/examples/01_train_test_split_baseline.py
python modules/03-machine-learning-fundamentals/examples/02_linear_vs_logistic_baseline.py
```

Recomendacion: ejecutar primero el ejemplo 01 y luego modificar `test_size` para
observar estabilidad de metricas.

## Proximos pasos

1. Agregar ejemplos L2 de regularizacion y control de overfitting.
1. Conectar estos baselines con una practica de comparacion de modelos.
1. Registrar resultados y observaciones en `notes/README.md`.
