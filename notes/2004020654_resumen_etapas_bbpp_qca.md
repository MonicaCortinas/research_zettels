---
tags: [csQCA, fsQCA, methods, Notebooks/methods, Notebooks/QCA, goodpractices]
title: 20004020637_Resumen etapas y buenas prácticas QCA
created: '2020-04-02T06:37:00.275Z'
modified: '2020-04-02T06:37:07.962Z'
---

# Resumen de etapas y buenas prácticas QCA

El capítulo 11 del libro de @schneider2012_set hace un buen resumen de todas las etapas necesarias en QCA y sus respectivas buenas prácticas.

1. Se ha comprobado que un método set-theoretic es adecuado al problema: es decir, las condiciones bajo estudio pueden ser representadas como sets y tienen relaciones causales complejas entre ellas. Dicho de otra forma, podemos afirmar que el outcome está basado en unas relaciones equifinales, conjuntas y asimétricas en términos de condiciones necesarias, suficientes, INUS y o SUIN.

2. Se ha elegido unas condiciones razonables. El número debe ser moderado, ya que si no, encontramos problemas severos de diversidad limitadas y la solución suele ser demasiado compleja o demasiado basada en supuestos sobre los recordatorios lógicos. Si tenemos demasiadas condiciones, podemos crear constructos de orden superior para agruparlas (Ragin 2000, 321-328)

3. La elección de la variante QCA: en general se prefiere el fuzzy al crisp, porque es más preciso. Además, se pueden integrar condiciones crips (que no outcome) en un análisis fuzzy, pero a la inversa no es posible.

4. Calibración de las puntuaciones de pertenencia: este procedimiento debe discutirse y documentarse en detalle. Se necesitan conocimientos teóricos para decidir dónde colocar las anclas: 0, 0.5 y 1. También se puede utilizar la evidencia empírica y los [métodos directos e indirectos de Ragin](2003221733_calibracion_sets.md)

5. Análisis de condiciones necesarias: siempre debe hacerse de forma separada y precediendo al análisis de suficiencia. Los valores de consistencia en condiciones necesarias **deben ser superiores** a los de las condiciones sufciientes y se recomienda un umbral de 0.9 o incluso mayor. Solo deben declararse necesarias aquellas variables que pasen el test de relevancia (cobertura) y que no sean, por tanto, trivialmente necesarias. Si una condición se declara necesaria porque es consistente y relevante, cuando hacemos la minimización de la tabla de la verdad debemos evitar supuestos incoherentes con esta condición (aplicando el Enhanced Standard Analysis).

6. Análisis de condiciones suficientes: Se construye la tabla de la verdad y se decide qué rows son un recordatorio lógico y, si no lo son, si pueden considerarse condición suficiente para el outcome, en base al número de casos en cada fila y a su valor de consistencia. Los valores de consistencia raw no tienen un umbral determinado. Deben comprobarse los casos que son [contradicciones lógicas](2003280813_consistencia_qca.md) (consultar también [esta entrada](2003311642_resumen_algoritmo_tabla_verdad.md)), para evitar incluirlos. En general, se recomiendan valores de consistencia bastante por encima de 0.75 y con pocas contradicciones lógicas.

7. Recordatorios lógicos y la elección de los términos de solución: el tratamiento que se ha hecho de los recordatorios lógicos debe ser transparente, porque es muy importante para los resultados. Se deben eliminar los supuestos que no sean admisibles y también la dirección esperada de las relaciones. Debemos reportar las tres soluciones: conservadora, intermedia y parsimoniosa y centrar la discusión en la intermedia.

8. Análisis del resultado negativo. El análisis del resultado negado no es simétrico, por lo que si queremos obtener conclusiones al respecto tenemos que hacer todo el análisis de condiciones necesarias y suficientes desde el principio.

9. Presentación de resultados: Podemos usar tablas y gráficos, especialmente diagramas de Venn y XY plots.Todo trabajo publicado con QCA **debe incluir al menos la tabla de la verdad y la pertenecia de cada caso a los single sets y al outcome**. Además, para cada path y para la solución completa, se debe incluir consistencia y cobertura, los casos únicos cubiertos y los casos que son contradicciones lógicas y para la solución completa, aquellos casos que no cubrimos y que están más dentro que fuera del outcome. Normalmente utilizamos más de una forma de presentación para presentar:
- condiciones que explican el outcome
- qué casos (y cuales no) cubre la solución
- cómo de bien la solución se ajusta a la evidencia empírica

10. Interpretación de resultados: El potencial de QCA es cualitativo, por lo que debemos centrarnos en los casos individuales y no solo en los datos agregados totales. También debemos analizar la solución parte por parte. Aquí es importante la reiteración del ciclo de investigación, porque esta interpretación nos puede llevar a cambiar la pertenencia a los sets, las condiciones...

11. Test de robustez: presentación de resultados alternativos cuando se cambia el proceso de calibración, la elección del nivel de consistencia para la tabla de la verdad y las opciones de añadir o quitar casos individuales. Hay dos dimensiones de robustez: la solidez de las fórmulas relacionales y los valores de ajuste del modelo.

Además, en este capítulo se incluyen algunas cuestiones sobre el software. Las alternativas son:
- fsQCA 3.0: es el de Ragin y Davey
- Tosmana: https://www.tosmana.net/ es menos potente pero hace gráficos de Venn
- Stata
- R: hay distintos paquetes el recomendado es QCA de Dusa y Thiem, aunque hay también QCAGui y QCA3. Ahora QCA va por la versiçón 3.7 actualizada en marzo de este año.

 ## Notas relacionadas

- [Index](_2003101705_index.md)
- [Los métodos set theoretic](2003212003_set_theoretic_methods.md)
- [Qué es el QCA](2003212024_qca_descripcion.md)
- [Aplicaciones en marketing de QCA](2005091837_aplicaciones_marketingQCA.md)
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
- [Diversidad limitada](2003300812_diversidad_limitada_qca.md)
- [Problemas potenciales en QCA](2004020637_problemas_potenciales_QCA_extensiones.md)


--

Referencias:

Schneider, C. Q., & Wagemann, C. (2012). Set-theoretic methods for the social sciences: A guide to qualitative comparative analysis (C. Elman, J. Gerring, & J. Mahoney, eds.). Cambrigde: Cambridge University Press.


