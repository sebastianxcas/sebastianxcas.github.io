---
title: 'Dependencias funcionales'
description: 'Qué significa que un conjunto de atributos determine otro.'
pubDate: 2026-11-07
author: Sebastián Castellanos Parra
tags: ['Relacional']
---

Una dependencia funcional `X → Y` expresa una regla: si dos filas coinciden en X, deben coincidir en Y. Se trata de una propiedad de los datos permitidos por el dominio del problema, no de una conclusión garantizada por una muestra pequeña.

## Un ejemplo

Si cada código de producto identifica un único nombre, entonces `codigo_producto → nombre_producto`. Ver dos códigos distintos con el mismo nombre no contradice esa dependencia; lo que la contradice es un mismo código con dos nombres distintos.

## Dependencias parciales y transitivas

Una dependencia parcial aparece cuando un atributo no primo depende de una parte propia de una clave candidata compuesta. Una dependencia transitiva problemática puede aparecer cuando la clave determina un atributo no clave a través de otro atributo no clave.

Estas dependencias ayudan a analizar normalización. Las conclusiones cambian si cambian las reglas: por eso los supuestos del [taller de hospitalización y pedidos](/work/#normalizacion) importan.
