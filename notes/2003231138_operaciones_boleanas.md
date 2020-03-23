---
tags: [methods, fsQCA, csQCA, settheoretic, operations, Notebooks/QCA, Notebooks/methods]
title: 2003231139_Operaciones booleanas
created: '2020-03-23T11:39:00.275Z'
modified: '2020-03-23T11:39:00.275Z'
---

# Operaciones básicas en teoría de sets.

El capítulo 3 del libro de @schneider2012_set recoge cómo se opera con los conjuntos de sets, que se puede describir desde tres teorías matemáticas:

- la teoría de la lógica de las proposiciones
- el álgebra booleana
- la teoría de set

Las tres aproximaciones tienen distinta nomenclatura, pero las operaciones básicas son las mismas:

- AND
- OR
- NOT
- Inclusion

Estas operaciones nos sirven para combinar los sets en otros conjuntos nuevos de manera que podamos generar otros nuevos sets.
Estos nuevos sets combinados son los que nos sirven para establecer relaciones entre:
    - Condiciones
    - Resultado

Las condiciones se expresan como un nuevo set expresado en términos de estos operadores.

La notación es muy variada pero básicamente quiere decir lo mismo:

|Operador  | Lógica          | Álgebra Booleana      | Teoría de set    |
|----------|-----------------|-----------------------|------------------|
| AND      |Conjunción ∧     | Multiplicación * , (.)| Intersección ∩   |
| OR       |Disjunción ∨     | Suma +                | Union  ∪         |
| NOT      |Complement ~ , ¬ | Negación 1-D          | Conjunto negado  |
|Inclusión |If-then → , ⇒    |                      | Subconjunto ⊂    |

Los cálculos son más sencillos de lo que parece:

- AND: en crisp es 1 si todos son 1, 0 en caso contrario. En fuzzy es el valor **mínimo**
- OR: en crisp es 1 si cualquiera de ellos es 1, 0 en caso contrario. EN fuzzy es el valor **máximo**. No confundir que XOR que exige que solo uno sea 1 y que no se usa en set theory
- NOT : en crisp y en fuzzy es 1- valor

Para agregar operaciones, es necesario tener en cuenta las propiedades de estos operadores: conmutativa, asociativa, distributiva y la ley de DeMorgan para invertir las operaciones.


## Notas relacionadas

- [Index](_2003101705_index.md)
- [Los métodos set theoretic](2003212003_set_theoretic_methods.md)
- [Qué es el QCA](2003212024_qca_descripcion.md)
- [Qué es un set](2003221713_setdefinition_qca.md)
- [Cómo calibrar](2003221733_calibracion_sets.md)

--

Referencias:

Schneider, C. Q., & Wagemann, C. (2012). Set-theoretic methods for the social sciences: A guide to qualitative comparative analysis (C. Elman, J. Gerring, & J. Mahoney, eds.). Cambrigde: Cambridge University Press.




