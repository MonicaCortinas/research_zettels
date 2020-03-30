---
tags: [csQCA, fsQCA, methods, Notebooks/methods, Notebooks/QCA, settheoretic, truthtable]
title: 2003261610_Minimización de las Tablas de la verdad en QCA
created: '2020-03-26T16:27:00.275Z'
modified: '2020-03-26T16:27:07.962Z'
---

# Cómo minimizamos las tablas de la verdad

La minimización de la [tabla de la verdad](2003260827_qca_tabladelaverdad.md) se hace siguiendo las reglas del algoritmo de Quine-McCluskey para las filas de la tabla de la verdad que conducen al outcome [@schneider2012_set].

Por ejemplo, suponiendo la siguiente tabla de la verdad:

| A | B | C | Y |
|---|---|---|---|
| 0 | 0 | 0 | 1 |
| 0 | 0 | 1 | 1 |
| 0 | 1 | 0 | 1 |
| 0 | 1 | 1 | 1 |
| 1 | 0 | 0 | 0 |
| 1 | 0 | 1 | 1 |
| 1 | 1 | 0 | 0 |
| 1 | 1 | 1 | 0 |

Las filas relevantes serían la 1, 2, 3, 4 y la 6. Se podría escribir como:

~A~B~C + ~A~BC+ ~AB~C + ~ABC + A~BC →  Y

Ahora comenzamos la simplificación eliminando las redundantes, por ejemplo si un dos términos aparece un set y su negación y lo demás es igual podemos eliminarlo como pasa en  ~A~BC y A~BC que se queda como ~A~B:
 
~A~B + ~AB~C +~ABC + A~BC →  Y

Ahora observamos que también podemos simplificar ~AB~C +~ABC

~A~B + ~AB + A~BC →  Y

Y de aquí vemos que podemos simplificar la B:

~A + A~BC →  Y

También podríamos eliminar la A del segundo término si no nos hace falta la interpretación, dado que como está negada en el primer término, es redundante en el segundo:

~A + BC →  Y

Estos son los implicantes principales (~A y BC) para el outcome.

A veces podemos simplificar implicantes principales redundantes más allá del algoritmo por razones no obvias y soluciones que son equivalentes, por lo que la selección de una u otra dependenderá de la lógica de la teoría.

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
- [Tablas de la verdad](2003261610_minimizacion_tabladelaverdad.md)
- [Consistencia de condiciones suficientes](2003280813_consistencia_qca.md)
- [Cobertura de condiciones suficientes](2003280911_cobertura_solucionsuficiente.md)
- [Diversidad limitada y recordatorios lógicos](2003300812_diversidad_limitada_qca.md)

--

Referencias:

Schneider, C. Q., & Wagemann, C. (2012). Set-theoretic methods for the social sciences: A guide to qualitative comparative analysis (C. Elman, J. Gerring, & J. Mahoney, eds.). Cambrigde: Cambridge University Press.