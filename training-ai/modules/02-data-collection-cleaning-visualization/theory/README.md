# Theory — Data Collection, Cleaning & Visualization

## 1) Por qué este módulo importa
Un modelo no puede ser mejor que sus datos. Si los datos están incompletos, sesgados o mal estructurados, el modelo aprenderá errores.

## 2) Recolección de datos (Data Collection)
- Fuentes comunes:
	- Archivos CSV/Excel.
	- APIs.
	- Bases de datos.
	- Datos internos de negocio.
- Criterios iniciales:
	- Relevancia para el problema.
	- Volumen mínimo útil.
	- Calidad y actualidad.
	- Restricciones legales/privacidad.

## 3) Calidad de datos
Dimensiones básicas:
- Completitud: ¿faltan valores?
- Consistencia: ¿formato y reglas coherentes?
- Unicidad: ¿hay duplicados?
- Validez: ¿los valores están en rango?
- Puntualidad: ¿datos actualizados?

## 4) Limpieza de datos (Data Cleaning)
Pasos mínimos:
- Estandarizar nombres de columnas y tipos de datos.
- Tratar nulos (eliminar, imputar, marcar).
- Eliminar duplicados.
- Detectar y tratar outliers.
- Corregir errores de formato (fechas, decimales, categorías).

## 5) Visualización y EDA
- Objetivo del EDA: entender estructura, distribución y relaciones.
- Gráficos base:
	- Histograma: distribución de una variable.
	- Boxplot: dispersión y outliers.
	- Scatter: relación entre dos variables.
	- Heatmap de correlación: dependencias lineales.

## 6) Buenas prácticas
- Crear pipeline reproducible (pasos claros).
- Evitar modificar datos originales sin respaldo.
- Documentar supuestos y transformaciones.
- Separar claramente train/validation/test antes de modelar.

## 7) Checklist de comprensión
- ¿Podés detectar 3 problemas de calidad en un dataset?
- ¿Sabés elegir una estrategia de imputación según contexto?
- ¿Podés justificar una visualización para una decisión técnica?
