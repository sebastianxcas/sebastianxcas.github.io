---
title: 'Álgebra relacional: seleccionar y proyectar'
description: 'Operaciones para expresar consultas sobre relaciones.'
pubDate: 2026-11-07
author: Sebastián Castellanos Parra
tags: ['Relacional']
---

El álgebra relacional es un lenguaje formal de operaciones sobre relaciones. Cada operación produce una relación que puede usarse como entrada de otra.

## Selección y proyección

La **selección**, representada por `σ`, filtra filas que cumplen una condición. Por ejemplo, `σ ciudad = 'Bogotá' (SEDE)` conserva las sedes de esa ciudad.

La **proyección**, representada por `π`, conserva los atributos indicados. `π nombre, ciudad (SEDE)` obtiene esos atributos de la relación. En el álgebra relacional de conjuntos se eliminan duplicados; SQL puede conservarlos salvo que se use `DISTINCT`.

Se pueden combinar operaciones: primero seleccionar sedes de Bogotá y después proyectar sus nombres. La expresión muestra qué se quiere obtener sin depender directamente de un gestor.
