---
title: 'Funciones de una fila y conversión'
description: 'Transformar valores y tratar tipos de datos en una consulta.'
pubDate: 2026-11-07
author: Sebastián Castellanos Parra
tags: ['SQL']
---

Las funciones de una fila se aplican a cada fila procesada y producen un resultado por fila. Pueden trabajar con texto, números, fechas u otros tipos, según el gestor.

## Ejemplos

```sql
SELECT UPPER(nombre) AS nombre_mayusculas
FROM cliente;
```

`UPPER` transforma el texto a mayúsculas en el resultado. Una función de conversión puede interpretar o presentar un valor en otro tipo; en Oracle, por ejemplo, `TO_CHAR` y `TO_DATE` usan formatos que deben indicarse con cuidado.

Conviene considerar los valores nulos y no asumir que una cadena tiene siempre el formato de fecha esperado. Es importante distinguir entre **mostrar** un valor con un formato y cambiar el tipo o el valor almacenado.
