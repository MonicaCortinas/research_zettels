---
tags: [artificialintelligence, vapas, Notebooks/artificialintelligence, amazon, textualanalysis]
title: 2004280735_El uso de datos textuales para el estudio de los VAPAs
created: '2020-04-28T07:35:55.880Z'
modified: '2020-04-28T07:35:55.880Z'
---

# El uso de reviews para el estudio de los VAPAs


pradhan2018_accesibility utilizan datos de reviews de Amazon para estudiar el uso que hacen de estos asistentes las [personas con discapacidad](2004081204_uso_vapas_discapacidad.md). Realizan un análisis de contenido de las reviews de Alexa, seleccionando palabras relacionadas con la discapacidad. Para ello construyen un diccionario de términos especificados previamente (95 términos). Con esto seleccionan las reviees, evaluando la relevancia de una muestra aleatoria por dos revisores independientes (se reporta el índice kappa) y uno solo después codificó el resto y se quedan con una muestra de 346 reviews. El análisis se realiza con codificación manual del contenido para construir las nuevas variables.

@purington2017_alexa también usan reviews de Amazon para estudiar la [personificación de los VAPAs](2004060734_antropomorfismo_vapas.md). Para ello, también hacen un diccionario manual de personificación, identificando aquellas reviews que utilizan pronombres como "her" vs "it" y sociabilidad, de forma manual, al igual que en el caso de @pradhan2018_accesibility y las relacionan con los ratings. Codifican 587 reviews.

@nguyen2019_hey también utilizan reviews pero en este caso no se de Amazon, sino de **Bestbuy** para hacer un análisis de topic modeling usando un modelo de Lantent Dirichlet Allocation (LDA). En este caso, parten de 53.273 reviews. Recogen datos de Amazon (Echo, Echo Dot, Echo Spot), Google (Home, Home Mini, Home Max), Apple (HomePod) and Sonos (One, Beam). El resultado son 13 tópicos distintos que después unifican en ocho: precio, integración, calidad de sonido, fiabilidad, skills, diversión, facilidad de uso, poner música. Comparan el rendimiento por dispositivo, siendo mejor en los aspectos de sonido para Apple y Sonnos, pero mejor en skills y diversión para Google Home y Amazon Alexa.

## Notas relacionadas:

- [Index](_2003101705_index.md)
- [Textual Analysis](2003250920_textual_analysis.md)

-- 
References

- Nguyen, H., & Hovy, D. (2019). Hey Siri . Ok Google . Alexa : A topic modeling of user reviews for smart speakers. W-NUT Workshop, EMNLP.
- Pradhan, A., Mehta, K., & Findlater, L. (2018). “Accessibility came by accident”: Use of voice-controlled intelligent personal assistants by people with disabilities. Conference on Human Factors in Computing Systems - Proceedings, 2018-April, 1–13. https://doi.org/10.1145/3173574.3174033
- Purington, A., Taft, J. G., Sannon, S., Bazarova, N. N., & Taylor, S. H. (2017). “Alexa is my new BFF”: Social Roles, User Satisfaction, and Personification of the Amazon Echo. Proceedings of the 2017 CHI Conference Extended Abstracts on Human Factors in Computing Systems - CHI EA ’17, 2853–2859. https://doi.org/10.1145/3027063.3053246