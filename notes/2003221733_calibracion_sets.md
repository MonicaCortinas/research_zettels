---
tags: [methods, fsQCA, csQCA, settheoretic, calibration, Notebooks/QCA, Notebooks/methods]
title: 2003211733_Procedimiento de calibración
created: '2020-03-22T17:33:00.275Z'
modified: '2020-03-22T17:33:00.275Z'
---

# Procedimiento de calibración

El procedimiento de calibración consiste en asignar a los casos una puntuación de pertenencia a cada set.

Según @schneider2012_set, en el proceso de calibración se necesitan:

1. Una definición precisa de la población relevante de casos
2. Una definición precisa del significado de todos los conceptos (tanto las condiciones como el resultado)
3. Una decisión sobre dónde está el punto de máxima indiferencia
4. Una decisión sobre la pertenencia plena o la no pertenencia plena (que es lo mismo que pertenencia plena al conjunto opuesto, por ejemplo, pertenencia plena al conjunto de los insatisfechos)
5. Una decisión sobre cómo se gradúa la pertenencia entre estas 

En general, la calibración debe deberse a motivos externos, teóricos, de conocimiento de los datos, a nociones generalmente aceptadas y al conocimiento del investigador.

Todos los datos pueden recalibrarse en sets crisp, pero solo los continuos y los de intervalo pueden codificarse como fuzzy [@dusa2019_qca].

Podemos optar por una aproximación puramente cualitativa, como la de Emmenegger (2011) en la que se asignan directamente 4 valores a los casos (0, 0.33, 0.67, 1). A esto se le llama un método de **Asignación Directa** y no es muy recomendable [@dusa2019_qca, capítulo 4]

De manera más adecuada, podemos optar po un método de ajuste como los métodos **directo** e **indirecto** de Ragin (2008).

- Método directo: ajusta una función logística entre los valores de 1, 0.5 y 0 proporcionados por el investigador. También podemos usar una campana invertida si nuestro set es algo como "moderadamente rico" cuya puntuación de pertenencia desciende en los extremos.
- Método indirecto: primero se clasifican los casos manualmente en valores de 0.8, 0.6, 0.4 y 0.2 , después ajustamos un modelo econométrico para establecer los parámetros para esos niveles y luego se utilizan las predicciones como puntuaciones de pertenencia [@dusa2019_qca, capítulo 4].

Estos métodos no están tampoco exentos de crítica, porque dan una aproximación aparentemente cuantitativa que es en cierta medida arbitratia (e.g. porqué función logística).

En general, los tres métodos deberían llevar a conclusiones similares, salvo que los casos estén muy sesgados cerca de alguna de las fronteras.

## La calibración de variables cualitativas

Cuando Ragin (2008a, b) introduce el concepto de calibración se refiere la transformación de **variables de intervalo en sets fuzzy**.

Las variables cualitativas solo pueden ser transformadas en crisp binarios o multivalores.

Es más dudoso qué pasa cuando las variables son ordinales. Esto pasa especialmente con las variables de tipo likert, que son problemáticas por:

- son bipolares (completamente de acuerdo y completamente en desacuerdo) lo que va en contra de la naturaleza asimétrica de la teoría del test. Aquí hay una referencia de Emmenegger (2014) que estudia las actitudes hacia los inmigrantes y usan el 1,2 y 3 como fuera del set y el 4 y 5 dentro del set (definiendo un punto en el medio). *Revisar, puede ser útil*
- Además, las respuesta suelen estar sesgadas en uno de los polos y esto dificulta poder convertirlos en un multiset crisp. Si tienes más de 5 no tiene sentido hacer crisp

> En general, **transformar escalas de Likert** en fuzzy scores es altamente problemático incluso para la investigación cuantitativa y pretender que la investigación cualitativa va a hacer un mejor trabajo creando puntuaciones numéricas es altamente cuestionable. @dusa2019_qca, página 97.

Un posible método, si hay siete o más y si se distribuyen proporcionalmente entre categorías, es el de Cheli y Lemmi (1995), llamado **método TFR**. Cuando los datos son categóricos, incluso sesgados, se propone una normalización que aplica una transformación para crear una función de pertenecia.

## Notas relacionadas

- [Index](_2003101705_index.md)
- [Los métodos set theoretic](2003212003_set_theoretic_methods.md)
- [Qué es el QCA](2003212024_qca_descripcion.md)
- [Qué es un set](2003221713_setdefinition_qca.md)
- [Operaciones booleanas](2003231138_operaciones_boleanas.md)
- [Análisis de suficiencia](2003241628_analisissuficiencia_qca.md)
- [Análisis de necesidad](2003241901_condicionnecesidadqca.md)
- [Complejidad causal: INUS Y SUIN](2003250705_causalcomplexity.md)

--

Referencias:

Duşa, A. (2019). QCA with R: A comprehensive resource. In QCA with R: A Comprehensive Resource. https://doi.org/10.1007/9783319756684
Schneider, C. Q., & Wagemann, C. (2012). Set-theoretic methods for the social sciences: A guide to qualitative comparative analysis (C. Elman, J. Gerring, & J. Mahoney, eds.). Cambrigde: Cambridge University Press.