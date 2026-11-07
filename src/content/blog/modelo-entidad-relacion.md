---
title: 'Del problema al modelo entidad–relación'
description: 'Entidades, atributos, cardinalidades y algunas decisiones de modelado.'
pubDate: 2026-11-06
author: Sebastián Castellanos Parra
tags: ['Modelado']
---

El modelo entidad–relación ayuda a representar la información de un problema antes de convertirla en tablas. Una **entidad** representa aquello sobre lo que se quiere guardar información; un **atributo** la describe y una **relación** conecta entidades.

## Atributos y cardinalidad

Un atributo puede ser simple, compuesto, multivaluado, derivado o formar parte de una clave. Por ejemplo, el nombre puede descomponerse en nombres y apellidos; una persona puede tener varios correos y la edad puede calcularse a partir de la fecha de nacimiento. En notación de Chen se usan, entre otras convenciones, el subrayado para claves, la elipse doble para atributos multivaluados y la elipse discontinua para derivados.

La cardinalidad expresa cuántas instancias pueden relacionarse: uno a uno, uno a muchos o muchos a muchos. La participación indica si la relación es obligatoria para una entidad.

## La práctica

En el ejercicio de clase se representan equipos, jugadores y partidos. También hay modelos de biblioteca y CineAndes entre las [evidencias](/work/#modelado). La idea principal es que los nombres, las claves y las relaciones deben reflejar las reglas del caso; un diagrama es una representación que se puede revisar y mejorar.
