---
title: 'SQL: unir tablas con JOIN'
description: 'Cómo recuperar información relacionada sin perder de vista la condición.'
pubDate: 2026-11-07
author: Sebastián Castellanos Parra
tags: ['SQL']
---

Un `JOIN` permite combinar datos de dos tablas a partir de una condición. Imaginemos las tablas SEDE y SALA, donde la segunda guarda el código de su sede.

```sql
SELECT se.nombre, sa.numero_sala
FROM sede se
JOIN sala sa ON sa.codigo_sede = se.codigo_sede;
```

Un `INNER JOIN` devuelve las combinaciones que cumplen la condición. Un `LEFT JOIN` conserva las filas de la tabla izquierda aunque no encuentren coincidencia a la derecha, completando con nulos las columnas del otro lado.

Una condición incorrecta u omitida puede producir asociaciones indebidas o muchas más filas de las esperadas. También conviene recordar que un join puede devolver varias filas para una misma sede si esta tiene varias salas.
