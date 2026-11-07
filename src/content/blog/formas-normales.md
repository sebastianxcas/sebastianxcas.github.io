---
title: 'Primera, segunda y tercera forma normal'
description: 'Un recorrido por valores atómicos y dependencias.'
pubDate: 2026-11-07
author: Sebastián Castellanos Parra
tags: ['Relacional']
---

La normalización analiza cómo se distribuyen los atributos entre tablas para reducir redundancias y ciertas anomalías.

## Tres pasos de análisis

**1FN:** los atributos contienen valores atómicos para el dominio considerado; no se usan grupos repetidos como una lista de productos en una sola celda.

**2FN:** además de cumplir 1FN, ningún atributo no primo depende de una parte propia de una clave candidata compuesta. Si la clave es simple, no puede haber dependencia parcial respecto de ella.

**3FN:** para cada dependencia funcional no trivial `X → A`, X debe ser superclave o A debe ser un atributo primo. Como regla práctica, se revisan dependencias transitivas problemáticas de atributos no primos.

Descomponer requiere revisar que no se pierda información al reunir las tablas y que se conserven las restricciones necesarias. Los resultados dependen de las dependencias y supuestos del caso.
