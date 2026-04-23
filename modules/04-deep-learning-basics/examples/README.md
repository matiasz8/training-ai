# Examples — Deep Learning Basics

## Ejemplo 1 — Primera red neuronal

Entrenar una MLP simple para clasificación binaria.

## Ejemplo 2 — Curvas de entrenamiento

Visualizar loss y accuracy en train/validation por época.

## Ejemplo 3 — Dropout y regularización

Comparar resultados con y sin regularización.

## Ejemplo 4 — Ajuste de hiperparámetros

Evaluar impacto de learning rate, batch size y número de capas.

## Reglas

- Incluir objetivo, entrada, salida esperada y errores comunes.
- Mantener notebooks/scripts reproducibles.

## Ejemplos disponibles

### Scripts ejecutables (piloto Fase 2)

1. `01_neuron_forward_baseline.py`

   - Forward pass de una neurona con activacion sigmoide.
   - Salida esperada: `output_a` y `output_b` entre 0 y 1.

1. `02_gradient_descent_baseline.py`

   - Entrenamiento de un parametro con gradient descent.
   - Salida esperada: descenso progresivo de `mse`.

1. `03_activation_functions_comparison.py`

   - Comparacion de ReLU, tanh y sigmoid en entradas comunes.
   - Salida esperada: tabla con diferencias de comportamiento.

1. `04_overfitting_regularization_simulation.py`

   - Simulacion de overfitting y seleccion con penalizacion.
   - Salida esperada: cambio de modelo seleccionado segun `alpha`.

1. `05_simple_mlp_from_scratch.py`

   - Forward pass de una MLP pequena sin frameworks.
   - Salida esperada: predicciones reproducibles por muestra.

1. `06_reproducible_training_loop.py`

   - Loop de entrenamiento reproducible con seed fija.
   - Salida esperada: dos corridas identicas (`same_result=True`).

## Como usar estos ejemplos

```bash
python modules/04-deep-learning-basics/examples/01_neuron_forward_baseline.py
python modules/04-deep-learning-basics/examples/02_gradient_descent_baseline.py
python modules/04-deep-learning-basics/examples/03_activation_functions_comparison.py
python modules/04-deep-learning-basics/examples/04_overfitting_regularization_simulation.py
python modules/04-deep-learning-basics/examples/05_simple_mlp_from_scratch.py
python modules/04-deep-learning-basics/examples/06_reproducible_training_loop.py
```

Recomendacion: ejecutar del 01 al 06 en orden para conservar progresion conceptual.

## Proximos pasos

1. Incorporar variante L4 con mini-batch training y early stopping.
1. Conectar ejemplos 04 y 06 con practicas de generalizacion.
1. Documentar observaciones de estabilidad en `notes/README.md`.
