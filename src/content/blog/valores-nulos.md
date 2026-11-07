---
title: 'Qué significa NULL en SQL'
description: 'Ausencia de un valor y comparaciones que requieren cuidado.'
pubDate: 2026-11-07
author: Sebastián Castellanos Parra
tags: ['SQL']
---

En SQL, `NULL` representa la ausencia de un valor conocido o aplicable. No equivale automáticamente a cero, a una cadena vacía ni a un valor específico.

## Cómo consultar valores ausentes

```sql
SELECT nombre
FROM cliente
WHERE correo IS NULL;
```

La condición `IS NULL` busca filas sin un valor de correo. Comparar con `= NULL` no funciona como una comparación ordinaria: SQL utiliza lógica de tres valores, que incluye verdadero, falso y desconocido.

Las funciones de agregación también requieren atención. `COUNT(*)` cuenta filas, mientras que `COUNT(correo)` cuenta los correos no nulos. La forma en que se muestran y manejan cadenas vacías puede variar entre gestores; por ejemplo, Oracle trata una cadena vacía de caracteres como NULL.
