---
title: 'SQL: subconsultas'
description: 'Una consulta dentro de otra para expresar una condición.'
pubDate: 2026-11-07
author: Sebastián Castellanos Parra
tags: ['SQL']
---

Una subconsulta es una consulta anidada dentro de otra sentencia. Puede aportar un valor o un conjunto de valores para una condición.

```sql
SELECT titulo
FROM pelicula
WHERE codigo_pelicula IN (
  SELECT codigo_pelicula
  FROM funcion
);
```

Este ejemplo hipotético busca títulos cuyos códigos aparecen en la tabla FUNCION. `IN` compara con un conjunto; una subconsulta escalar, en cambio, debe producir como máximo un valor cuando se usa donde se espera uno solo.

Una subconsulta correlacionada depende de valores de la consulta exterior. Antes de elegir entre subconsulta y join hay que comprender la pregunta, las posibles duplicaciones y los nulos; el rendimiento concreto depende del gestor y su plan de ejecución.
