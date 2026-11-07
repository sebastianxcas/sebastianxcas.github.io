---
title: 'SQL: contar, resumir y agrupar'
description: 'COUNT, SUM, GROUP BY y HAVING.'
pubDate: 2026-11-07
author: Sebastián Castellanos Parra
tags: ['SQL']
---

Las funciones de grupo producen un resumen para un conjunto de filas. Entre las más comunes están `COUNT`, `SUM`, `AVG`, `MIN` y `MAX`.

```sql
SELECT codigo_sede, COUNT(*) AS numero_salas
FROM sala
GROUP BY codigo_sede
HAVING COUNT(*) > 2;
```

En este ejemplo hipotético, `GROUP BY` forma un grupo por sede y `COUNT(*)` cuenta las filas de cada grupo. `HAVING` filtra los grupos resultantes; `WHERE` filtra filas antes de agrupar.

## Un detalle sobre NULL

`COUNT(*)` cuenta filas, mientras que `COUNT(columna)` cuenta los valores no nulos de esa columna. Si se agregan columnas que no son parte de una función de grupo, deben respetarse las reglas de agrupación del gestor.
