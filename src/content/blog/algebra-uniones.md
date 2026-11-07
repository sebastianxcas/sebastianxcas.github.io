---
title: 'Álgebra relacional: conjuntos y reuniones'
description: 'Unión, diferencia, producto cartesiano y join.'
pubDate: 2026-11-07
author: Sebastián Castellanos Parra
tags: ['Relacional']
---

Además de seleccionar filas y proyectar columnas, el álgebra relacional permite combinar relaciones.

## Conjuntos y combinaciones

La **unión** reúne las tuplas de dos relaciones compatibles; la **intersección** conserva las comunes y la **diferencia** conserva las de la primera que no estén en la segunda. Para esas operaciones las relaciones deben ser compatibles en grado y dominios correspondientes.

El **producto cartesiano** combina cada fila de una relación con cada fila de la otra. Una **reunión** o join combina las filas que satisfacen una condición; puede pensarse como un producto seguido de una selección, según el tipo de join.

Por ejemplo, unir SALA con SEDE por `codigo_sede` permite mostrar cada sala con datos de su sede. La condición de unión evita combinaciones que no representan una asociación válida.
