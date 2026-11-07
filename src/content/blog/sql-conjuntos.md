---
title: 'SQL: operadores de conjuntos'
description: 'Combinar resultados con UNION, INTERSECT y diferencia.'
pubDate: 2026-11-07
author: Sebastián Castellanos Parra
tags: ['SQL']
---

Los operadores de conjuntos combinan resultados de consultas compatibles. Las consultas deben producir el mismo número de columnas y tipos compatibles en las posiciones correspondientes.

```sql
SELECT ciudad FROM sede
UNION
SELECT ciudad FROM proveedor;
```

`UNION` combina resultados y elimina duplicados; `UNION ALL` los conserva. `INTERSECT` devuelve valores presentes en ambos resultados. La diferencia se escribe como `MINUS` en Oracle y como `EXCEPT` en otros gestores; la disponibilidad depende de la versión y del producto.

En el ejemplo, el resultado representa ciudades que aparecen en una u otra tabla. No identifica por sí solo si cada ciudad provino de una sede, de un proveedor o de ambos.
