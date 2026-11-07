---
title: 'Atributos en un modelo entidad–relación'
description: 'Claves, valores compuestos, multivaluados y derivados.'
pubDate: 2026-11-07
author: Sebastián Castellanos Parra
tags: ['Modelado']
---

Los atributos describen propiedades de las entidades o de sus relaciones. Elegir cómo representarlos depende de las reglas del caso.

## Tipos frecuentes

Un atributo **simple** no se descompone en el modelo. Uno **compuesto** puede dividirse en partes con significado, como una dirección en ciudad y calle. Un atributo **multivaluado** admite varios valores para una entidad, como varios teléfonos. Uno **derivado** se obtiene de otros datos: la edad puede calcularse a partir de la fecha de nacimiento.

Un atributo clave, o una combinación de atributos, permite distinguir una entidad de las demás. En notación de Chen suelen usarse subrayado para la clave, elipse doble para el multivaluado y elipse discontinua para el derivado.

Al transformar a tablas, se representan las partes del compuesto; los multivaluados suelen pasar a una tabla propia y los derivados suelen calcularse cuando se necesitan. La decisión depende de las reglas y requisitos del sistema.
