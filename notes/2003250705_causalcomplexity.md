---
tags: [csQCA, fsQCA, methods, Notebooks/methods, Notebooks/QCA, settheoretic, causalcomplexity, INUS, SUIN]
title: 2003250705_Complejidad Causal en QCA. INUS y SUIN
created: '2020-03-25T07:05:00.275Z'
modified: '2020-03-25T07:05:07.962Z'
---

# Complejidad causal en QCA

El capítulo 3 del libro de @schneider2012_set explica cómo los métodos QCA son adecuados cuando existe complejidad causal, que implica que hay:

- Equifinalidad: implica que distintas combinaciones de condiciones pueden causar el resultado. 

> e.g. A*B + ~C → Y  AB  y ~C son equifinales

- Conjunctural causation: el efecto de una condición solo se revela cuando actua en combinación con otras.

> e.g. A*B + ~C → Y  A y B  causan conjuntamente Y

- Asimetría: las condiciones qie explican el outcome no necesariamente explican la negación del outcome. 

> e.g. A*B + ~C → Y   ~A~B + C no lleva a ~Y

Esta es una diferencia importante con los métodos de regresión y basados en correlaciones.

Dos tipos de combinaciones en estas condiciones son especialmente interesantes:

## Condiciones INUS

Es una parte insuficiente pero necesaria de una condición que es en sí misma, innecesaria pero suficiente para el resultado.

> A*B + ~C → Y A y B son condiciones INUS

## Condiciones SUIN

Es una parte suficiente pero no necesaria de un factor que es insuficiente pero necesario para el outcome. Se suele dar más en el análisis de necesidad.

> (A+B)*(C+~D) ← Y  A, B, C y ~D son condiciones SUIN

## Notas relacionadas

- [Index](_2003101705_index.md)
- [Los métodos set theoretic](2003212003_set_theoretic_methods.md)
- [Qué es el QCA](2003212024_qca_descripcion.md)
- [Qué es un set](2003221713_setdefinition_qca.md)
- [Cómo calibrar](2003221733_calibracion_sets.md)
- [Lógica booleana](2003231138_operaciones_boleanas.md)
- [Análisis de suficiencia](2003241628_analisissuficiencia_qca.md)
- [Tablas de la verdad](2003260827_qca_tabladelaverdad.md)
- [Minimización de la tabla de la verdad](2003261610_minimizacion_tabladelaverdad.md)
- [Consistencia de condiciones suficientes](2003280813_consistencia_qca.md)
- [Cobertura de condiciones suficientes](2003280911_covertura_solucionsuficiente.md)

--

Referencias:

Schneider, C. Q., & Wagemann, C. (2012). Set-theoretic methods for the social sciences: A guide to qualitative comparative analysis (C. Elman, J. Gerring, & J. Mahoney, eds.). Cambrigde: Cambridge University Press.