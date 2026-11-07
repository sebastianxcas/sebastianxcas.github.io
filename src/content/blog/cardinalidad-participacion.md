---
title: 'Cardinalidad y participación'
description: 'Dos preguntas para describir cómo se relacionan las entidades.'
pubDate: 2026-11-07
author: Sebastián Castellanos Parra
tags: ['Modelado']
---

En un MER, la cardinalidad indica cuántas instancias pueden asociarse a través de una relación. La participación expresa si intervenir en esa relación es obligatorio o no.

## Un ejemplo

Si una sede tiene varias salas y cada sala pertenece a una sola sede, la relación es **uno a muchos** desde SEDE hacia SALA. Si toda sala debe pertenecer a una sede, su participación en esa relación es total. La participación de SEDE depende de si las reglas permiten registrar una sede sin salas.

En una relación muchos a muchos, una instancia de cada lado puede asociarse con varias del otro. Por ejemplo, una compra puede vincular clientes y funciones; el significado exacto depende del enunciado.

Conviene revisar mínimo y máximo por separado: **cuántas asociaciones se permiten** no responde por sí solo si alguna es obligatoria.
