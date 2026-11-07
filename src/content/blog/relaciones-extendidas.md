---
title: 'Especialización, relaciones ternarias y agregación'
description: 'Tres herramientas del modelo entidad–relación extendido.'
pubDate: 2026-11-07
author: Sebastián Castellanos Parra
tags: ['Modelado']
---

El modelo entidad–relación extendido permite describir reglas que van más allá de asociaciones binarias simples.

## Especialización

Una superentidad puede tener subtipos con características propias. La especialización es **total** si toda instancia de la superentidad pertenece al menos a un subtipo, y **disjunta** si no puede pertenecer a varios a la vez. Totalidad y exclusividad son preguntas distintas.

## Relación ternaria

Una relación ternaria conecta tres entidades en un mismo hecho. En una entrega de proveedor, producto y sede, la cantidad corresponde a esa combinación. Tres relaciones binarias no conservan automáticamente qué tres participantes forman cada entrega.

## Agregación

La agregación permite tratar una relación y sus participantes como una unidad para asociarla con otro elemento. En CineAndes, el medio de pago corresponde a una compra concreta, es decir, a la asociación entre cliente y función.
