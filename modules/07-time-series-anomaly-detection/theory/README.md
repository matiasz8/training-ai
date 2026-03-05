# Theory — Time Series & Anomaly Detection

## 1) ¿Qué es una serie temporal?
Es una secuencia de datos ordenados por tiempo. El orden importa porque cada valor puede depender de valores anteriores.

## 2) Componentes principales
- Tendencia: dirección general en el tiempo.
- Estacionalidad: patrones repetitivos periódicos.
- Ruido: variaciones aleatorias.
- Ciclos: variaciones de largo plazo sin período fijo.

## 3) Preparación de datos temporales
- Ordenar por timestamp.
- Verificar frecuencia temporal (diaria, horaria, etc.).
- Manejar faltantes sin romper continuidad.
- Crear features temporales (día, mes, hora, lags).

## 4) Forecasting básico
- Baselines simples:
	- Último valor (naive).
	- Promedio móvil.
- Modelos comunes:
	- ARIMA/SARIMA.
	- Prophet.
	- Modelos de ML con features de lags.

## 5) Métricas de forecasting
- MAE, RMSE, MAPE.
- Recomendación: usar más de una métrica y revisar error visualmente.

## 6) Detección de anomalías
- Enfoques:
	- Umbrales estáticos/dinámicos.
	- Z-score sobre residuales.
	- Isolation Forest / métodos no supervisados.
- Meta: detectar eventos raros con balance entre recall y falsos positivos.

## 7) Buenas prácticas
- Split temporal correcto (sin mezclar futuro en train).
- Validación con ventanas temporales.
- Monitorear drift y cambios de patrón.

## 8) Checklist de comprensión
- ¿Podés identificar tendencia y estacionalidad en un gráfico?
- ¿Sabés por qué no sirve un split aleatorio clásico en series temporales?
- ¿Podés justificar un umbral de anomalía?
