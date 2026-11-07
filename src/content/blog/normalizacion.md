---
title: 'Normalización: identificar dependencias'
description: 'Una reflexión sobre los ejercicios de hospitalización y pedidos del taller.'
pubDate: 2026-11-06
author: Sebastián Castellanos Parra
tags: ['Normalización']
---

La normalización organiza los atributos en tablas para reducir problemas de redundancia. En el taller analizamos dependencias funcionales y anomalías de inserción, actualización y eliminación.

## Dos casos

En **hospitalización**, bajo los supuestos del ejercicio, se identificaron dependencias transitivas desde la cama hacia el ala y desde el médico hacia sus datos de contacto. En **pedido, cliente y producto**, la clave compuesta de cada línea permitió identificar dependencias parciales y transitivas.

La primera forma normal exige valores atómicos; la segunda aborda dependencias parciales de atributos no primos respecto de una clave candidata compuesta; la tercera, de forma resumida, aborda las dependencias transitivas problemáticas. Cada descomposición depende de las reglas y supuestos del caso.

## Aprendizaje

Separar los datos por sus dependencias facilita mantenerlos sin repetir información innecesariamente. En [evidencias](/work/#normalizacion) se encuentran el desarrollo paso a paso en Excel, las respuestas del grupo y los demás ejercicios.
