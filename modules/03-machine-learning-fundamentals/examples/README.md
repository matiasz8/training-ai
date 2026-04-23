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

1. `03_regularization_tradeoffs.py`

   - Efecto de regularizacion L2 sobre pesos y error.
   - Salida esperada: cambio de `w`, `train_mse` y `test_mse` segun `lambda`.

1. `04_tree_depth_vs_overfitting.py`

   - Simulacion de comportamiento de sobreajuste por complejidad.
   - Salida esperada: `train_acc` alta con generalizacion menor.

1. `05_model_comparison_metrics.py`

   - Comparacion de modelos con `accuracy`, `precision`, `recall` y `f1`.
   - Salida esperada: diferencias de ranking segun metrica.

1. `06_reproducible_ml_pipeline.py`

   - Pipeline minimo reproducible con seed fijo.
   - Salida esperada: `threshold` y `accuracy` estables entre ejecuciones.

## Como usar estos ejemplos

```bash
python modules/03-machine-learning-fundamentals/examples/01_train_test_split_baseline.py
python modules/03-machine-learning-fundamentals/examples/02_linear_vs_logistic_baseline.py
python modules/03-machine-learning-fundamentals/examples/03_regularization_tradeoffs.py
python modules/03-machine-learning-fundamentals/examples/04_tree_depth_vs_overfitting.py
python modules/03-machine-learning-fundamentals/examples/05_model_comparison_metrics.py
python modules/03-machine-learning-fundamentals/examples/06_reproducible_ml_pipeline.py
```

Recomendacion: ejecutar primero el ejemplo 01 y luego modificar `test_size` para
observar estabilidad de metricas.

## Proximos pasos

1. Conectar estos ejemplos con practicas de comparacion de modelos.
1. Agregar un ejemplo L4 con validacion cruzada automatizada.
1. Registrar resultados y observaciones en `notes/README.md`.
