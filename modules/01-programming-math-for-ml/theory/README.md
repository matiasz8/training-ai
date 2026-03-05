# Theory — Programación y Matemática para ML

## 1) Por qué este módulo importa
Sin base matemática y de programación, usar modelos se vuelve una caja negra. Este módulo te da herramientas para entender qué hace un modelo, por qué falla y cómo mejorarlo.

## 2) Python esencial para ML (desde 0)
- Tipos de datos: `int`, `float`, `str`, `list`, `dict`.
- Control de flujo: `if`, `for`, `while`, funciones.
- Librerías base:
	- `NumPy`: operaciones numéricas y vectores/matrices.
	- `Pandas`: manipulación tabular.
	- `Matplotlib`: visualización básica.

## 3) Álgebra lineal aplicada
- Escalares, vectores y matrices.
- Operaciones principales:
	- Suma/resta de vectores.
	- Producto punto.
	- Multiplicación de matrices.
- Intuición ML: un modelo lineal combina características usando pesos.

## 4) Cálculo aplicado a optimización
- Derivada: mide cambio local.
- Derivada parcial: cambio respecto a una variable.
- Regla de la cadena: base conceptual para backpropagation.
- Intuición ML: si conocés la pendiente del error, podés ajustar parámetros en la dirección correcta.

## 5) Probabilidad y estadística
- Media, mediana, varianza, desvío estándar.
- Probabilidad condicional y teorema de Bayes.
- Distribuciones comunes (normal, binomial).
- Intuición ML: entender ruido, incertidumbre y calibración de predicciones.

## 6) Optimización
- Función de costo: mide qué tan mal predice el modelo.
- Gradiente descendente:
	- Elegir tasa de aprendizaje.
	- Actualizar parámetros iterativamente.
	- Detectar convergencia.

## 7) Reproducibilidad mínima
- Fijar semillas aleatorias.
- Separar datos de entrenamiento y validación.
- Guardar experimentos y decisiones en `notes/`.

## 8) Checklist de comprensión
- ¿Podés explicar qué es una derivada con un ejemplo?
- ¿Podés calcular un producto punto en Python?
- ¿Podés interpretar media y varianza en un dataset?
- ¿Podés implementar una actualización de gradiente?
