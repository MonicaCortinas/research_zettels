---
tags: [csQCA, fsQCA, methods, Notebooks/methods, Notebooks/QCA, settheoretic, truthtable]
title: 2003260727_Tablas de la verdad en QCA
created: '2020-03-26T07:27:00.275Z'
modified: '2020-03-26T07:27:07.962Z'
---

# Las tablas de la verdad

Las tablas de la verdad son una herramienta básica de QCA y se describen en el capítulo 4 de @schneider2012_set.

Las tablas de la verdad son importantes para el análisis de **suficiencia**, no para la **necesidad**, porque para las condiciones necesarias el análisis se hace de una en una y no tiene sentido hacer combinaciones, ya que una combinación AB no puede ser necesaria si no lo son A y B.

La tabla de la verdad se construye con todas las combinaciones teóricas de las condiciones y los resultados (2^k). Después se comprueba qué casos caen en cada una de las filas, en el caso de **crisp**.

En el caso de **fuzzy**, la asignación es más compleja pero se hace comprobando la puntuación de cada caso a todas las combinaciones posibles mediante AND y asignando a aquella en la que la puntuación sea mayor que 0.5 (solo puede ser una, a no ser qué la puntuación en alguna de ellas sea 0.5 y, por tanto, no podemos asignar el caso).

Ejemplo con 3 condiciones, 8 combinaciones 2^3: Se comprueban las combinaciones AND con la regla del MÍNIMO:

| A | B | C | Y | ABC   | AB~C  | A~BC  | A~B~C | ~ABC  |~AB~C  |~A~BC  |~A~B~C |
|---|---|---|---|-------|-------|-------|-------|-------|-------|-------|-------|
|0.9|0.3|0.1|0.7|  0.1  |   0.3 |  0.1  |  0.7  |  0.1  |  0.1  |  0.1  |  0.1  |

La combinación a la que se asigna el caso es **A~B~C** como podríamos pensar intuitivamente.


## Notas relacionadas

- [Index](_2003101705_index.md)
- [Los métodos set theoretic](2003212003_set_theoretic_methods.md)
- [Qué es el QCA](2003212024_qca_descripcion.md)
- [Qué es un set](2003221713_setdefinition_qca.md)
- [Cómo calibrar](2003221733_calibracion_sets.md)
- [Lógica booleana](2003231138_operaciones_boleanas.md)
- [Análisis de necesidad](2003241901_condicionnecesidadqca.md)
- [Análisis de suficiencia](2003241628_analisissuficiencia_qca.md)
- [Complejidad causal: INUS Y SUIN](2003250705_causalcomplexity.md)
- [Minimización de la tabla de la verdad](2003261610_minimizacion_tabladelaverdad.md)

--

Referencias:

Schneider, C. Q., & Wagemann, C. (2012). Set-theoretic methods for the social sciences: A guide to qualitative comparative analysis (C. Elman, J. Gerring, & J. Mahoney, eds.). Cambrigde: Cambridge University Press.