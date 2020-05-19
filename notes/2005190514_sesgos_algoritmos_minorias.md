---
tags: [artificialintelligence, algorithm, bias, Notebooks/artificialintelligence, minorías]
title: 2005190515_Los sesgos de los algoritmos dependen del tamaño de los datos, efectos en los anuncios Google
created: '2020-05-15T05:27:55.880Z'
modified: '2020-05-15T05:27:55.880Z'
---

# Los sesgos de los algoritmos dependen del tamaño de los datos, efectos en los anuncios Google

@lambrecht2020_apparent en un trabajo en curso que está publicado en SSRN y que se presentó en un seminario online de EMAC analizan los conocidos sesgos de los algoritmos que pueden discriminar a distintos grupos como grupos étnicos, religiosos, por género, etc...

En este caso se centran en un sesgo muy conocido, el que asocia la búsqueda de nombres típicamente asociados a personas negras con anuncios de búsqueda de antecedentes. Este es un trabajo académico de Sweeney (2013) que ha recibido mucha atención también en la prensa especializada. En el trabajo original, solo se muestra el sesgo, sin incidir en las posibles fuentes de este.

En este trabajo, @lambrecht2020_apparent establecen una campaña más neutra (anuncios de trabajo) con anuncios en Google destinados a distintos nombres "blancos" y "negros" (865 en total) para comprobar:

- si efectivamente se reproduce el sesgo, con diferencias de aparición entre los distintos nombres
- el origen de estas diferencias

Lo que se observa es que el anuncio se detecta rápidamente como poco relevante para los nombres blancos, que tienen muchas búsquedas y rápidamente dejan de aparecer. Sin embargo, los nombres negros tienen frecuencias menores y, aunque el anuncio sea malo, se les presenta con más frecuencia. El algoritmo actualiza menos la información.

El análisis se repite con grupos religiosos, obteniendo lo mismo, los grupos más minoritarios están más expuestos al anuncio aunque sea muy malo (en el sentido de que tiene un click-through rate muy bajo).

## Notas relacionadas


- [Index](_2003101705_index.md)
- [El funcionamiento de la publicidad SEM en Google](005190530_elalgoritmoanunciones_google.md)
- [Aceptación del consejo de los algoritmos](2004060917_aceptacion_consejo_algoritmos.md)
- [Atención a los anuncios en Facebook según el nivel de amistad](2004180843_atencion_anuncios_facebook_segunamistad.md)
- [Adecuación del algoritmo según tarea: Análisis con anuncios en Facebook](2004271035_algorithm_type_task.md)

--
References

Lambrecht, A., & Tucker, C. E. (2020). Apparent Algorithmic Bias and Algorithmic Learning. SSRN Electronic Journal. https://doi.org/10.2139/ssrn.3570076

