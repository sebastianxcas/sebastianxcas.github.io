---
title: 'Claves e integridad en una base de datos'
description: 'Cómo ayudan las restricciones a mantener coherencia entre tablas.'
pubDate: 2026-11-07
author: Sebastián Castellanos Parra
tags: ['Relacional']
---

Las claves y restricciones convierten algunas reglas del diseño en condiciones que los datos deben cumplir. Son una parte esencial de la integridad de una base de datos.

## Claves y relaciones

Una clave primaria identifica cada fila: sus valores no se repiten y ninguno de sus componentes puede ser nulo. Puede estar formada por uno o varios atributos. Una clave foránea, en cambio, referencia una clave en otra relación —o en la misma— para representar una asociación.

Por ejemplo, una sala puede referenciar la sede a la que pertenece. Si esa asociación es obligatoria, la columna correspondiente debe impedir nulos además de tener la restricción de clave foránea.

## Restricciones adicionales

`UNIQUE`, `NOT NULL` y `CHECK` permiten expresar otras reglas, sujetas a las características del gestor. Sin embargo, no todas las reglas de negocio se pueden representar con una sola restricción: algunas requieren validaciones adicionales. Una base bien diseñada combina claves, restricciones y decisiones que responden al caso.
