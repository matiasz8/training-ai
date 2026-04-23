# Examples — Computer Vision

## Ejemplo 1 — Carga y visualización de imágenes

Leer dataset de imágenes y visualizar muestras por clase.

## Ejemplo 2 — Preprocesamiento base

Aplicar resize, normalización y split train/validation/test.

## Ejemplo 3 — CNN mínima

Entrenar una CNN pequeña y reportar accuracy.

## Ejemplo 4 — Análisis de errores

Usar matriz de confusión para encontrar clases difíciles.

## Reglas

- Explicar entrada, salida y criterio de éxito.
- Mantener reproducibilidad del entrenamiento.

## Ejemplos disponibles

### Scripts ejecutables (piloto Fase 2)

1. `01_image_matrix_basics.py`

   - Operaciones basicas sobre matriz de imagen en escala de grises.
   - Salida esperada: min/max/media y valor normalizado.

1. `02_convolution_baseline.py`

   - Convolucion 2D valida con kernel tipo deteccion de bordes.
   - Salida esperada: matriz de salida de la convolucion.

1. `03_edge_detection_filter.py`

   - Filtros Sobel-like para gradientes X e Y.
   - Salida esperada: mapas de gradiente diferenciados.

1. `04_iou_metric_demo.py`

   - Calculo de IoU para cajas de deteccion.
   - Salida esperada: `iou_good` mayor que `iou_bad`.

1. `05_object_detection_nms_demo.py`

   - Supresion de no maximos (NMS) en detecciones solapadas.
   - Salida esperada: menos cajas despues de NMS.

1. `06_cv_pipeline_reproducible.py`

   - Pipeline minimo reproducible con augmentacion deterministica.
   - Salida esperada: `same_result=True` con seed igual.

## Como usar estos ejemplos

```bash
python modules/06-computer-vision/examples/01_image_matrix_basics.py
python modules/06-computer-vision/examples/02_convolution_baseline.py
python modules/06-computer-vision/examples/03_edge_detection_filter.py
python modules/06-computer-vision/examples/04_iou_metric_demo.py
python modules/06-computer-vision/examples/05_object_detection_nms_demo.py
python modules/06-computer-vision/examples/06_cv_pipeline_reproducible.py
```

Recomendacion: correr 01-03 antes de 04-05 para reforzar base de representacion y filtros.

## Proximos pasos

1. Agregar ejemplo de mAP simplificado para evaluacion de deteccion.
1. Integrar NMS e IoU en una practica de pipeline end-to-end.
1. Registrar errores comunes de cajas y filtros en `notes/README.md`.
