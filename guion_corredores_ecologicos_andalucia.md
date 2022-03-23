# Guión de la práctica "caracterización de la conectividad de los espacios de  la Red Natura 2000 en Andalucía"


> + **_Versión_**: 2021-2022
> + **_Asignatura (grado)_**: Ecología (CCAA)
> + **_Autor_**: Curro Bonet-García (fjbonet@uco.es)
> + **Duración**: 3 horas



## Objetivos

Este ejercicio tiene los siguientes objetivos instrumentales y disciplinares:

 + Instrumentales: Se refiere al conjunto de habilidades o conocimientos genéricos que se espera que adquieran o entrenen los estudiantes durante el desarollo de esta actividad.
   +    Familiarizarse con el concepto de flujo de trabajo como herramienta básica para planificar los procedimientos de análisis de datos.
   +    Profundizar en los conocimientos adquiridos sobre biogeografía de islas y conectividad de espacios naturales protegidos.
   +    Mejorar la destreza de los estudiantes en el manejo de SIG.
   +    Evocar el conocimiento previamente adquirido sobre técnicas de integración de información ambiental espacializada.
   +    Transferir el conocimiento adquirido en un ejemplo concreto (competencia intraespecífica) a otro diferente (corredores ecológicos)
 + Disciplinares: Se trata de objetivos relacionados con competencias propios de la ecología. 
    +    Adquirir información sobre cómo se distribuye la biodiversidad en Andalucía.
    +    Adquirir información sobre la distribución y tamaño de los espacios naturales protegidos de Andalucía.
    +    Adquirir información sobre la distribución de las infraestructuras humanas (cultivos, carreteras, núcleos urbanos) de Andalucía.
    +    Reflexionar sobre cómo se relacionan las infraestructuras "naturales" y las humanas bajo el hilo argumental de la biogeografía de islas y la gestión de espacios naturales protegidos.
    +    Analizar en qué medida los espacios protegidos se comportan como islas de biodiversidad en medio de una matriz ocupada por cultivos e infraestructuras.

Antes de detallar en qué consiste el ejercicio, lee el siguiente apartado en el que se describe el contexto ecológico planteado.



## Contextualización ecológica

Esta práctica se sustenta en la teoría de la biogeografía de islas. Lamentablemente impartimos la práctica antes de ver los contenidos teóricos. Así que, en este apartado resumimos las ideas principales de la biogeografía de islas que necesitamos para hacer la práctica. 



Supongamos un punto de partida teórico e irreal para esta práctica: nuestra zona de estudio, Andalucía, no está ocupada por humanos. Solo hay naturaleza. La siguiente imagen muestra cómo podría ser esta situación: bosques densos en mitad del valle del Guadalquivir y ausencia de infraestructuras humanas.







## Diseño de corredores ecológicos en Andalucía



Andalucía cuenta con una amplia red de espacios naturales protegidos. No en vano, es considerada como un punto caliente de biodiversidad en la región Mediterránea. Cuenta con una gran superficie forestal y una riqueza específica notable. El siguiente mapa muestra la distribución de los espacios de la red [Natura 2000](http://www.juntadeandalucia.es/medioambiente/site/portalweb/menuitem.220de8226575045b25f09a105510e1ca/?vgnextoid=d0e77b32b31f4310VgnVCM1000001325e50aRCRD), que puede considerarse como la red de espacios protegidos de Andalucía. 



![Mapa 1: Espacios de la Red Natura en Andalucía](https://github.com/aprendiendo-cosas/A_corredores_ecologia_ccaa/raw/2020-2021/images/1_enp.png)



Esta red de espacios protegidos incluye buena parte de todo el territorio considerado como "natural" en la región. Es decir, la mayoría de los bosques, matorrales o pastos naturales se encuentran dentro de la red de espacios protegidos. El siguiente mapa muestra la superficie ocupada por "vegetación natural" (verde) y por zonas no "naturales" (naranja. Cultivos, infraestructuras humanas, etc.). También se superponen el contorno de la red Natura 2000 y el de las principales infraestructuras viarias y núcleos urbanos.

![Mapa 2: distribución de vegetación natural en Andalucía](https://github.com/aprendiendo-cosas/A_corredores_ecologia_ccaa/raw/2020-2021/images/3_infraestructuras.png)



El fin último de este ejercicio es analizar en qué medida los espacios protegidos se comportan como islas de biodiversidad en medio de una matriz ocupada por cultivos e infraestructuras. Se trata de evaluar cómo se podrían conectar los espacios protegidos de Andalucía usando como marco conceptual la biogeografía de islas.

Para empezar, recuerda que la biogeografía de islas describe cómo cambia la riqueza de especies de una serie de fragmentos aislados en función de su distancia y de su tamaño. La distancia afecta a la tasa de inmigración de especies y el tamaño afecta fundamentalmente a la tasa de extinción de especies. En este caso, evaluaremos cómo se pueden combinar una serie de criterios ecológicos con otros relacionados con la distribución de infraestructuras humanas para planificar la creación de una red de corredores ecológicos. 

Dicho esto, tienes que generar un mapa que asigne un valor de idoneidad a cada punto del territorio no protegido en función de su capacidad de servir como corredor ecológico ([aquí](https://es.wikipedia.org/wiki/Corredor_ecol%C3%B3gico) tienes una definición general). El siguiente mapa muestra nuestra zona de estudio, que comprende todo el territorio andaluz no ocupado por la [Red Natura 2000](https://es.wikipedia.org/wiki/Red_Natura_2000). Ver mapa inferior.

![Zona de estudio](https://github.com/aprendiendo-cosas/A_corredores_ecologia_ccaa/raw/2020-2021/images/zona_estudio.png)

Para hacer este análisis tendrás que aplicar la técnica de evaluación multicriterio que aprendimos en la sesión sobre competencia intraespecífica. En este ejercicio, usaremos las siguientes variables ambientales:



## Variables a utilizar



### Biodiversidad (índice de Shannon)

Como sabes, el índice de Shannon permite conocer la diversidad de una comunidad biológica dada. De manera parecida a como haremos para generar el mapa de biodiverisidad de Sierra Nevada, se ha obtenido un mapa de biodiversidad de nuestra zona de estudio. Para ello se han usado los datos de ocurrencia de especies que hay disponibles en [GBIF](https://www.gbif.org/) (se trata de una organización internacional que almacena datos de biodiversidad). 

Desde el punto de vista del objetivo de este trabajo, asumiremos que la idoneidad de un punto del territorio aumenta al hacerlo su biodiversidad. Los lugares con mayor índice de Shannon tienen más capacidad de albergar ecosistemas funcionales y por tanto de servir como corredores ecológicos. **Así que a más diversidad de Shannon, más idoneidad**. Es decir, para obtener el mapa de idoneidad se usa una función de transferencia directa y lineal. Abajo puedes descargar el mapa de idoneidad desde el punto de vista de la biodiversidad. El mapa muestra la distribución de la aptitud de cada punto de estudio en función del índice de Shannon. Los colores más azules indican más aptitud (mayor índice de Shannon). El color rojo indica menor aptitud (muy bajo índice de Shannon)

![Mapa aptitud biodiversidad](https://github.com/aprendiendo-cosas/A_corredores_ecologia_ccaa/raw/2020-2021/images/apt_biodiv.png)



### **Distancia a espacios protegidos**

Según la biogeografía de islas, la distancia entre dos "islas" condiciona la probabilidad de que exista la inmigración. En nuestro caso las islas son los espacios protegidos (incluidos en la red Natura 2000), por lo que podemos asumir que un punto determinado del territorio funcionará tanto mejor como corredor cuanto más cerca esté de un espacio protegido. **A más distancia, menor idoneidad**. Es decir, para obtener este mapa de idoneidad se usó una función de transferencia indirecta y lineal. A continuacón puedes ver el mapa de idoneidad desde el punto de vista de la distancia a espacios de la red Natura 2000. Y [aquí](http://www.juntadeandalucia.es/medioambiente/site/portalweb/menuitem.220de8226575045b25f09a105510e1ca/?vgnextoid=d0e77b32b31f4310VgnVCM1000001325e50aRCRD) tienes información general sobre la red Natura 200 en Andalucía. 

![Mapa de aptitud respecto a distancia a Red Natura 2000](https://raw.githubusercontent.com/aprendiendo-cosas/A_corredores_ecologia_ccaa/2020-2021/images/apt_dist_natura.png)



### Grado de naturalidad

En este trabajo consideramos que un criterio importante para que un punto pueda ser considerado como corredor ecológico, es su grado de naturalidad. Distinguimos lugares con vegetación natural de otros que no tienen vegetación natural. Esta información procede del mapa [forestal español](https://www.mapa.gob.es/es/cartografia-y-sig/ide/descargas/desarrollo-rural/mfe.aspx). Para transformar esta variable de naturalidad en un criterio de aptitud, se considera que **a más naturalidad, más aptitud**. Como solo hay dos tipos de valores (natural o no natura), el mapa de aptitud generado tiene solo valores de 1 (zonas naturales) y 0 (zonas no naturales). El mapa de abajo muestra la distribuicón del grado de naturalidad.

![Mapa de aptitud según naturalidad](https://raw.githubusercontent.com/aprendiendo-cosas/A_corredores_ecologia_ccaa/2020-2021/images/apt_naturalidad.png)



### Distancia a infaestructuras viarias

Los criterios descritos anteriormente reflejan los aspectos ecológicos del problema que nos ocupa (biodiversidad, distancia a espacios protegidos, naturalidad de cada punto). Los tres criterios están relacionados con la biogeografía de islas. Sin embargo, además de la ecología, en este caso intervienen otros aspectos clave relacionados con la forma en la que el ser humano modifica el territorio y altera el funcionamiento de las infraestructuras naturales. Uno de los impactos principales procede de las infraestructuras viarias, que fragmentan el territorio e impiden en muchas ocasiones el libre tránsito de la fauna. En este sentido, se considera que la aptitud de un punto del territorio para actuar como corredor ecológico depende de su distancia a una infraestructura viaria. **A más distancia mayor aptitud**. De esta manera, abajo puedes ver un mapa de aptitud desde este punto de vista. Dicho mapa se muestra con la misma paleta de colores que en los demás mapas. 

![Aptitud desde el punto de vista de la distancia a carreteras](https://raw.githubusercontent.com/aprendiendo-cosas/A_corredores_ecologia_ccaa/2020-2021/images/apt_dist_carreteras.png)

### **Distancia a zonas urbanas**

Otro elemento espacial de gran importancia para caracterizar la presencia de corredores ecológicos, son los núcleos urbanos. En este sentido, consideramos que la idoneidad de un punto del territorio para comportarse como corredor es tanto **mayor cuanto mayor sea la distancia al núcleo urbano más cercano**. Abajo puedes ver este mapa de aptitud.

![Mapa de aptitud respecto a la distancia a zonas urbanas](https://raw.githubusercontent.com/aprendiendo-cosas/A_corredores_ecologia_ccaa/2020-2021/images/apt_dist_zona_urbana.png)



### **Presencia de vías pecuarias**

Por último, además de las "infraestructuras naturales" y las creadas por el ser humano, se incluye en este análisis un elemento que podría ser clave para nuestro objetivo: las vías pecuarias. Se trata de rutas lineales que se usaban en la antigüedad (todavía hoy se usan algunas) para el movimiento de ganado desde las zonas de pasto de invierno hasta las de verano (la llamada trashumancia). Resulta que las vías pecuarias son de titularidad pública y por tanto no pueden ser ocupadas por usos distintos a aquellos por las cuales fueron concebidas. Si te interesa el asunto de las vías pecuarias, puedes empezar leyendo [esto](http://www.juntadeandalucia.es/medioambiente/site/portalweb/menuitem.7e1cf46ddf59bb227a9ebe205510e1ca/?vgnextoid=720e1035e45d6410VgnVCM2000000624e50aRCRD&vgnextchannel=ffd439b8301f4310VgnVCM1000001325e50aRCRD) 

En este ejercicio se considera que un punto ocupado por una vía pecuaria tiene una idoneidad alta desde el punto de vista de su capacidad para ser usado como corredor ecológico. Esto ocurre independientemente de si en ese punto hay o no unas buenas condiciones ecológicas (según los tres criterios descritos más arriba). El hecho de que estos terrenos sean de titularidad pública, permite plantear la posibilidad de que se restauren para transformarse en corredores ecológicos. Éste es uno de los aspectos sobre los que tendrás que reflexionar en este ejercicio. 

Abajo puedes mapa el mapa de idoneidad desde el punto de vista de la presencia de vías pecuarias. 

![Mapa de aptitud respecto a la presencia de vías pecuarias](https://raw.githubusercontent.com/aprendiendo-cosas/A_corredores_ecologia_ccaa/2020-2021/images/apt_vias_pecuarias.png)



## Secuencia de acciones a realizar

Una vez estudiados los criterios a utilizar en este trabajo deberás de:

1. Construir dos escenarios diferentes que combinen de manera particular los criterios anteriores usando la técnica de evaluación multicriterio. Para ello deberás de asignar un peso a cada variable. Recuerda que la suma de todos los pesos debe de ser uno. Cuanto mayor sea el peso de cada variable, más importante será la misma en el resultado final. Por ejemplo, si pones un peso de 0.9 en la variable de biodiversidad, el mapa resultante se parecerá mucho al mapa de biodiversidad. En ese caso estarás diciendo que los lugares adecuados para construir corredores son sitios donde hay mucha biodiversidad. Si por el contrario pones el mismo peso a todas las variables, tu resultado será una combinación de todas las variables con la misma importancia. Lo importante aquí es que **justifiques** por qué usas una combinación de pesos y no otra. No hay una solución válida, sino que la clave es que justifiques tu decisión basándote en lo que sabes. Tampoco es obligatorio que uses todas las variables que se describen más arriba. Si decides excluir alguna, justifícalo. También puedes incorporar otras que no se hayan tenido en cuenta, por supuesto. 
2. Aplica las dos combinaciones de pesos a los criterios. Esto generará una capa con resultados en cada caso. Como tienes dos escenarios, tendrás dos capas. Para aplicar la combinación de pesos tendrás que usar la calculadora de mapas según puedes ver aquí:

```R
 ("apt_biodiv@1" * 0.3)+("apt_naturalidad@1"*0.2)+("apt_dist_natura2000@1"*0.2)+("apt_dist_carreteras@1"*0.1)+("apt_dist_zona_urbana@1"*0.1)+("apt_vias_pecuarias@1"*0.1)
```

3. Guarda el resultado en un archivo con formato *.tif*. Cuando lo muestres en QGIS verás que hay píxeles con valores desde 0 hasta 1. Para seleccionar los píxeles que son mejores candidatos a convertirse en corredores ecológicos, deberás de reclasificar el raster. Para eso, usa la herramienta *reclasify by table*. Deberás de fijar un umbral para la reclasificación. Lo más fácil es que uses los valores que se muestran abajo, pero puedes usar los que tú consideres (siempre que lo justifiques). Guarda el mapa reclasificado con otro nombre que puedas reconocer.

| Minimum | Maximum | Value |
| :-----: | :-----: | :---: |
|    0    |   0.5   |   0   |
|0.5|1|1|

4. Reflexiona sobre los resultados obtenidos. Imagina que tienes que tomar la decisión de definir 3 corredores ecológicos en Andalucía y los resultados del análisis anterior son la única información que tienes para adoptarla. Puedes seleccionar zonas candidatas a declararse como corredores ecológicos a partir de los mapas obtenidos en los dos escenarios. Es decir, puedes considerar que los criterios para construir corredores ecológicos cambian según la zona. No es lo mismo definir corredores ecológicos en Sierra Morena que en Cabo de Gata, por ejemplo. Una vez hecha la selección, deberás de describir cada zona de la siguiente forma:
   * Nombre del corredor: invéntate un nombre para el corredor que aluda a sus características principales. Ej. corredor entre Sierra Morena y la Subbética cordobesa.
   * Espacios protegidos que conecta: Esta capa vectorial contiene todos los espacios de la Red Natura 2000. Puedes consultar el nombre de cada uno de ellos en QGIs. Justifica por qué, según tu criterio es importante conectar estos espacios protegidos.
   * Características de la zona propuesta como corredor: indica cuáles son las principales características de la zona seleccionada atendiendo a los criterios utilizados en el análisis. Por ejemplo, la zona XX se caracteriza por tener una alta biodiversidad y también por tener muchas vías pecuarias. Esto hace que ya tenga funcionalidad como corredor ecológico. O también, la zona YY tiene muchas vías pecuarias, pero también está cerca de núcleos urbanos. Es decir, tiene mucha potencialidad como corredor, pero no es funcional aún. Debería de restaurarse el funcionamiento ecosistémico, etc. Para apoyar tu caracterización puedes incluir imágenes de la zona en cuestión. Bien imágenes aéreas o bien fotos de campo.



## Material a entregar

Una vez que hayas hecho lo anterior, deberás de preparar un informe que contenga la siguiente información:

* Justificación y descripción de los escenarios de pesos que has utilizado y las variables que has tenido en cuenta.
* Una ficha descriptiva de cada uno de los 3 corredores que hayas propuesto. Haz referencia en la ficha al escenario que ha permitido la "creación" del corredor seleccionado.
* Análisis crítico: indica qué variables echas en falta o qué aspectos de la metodología utilizada son mejorables según tu criterio. 

Una vez concluido el informe, deberás subirlo al moodle en formato **word**, **libre office** o equivalente. No en formato **pdf**, por favor.



## Información necesaria para hacer el ejercicio

Abajo tienes los enlaces de descarga de las capas que necesitas para hacer este trabajo. 

* [Capa de aptitud desde el punto de vista de la biodiversidad.](https://github.com/aprendiendo-cosas/A_corredores_ecologia_ccaa/raw/2020-2021/geoinfo/apt_biodiv.tif)
* [Capa de aptitud desde el punto de vista de la distancia a carreteras.](https://github.com/aprendiendo-cosas/A_corredores_ecologia_ccaa/raw/2020-2021/geoinfo/apt_dist_carreteras.tif)
* [Capa de aptitud desde el punto de vista de la distancia a espacios de la red Natura 2000.](https://github.com/aprendiendo-cosas/A_corredores_ecologia_ccaa/raw/2020-2021/geoinfo/apt_dist_natura2000.tif)
* [Capa de aptitud desde el punto de vista de la distancia a zonas urbanas.](https://github.com/aprendiendo-cosas/A_corredores_ecologia_ccaa/raw/2020-2021/geoinfo/apt_dist_zona_urbana.tif)
* [Capa de aptitud desde el punto de vista de la naturalidad](https://github.com/aprendiendo-cosas/A_corredores_ecologia_ccaa/raw/2020-2021/geoinfo/apt_naturalidad.tif)
* [Capa de aptitud desde el punto de vista de la presencia de vías pecuarias.](https://github.com/aprendiendo-cosas/A_corredores_ecologia_ccaa/raw/2020-2021/geoinfo/apt_vias_pecuarias.tif)
* [Delimitación de los espacios de la Red Natura 2000 en Andalucía.](https://github.com/aprendiendo-cosas/A_corredores_ecologia_ccaa/raw/2020-2021/geoinfo/Red_Natura_2000_andalucia.zip)




## Criterios de evaluación

En el moodle hay una rúbrica (pincha [aquí](https://es.wikipedia.org/wiki/R%C3%BAbrica_(docencia)) si no sabes lo que es una rúbrica) que describe de manera detallada los criterios de calificación. También puedes verlos en la siguiente tabla:




| Criterio de evaluación                                       | 0 puntos        | 1 punto                                                      | 2 puntos                                                     | 3 puntos                                                     | 4 puntos                                                     | 5 puntos                                                     |
| ------------------------------------------------------------ | --------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **Selección de variables**: Se refiere a si las variables elegidas para tu análisis se ajustan a la lógica del problema planteado. | No entrega nada | El conjunto de variables elegido no se alinea con el objetivo del trabajo. | No se tienen en cuenta los dos grupos de variables propuestas. | Incluye todas las variables sin justificar la decisión.      | Excelente selección de variables.                            | Además de lo anterior, incorpora variables nuevas no propuestas inicialmente en el ejercicio. |
| **Justificación de las decisiones adoptadas**: Se refiere sobre todo a la combinacion de pesos en los dos escenarios requeridos y a la selección de corredores. | No entrega nada | No justifica en ningún caso los pesos adoptados ni las zonas propuestas como corredores ecológicos. | La justificación no se alinea con nada conocido (por este humilde profesor) | Buena parte de las decisiones adoptadas están correctamente justificadas. | Tanto tu selección de pesos como la propuesta de zonas de corredores es muy convincente. | No estoy en absoluto de acuerdo con lo que propones, pero está tan bien justificado que me has convencido. |
| **Adecuación**: Este criterio evalúa en qué medida los conceptos mostrados en el trabajo están relacionados con la biogeografía de islas. | No entrega nada | No se observa nada relacionado con la biogeografía de islas. | Los conceptos teóricos en los que se basa el ejercicio aparecen tangencialmente. | Incorpora adecuadamente la biogeografía de islas y la fragmentación. | Además de lo anterior, mencionas adecuadamente la interferencia de las actividades humanas con las redes de "infraestructuras naturales" | Excelente integración de marcos conceptuales diferentes. Además de los requeridos has incluido otros. |
| **Legibilidad:** hace referencia a lo bien escrito que está el texto y a su legibilidad | No entrega nada | Apenas entiendo lo que has escrito                           | He tenido que reinterprestar casi cada frase para entenderlo | Se entiende bien todo, pero el texto no es fluido            | Muy buena redacción. La lectura fluye fácilmente, cual novela. | Impecable estilo de escritura.                               |



**PONER EN LA RÚBRICA ALGO PARA VALORAR LA PRESENTACIÓN Y LOS CRITERIOS ESTÉTICOS.**

**incluir una VARIAble que tenga en cuenta el tamaño de las islas (ENPs). Quizás esto les ayude a distinguir mejor los factores implicados en la biogeografía de islas.**

**incluir algo que permita distinguir mejor las variables ecológicas de las antrópias**


## Material útil para hacer la tarea

* [*An integrated approach for studying the land suitability for ecological corridors through spatial multicriteria evaluations*](https://github.com/aprendiendo-cosas/A_corredores_ecologia_ccaa/raw/2020-2021/biblio/ecological_corridors_multicriteria.pdf). Artículo científco en el que se inspira este ejercicio.

* [*Natura 2000 sites, public forests and riparian corridors: The connectivity backbone of forest green infrastructure*](https://github.com/aprendiendo-cosas/A_corredores_ecologia_ccaa/raw/2020-2021/biblio/ecological_corridors_spain.pdf). Artículo científico en el que se habla de corredores ecológicos en España.

* [*Multi-criteria decision analysis for nature conservation: A review of 20 years of applications*.](https://github.com/aprendiendo-cosas/A_corredores_ecologia_ccaa/raw/2020-2021/biblio/MCE_review.pdf) Revisión sobre el uso de la técnica de evaluación multicriterio aplicada a cuestiones ambientales.

* [Video](https://youtu.be/GIh5lWzQV_k) de una grabación de clase del curso 2019-2020 en la que se describe el contenido del ejercicio.

  

