# Theory — Deep Learning Basics

## 1) ¿Qué es Deep Learning?
Es una rama de ML basada en redes neuronales con múltiples capas que aprenden representaciones complejas a partir de datos.

## 2) Conceptos fundamentales
- Neurona artificial: combina entradas, pesos, sesgo y activación.
- Capa: conjunto de neuronas.
- Red neuronal: secuencia de capas (entrada, ocultas, salida).
- Forward pass: cálculo de predicción.

## 3) Funciones de activación
- ReLU: eficiente y simple para capas ocultas.
- Sigmoid: útil en salida binaria.
- Softmax: útil para clasificación multiclase.

## 4) Entrenamiento
- Función de pérdida (loss): mide error.
- Backpropagation: calcula gradientes.
- Optimizadores:
	- SGD
	- Adam

## 5) Overfitting y regularización
- Síntoma: mejora en train pero empeora en validación.
- Técnicas:
	- Dropout
	- Early stopping
	- Regularización L2

## 6) Buenas prácticas
- Empezar con red pequeña (baseline).
- Normalizar datos.
- Monitorear curvas de loss/accuracy.
- Ajustar hiperparámetros de forma ordenada.

## 7) Checklist de comprensión
- ¿Podés explicar la diferencia entre forward y backpropagation?
- ¿Sabés cuándo usar softmax vs sigmoid?
- ¿Podés detectar overfitting en curvas de entrenamiento?
