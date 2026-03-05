# Theory — Recommender Systems

## 1) ¿Qué es un sistema de recomendación?
Es un sistema que sugiere ítems relevantes (productos, películas, contenidos) a cada usuario según su historial, perfil o comportamiento similar de otros usuarios.

## 2) Enfoques principales
- Popularidad: recomienda lo más consumido.
- Basado en contenido: recomienda ítems similares a los que ya le gustaron al usuario.
- Filtrado colaborativo:
	- User-based: usuarios similares.
	- Item-based: ítems similares.

## 3) Matriz usuario-ítem
- Filas: usuarios.
- Columnas: ítems.
- Valores: rating, clic, compra o interacción.

## 4) Problemas típicos
- Cold start (usuario o ítem nuevo).
- Sparsity (muchos faltantes en la matriz).
- Popularity bias (siempre recomienda lo popular).

## 5) Métricas offline comunes
- Precision@K
- Recall@K
- MAP@K
- NDCG
- Coverage

## 6) Buenas prácticas
- Partir de baseline simple.
- Separar claramente train/test temporal cuando aplique.
- Medir calidad y diversidad de recomendaciones.
- Auditar sesgos de exposición.

## 7) Checklist de comprensión
- ¿Podés explicar diferencia entre colaborativo y contenido?
- ¿Sabés qué significa cold start?
- ¿Podés justificar una métrica @K para tu caso?
