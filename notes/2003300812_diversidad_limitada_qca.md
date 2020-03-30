---
tags: [csQCA, fsQCA, methods, Notebooks/methods, Notebooks/QCA, limitediversity, logicalreminders, intermediatesolution]
title: 2003300812_Diversidad limitada en QCA
created: '2020-03-30T08:13:00.275Z'
modified: '2020-03-30T08:13:07.962Z'
---

# Los tipos y efectos de diversidad limitada en QCA

El concepto de diversidad limitada se refiere a la ausencia de evidencia empírica para ciertas combinaciones de las condiciones.

Esta ausencia de evidencia empírica se refleja en lo que se llaman "recordatorios lógicos":

> Los recordatorios lógicos (logical reminders) son filas de la tabla de la verdad que carecen de evidencia empírica para someterese a un test de suficiencia. (@schneider2012_set página 152)

El número de casos para ser considerados suficientes depende de la muestra. Si hay pocos casos (entre 10 y 100) un caso puede ser suficiente, pero en muestras mayores podemos considerar un porcentaje.

Podemos distinguir tres fuentes de diversidad limitada:

- Recordatorios aritméticos: tienen que ver con el tamaño de la muestra. Si tenemos 25 casos y 32 combinaciones de las condiciones, va a haber combinaciones no presentes.
- Recordatorios agrupados: en ciencias sociales pasa muchas veces que hay combinaciones improbables históricamente y que no se suelen dar, por ejemplo, países con sindicatos fuertes en los que no exista un partido de izquierdas. Que no existan esas combinaciones en la práctica no significa que no sean teóricamente posibles.
- Recordatorios imposibles: son aquellas combinaciones que no podrían darse nunca, por ejemplo si X1 = mujer, X2 = embarazo, no podríamos tener ~X1*X2 hombres embarazados.

La diversidad limitada no tiene nada que ver con los valores missing (que solo afectan a alguna variable, mientras que esto afecta a los casos) o los grados de libertad (podemos recoger una muestra enorme, pero no encontraremos casos de hombres embarazados). La diversidad limitada afecta a todas las técnicas, pero como no están tan basadas en la interacción entre variables no se les presta tanta atención.

## El procedimiento de análisis estandarizado para lidiar con la diversidad limitada.

La cuestión relevante es que para minimizar la tabla de la verdad, necesitaríamos tener todas las filas, para poder quitar o combinar términos. Pero si tenemos diversidad limitada, hay algunas filas que no sabemos qué es lo que hacer con ellas.

Tenemos dos opciones extremas, que no contradicen la evidencia empírica (son supuestos):

- Considerar que ninguna de ellas hubiera llevado al outcome. Esta es la solución más conservadora, porque implica que ninguna de esas configuraciones son suficientes y, por tanto, **no se incluyen en la solución y no se utilizan para simplificar los términos**. Como esta solución normalmente implica menos simplificación, se denomina **solución "compleja" o "también conservadora"**.

- Considerar que todos ellos potencialmente podrían conducir al outcome y, por tanto, todos esos términos son términos potencialmente suficientes. Estos términos se incluyen en la solución y se utilizan en la simplificación, de manera que esta es la **solución más parsimoniosa**.

Sin embargo, en esta solución más parsimoniosa, podemos estar incluyendo términos que son recordatorios imposibles o implausibles.

Una solución es hacer el **Standard Analysis** de Ragin, que proporciona una **solución intermedia** entre ambos.

El Standard Analysis parte de la solución conservadora y recoge los **supuestos simplificadores** para eliminar términos, sin necesidad de incluir como suficientes todas las combinaciones ausentes. Se pueden incluir manualmente aquellos que apoye la teoría, los denominados "easy counterfactuals".

En general, se usa la comparación de la solución conservadora y la solución parsimoniosa de manera que se llega a la solución intermedia de dos formas:

- Se pueden quitar aquellas condiciones de suficiencia de la solución conservadora que no aparecen en la solución más parsimoniosa y que son consistentes con las expectativas direccionales. 
- Se pueden analizar los supuestos simplificadores de la solución más parsimoniosa y aceptar solo aquellos que consideramos "easy counterfactuals".

Ambas estrategias llevarían a la misma solución intermedia.

La solución intermedia es un superset de la solución compleja y un subset de la solución más parsimoniosa


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
- [Minimización de las tablas de la verdad](2003261610_minimizacion_tabladelaverdad.md)
- [Consistencia de condiciones suficientes](2003280813_consistencia_qca.md)
- [Cobertura de condiciones suficientes](2003280911_cobertura_solucionsuficiente.md)
- [Suficiencia y cobertura de condiciones necesarias](2003290828_consistencia_cobertura_condiciones_necesarias.md)

--

Referencias:

Schneider, C. Q., & Wagemann, C. (2012). Set-theoretic methods for the social sciences: A guide to qualitative comparative analysis (C. Elman, J. Gerring, & J. Mahoney, eds.). Cambrigde: Cambridge University Press.