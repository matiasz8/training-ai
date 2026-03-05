# Theory — Machine Learning Fundamentals

## 1) ¿Qué es Machine Learning?
Es una forma de crear sistemas que aprenden patrones a partir de datos para hacer predicciones o decisiones.

## 2) Tipos principales
- Supervisado: hay variable objetivo (`y`).
	- Regresión: predecir valores continuos.
	- Clasificación: predecir clases/categorías.
- No supervisado: no hay `y`.
	- Clustering: encontrar grupos naturales.

## 3) Pipeline básico de ML
1. Definir problema.
2. Preparar datos.
3. Separar train/validation/test.
4. Entrenar modelo baseline.
5. Evaluar con métricas correctas.
6. Ajustar y comparar.

## 4) Métricas clave
- Regresión: MAE, MSE, RMSE, $R^2$.
- Clasificación: accuracy, precision, recall, F1, AUC.
- Regla: elegir métrica según impacto de error en negocio.

## 5) Riesgos comunes
- Overfitting: el modelo memoriza train.
- Underfitting: modelo demasiado simple.
- Data leakage: usar información futura o indirecta.
- Split incorrecto: train/test mal separados.

## 6) Buenas prácticas
- Comenzar por un baseline simple.
- Comparar modelos con validación cruzada.
- Usar pipelines reproducibles de `scikit-learn`.
- Documentar decisiones y supuestos.

## 7) Checklist de comprensión
- ¿Podés elegir entre regresión o clasificación según problema?
- ¿Sabés seleccionar una métrica adecuada?
- ¿Podés detectar overfitting en resultados?
