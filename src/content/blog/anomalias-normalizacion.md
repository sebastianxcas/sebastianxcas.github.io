---
title: 'Las anomalías que ayuda a prevenir la normalización'
description: 'Ejemplos de inserción, actualización y eliminación.'
pubDate: 2026-11-07
author: Sebastián Castellanos Parra
tags: ['Relacional']
---

Si una tabla mezcla datos de pedidos, clientes y productos, es posible que el nombre de un cliente se repita muchas veces. Esa repetición puede causar problemas al mantener la información.

## Tres situaciones

- **Actualización:** si cambia el nombre de un cliente y solo se corrigen algunas filas, quedan valores contradictorios.
- **Inserción:** si una tabla exige datos de un pedido para cada fila, puede ser imposible registrar un producto nuevo antes de su primera venta.
- **Eliminación:** si se borra el último pedido de un cliente, podrían desaparecer también los únicos datos que se tenían de ese cliente.

Separar las entidades en tablas relacionadas ayuda a evitar estas anomalías cuando la descomposición respeta las dependencias del caso. La normalización no significa que nunca se repita una clave foránea: repetirla puede ser necesario para representar relaciones entre filas.
