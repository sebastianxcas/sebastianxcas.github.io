---
title: 'Del modelo conceptual al físico'
description: 'Cómo se relacionan el MER, el modelo relacional y la implementación.'
pubDate: 2026-11-07
author: Sebastián Castellanos Parra
tags: ['Fundamentos']
---

Diseñar una base de datos implica tomar decisiones en distintos niveles. Cada uno responde una pregunta diferente y sirve para revisar el diseño antes de pasar al siguiente.

## Tres miradas

- **Conceptual:** representa las entidades, atributos y relaciones relevantes para el problema. Un diagrama entidad–relación ayuda a comunicarlo.
- **Lógica:** organiza esa información en relaciones o tablas e identifica claves y restricciones, sin depender necesariamente de un gestor concreto.
- **Física:** considera la implementación en un SGBD: tipos de datos, índices, almacenamiento y otras decisiones propias del sistema.

Un modelo conceptual de biblioteca puede incluir LIBRO y AUTOR; el diseño lógico puede llevarlos a tablas y representar su relación; la implementación define finalmente las sentencias y tipos que usará el gestor.

La transformación debe conservar las reglas importantes del problema. Ver [los modelos y el taller](/work/#modelado) ayuda a seguir ese recorrido.
