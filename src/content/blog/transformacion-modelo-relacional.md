---
title: 'Del MER a las tablas'
description: 'Reglas de transformación aplicadas en el taller de la terminal portuaria.'
pubDate: 2026-11-06
author: Sebastián Castellanos Parra
tags: ['Modelado', 'Modelo relacional']
---

En el taller de la terminal portuaria Bahía Verde trabajamos en grupo las reglas para transformar un modelo entidad–relación. El documento desarrolla atributos compuestos, multivaluados y derivados; relaciones de muchos a muchos; relaciones ternarias y agregación.

## Qué cambia al transformar

Los componentes de un atributo compuesto pasan a representarse por separado. Un atributo multivaluado puede requerir una tabla propia; un valor derivado como la edad normalmente se calcula a partir de su dato de origen. En una relación muchos a muchos se crea una tabla que contiene las claves de las entidades relacionadas y los atributos de esa relación.

Una entidad débil necesita la clave de su propietaria junto con su identificador parcial. Si la propietaria también es débil, su clave completa debe acompañarla. Esto se observa en el caso de las recaladas y los embarques del taller.

## Aprendizaje

Transformar un modelo no consiste solo en cambiar dibujos por nombres de tablas: cada clave debe conservar la identificación y cada relación debe respetar las reglas del caso. El [taller y la solución guiada](/work/#modelado) están disponibles en evidencias.
