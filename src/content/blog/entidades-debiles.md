---
title: 'Entidades débiles y claves parciales'
description: 'Cómo se identifica una entidad que depende de otra.'
pubDate: 2026-11-07
author: Sebastián Castellanos Parra
tags: ['Modelado']
---

Una entidad débil necesita la identificación de una entidad propietaria junto con su propia clave parcial para distinguir cada instancia. Su identificación depende de una relación identificadora.

## Ejemplo de CineAndes

El número de una sala puede repetirse en sedes distintas. Por eso, si el número solo es único dentro de su sede, una clave para SALA combina el código de la sede con el número de sala.

Una silla se distingue por fila y número dentro de una sala. Para identificarla globalmente también necesita la clave completa de la sala: código de sede, número de sala, fila y número de silla.

La clave parcial por sí sola no basta fuera del contexto de la propietaria. En las [evidencias](/work/#proyecto) está el diagrama del caso.
