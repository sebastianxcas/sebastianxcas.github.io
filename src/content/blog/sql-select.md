---
title: 'SQL: seleccionar y ordenar datos'
description: 'SELECT, WHERE y ORDER BY con un ejemplo ilustrativo.'
pubDate: 2026-11-07
author: Sebastián Castellanos Parra
tags: ['SQL']
---

Una consulta permite pedir solo la información que se necesita. Los siguientes ejemplos son ilustrativos y usan nombres de tablas y columnas hipotéticos.

```sql
SELECT nombre, ciudad
FROM sede
WHERE ciudad = 'Bogotá'
ORDER BY nombre;
```

`SELECT` indica las columnas; `FROM` identifica la tabla; `WHERE` filtra las filas y `ORDER BY` ordena el resultado. `DISTINCT` puede eliminar filas duplicadas del resultado proyectado.

## Precisión al filtrar

Las cadenas se escriben entre comillas simples. Para comprobar ausencia de valor se usa `IS NULL` o `IS NOT NULL`, en lugar de comparar con `= NULL`. Las reglas de comparación, fechas y ordenamiento pueden variar según el gestor.

El material del curso se puede consultar en las [vistas de SQL](/work/#sql).
