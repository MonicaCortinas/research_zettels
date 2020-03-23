---
tags: [methods, fsQCA, csQCA, settheoretic, set, Notebooks/QCA, Notebooks/methods]
title: 2003211713_Que es un set
created: '2020-03-22T17:13:00.275Z'
modified: '2020-03-22T17:13:00.275Z'
---

# Qué es un set

En el capítulo 1 del libro Set Theoretic Methods, @schneider2012_set se centran en la descripción de los sets y cómo se realiza la asignación de las puntuaciones de pertenencia a los sets, lo que se denomina calibración.

Citando a Mahoney (2010) hay dos maneras de mirar a los conceptos básicos que utilizamos en ciencias sociales:

- Como representaciones mentales de una propiedad empírica. En ese caso, cuando recogemos información sobre los casos estaríamos recogiendo unformación sobre la medida en la que tienen o no tienen dicha propiedad. Sería nuestra operacionalización en variables habitual.
- Como conjuntos que tienen unas determinadas fronteras de inclusión y exclusión. En este caso, para analizar los casos lo que hacemos es ver si pertenecen o no (o en qué grado) pertenecen al conjunto.

En la teoría de sets se utiliza la pertenencia a un set para definir si un caso puede ser descrito por un concepto o no.

## Dos tipos de sets: fuzzy y crisp

Los conjuntos crisp son un caso particular de los fuzzy que presentan las siguientes desventajas:

- perdemos información empíricia al hacer la dicotomización
- reducimos la robustez de los resultados al hacerlos depender del punto de corte

Sin embargo, en los set fuzzy, asumimos que las **fronteras conceptuales** no están claramente definidas. Es decir, se utiliza una puntuación fuzzy no porque haya incertidumbre sobre la medición, sino porque la asignación al conjunto no es sí/no.

Los sets fuzzy mantienen la ventaja de distinguir entre casos en sentido cualitativo y añadir la posibilidad de diferencia en grado.

Los sets fuzzy requieren en general la definición de los valores de full set membership (1), fll non-membership (0) e indiferencia (0.5), aunque asignar 0.5 en general debe omitirse. Esta escala **no debe asimilarse a una escala de probabilidad de pertenencia** ya que es una escala cualitativa en la que la diferencia entre **0.4 y 0.6** es fundamentalmente distinta a la diferencia entre **0.1 y 0.3**.

Hay un ejemplo muy interesante para distinguir esto:

> ¿Qué preferiríamos beber: una bebida con una probabilidad de ser venenosa de 0.01 o con una puntuación de pertenencia al set de bebidas venenosas de 0.01?

Sería mucho mejor el segundo caso, porque en el primero, 1 de cada 100 veces podríamos beber algo muy venenoso, mientras que en el segundo, bebemos con certeza un líquido que prácticamente no es peligroso (porque casi no pertenece al set de bebidas venenosas) pero podría llegar a serlo en algún caso (por ejemplo, una bebida energética).

## Notas relacionadas

- [Index](_2003101705_index.md)
- [Los métodos set theoretic](2003212003_set_theoretic_methods.md)
- [Qué es el QCA](2003212024_qca_descripcion.md)
- [Calibración](2003221733_calibracion_sets.md)
- [Operaciones booleanas](2003231138_operaciones_boleanas.md)

--

Referencias:

Schneider, C. Q., & Wagemann, C. (2012). Set-theoretic methods for the social sciences: A guide to qualitative comparative analysis (C. Elman, J. Gerring, & J. Mahoney, eds.). Cambrigde: Cambridge University Press.