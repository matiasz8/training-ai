# Theory — Computer Vision

## 1) ¿Qué es Computer Vision?
Es el área de IA que permite a los sistemas interpretar imágenes y videos para detectar patrones, objetos o eventos.

## 2) Fundamentos de imagen digital
- Imagen = matriz de píxeles.
- Escala de grises: un canal.
- RGB: tres canales.
- Resolución: cantidad de píxeles (impacta calidad y costo computacional).

## 3) Preprocesamiento
- Resize: unificar dimensiones.
- Normalización: escalar valores de píxeles.
- Data augmentation: rotaciones, flips, zoom, ruido.
- Objetivo: mejorar generalización del modelo.

## 4) Modelos básicos
- MLP sobre píxeles (baseline simple).
- CNN:
	- Convoluciones para extraer patrones locales.
	- Pooling para reducir dimensionalidad.
	- Capas densas para clasificación final.

## 5) Métricas en visión
- Accuracy.
- Precision/Recall/F1 (si hay desbalance).
- Matriz de confusión para analizar errores por clase.

## 6) Errores comunes
- Dataset desbalanceado.
- Fuga de datos entre train/test.
- Overfitting por pocas imágenes o poca variación.

## 7) Buenas prácticas
- Empezar con baseline simple.
- Usar split estricto y reproducible.
- Analizar errores visualmente.
- Medir impacto de cada cambio (no ajustar todo a la vez).

## 8) Checklist de comprensión
- ¿Podés explicar por qué una CNN suele superar a un MLP en imágenes?
- ¿Sabés cuándo aplicar augmentación?
- ¿Podés detectar clases problemáticas con matriz de confusión?
