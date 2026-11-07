---
title: 'El modelo relacional: tablas y claves'
description: 'Relaciones, tuplas, atributos, dominios e integridad.'
pubDate: 2026-11-07
author: Sebastián Castellanos Parra
tags: ['Relacional']
---

El modelo relacional organiza los datos en relaciones, representadas habitualmente como tablas. Una fila es una tupla y una columna corresponde a un atributo. El dominio establece los valores admitidos para un atributo.

## Cómo se identifican y conectan los datos

Una **clave candidata** identifica de manera única una fila y es mínima: si se le quita algún atributo deja de identificarla. Una de las candidatas puede elegirse como clave primaria. Una **clave foránea** referencia una clave de otra tabla —o de la misma— y ayuda a mantener la integridad referencial.

Por ejemplo, SALA puede tener la clave `(codigo_sede, numero_sala)` y `codigo_sede` puede referenciar SEDE. Así se puede repetir el número de sala en dos sedes distintas sin confundirlas.

La estructura de una relación es su esquema. El número de atributos es su grado y el número de filas en un momento dado es su cardinalidad. En [modelado](/work/#modelado) hay material visual sobre el tema.
