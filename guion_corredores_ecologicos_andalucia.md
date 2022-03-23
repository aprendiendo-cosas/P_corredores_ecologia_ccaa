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

<img src="https://github.com/aprendiendo-cosas/P_corredores_ecologia_ccaa/raw/main/images/01_natural.jpeg" alt="naturaleza" style="zoom:100%;" />

Sin embargo, la realidad es bien diferente. El territorio se encuentra profundamente fragmentado y alterado por la actividad humana. El paisaje de Andalucía es en la actualidad una matriz de cultivos en los cuales se inserta una serie de islas de naturaleza. La siguiente imagen muestra la situación real de nuestra región.

<img src="https://github.com/aprendiendo-cosas/P_corredores_ecologia_ccaa/raw/main/images/03_islas.jpeg" alt="naturaleza" style="zoom:100%;" />

En este contexto, cuando los sistemas naturales están fragmentados, es importante conocer en qué medida el tamaño de las islas naturales existentes pueden sostener la diversidad total del sistema. Aquí es donde, en este caso, entra la biogeografía de islas. Esta teoría explica cómo cambia la diversidad de una serie de islas inmersas en una matriz no apta para la supervivencia de ciertas especies. Lo hace con las siguientes afirmaciones:

+ Cuanto más grande es una isla, más especies alberga.
+ Cuanto más grande es una isla, más cantidad de especies recibe vía inmigración.
+ Cuanto más grande es una isla, menor es la probabilidad de extinción de especies en su interior.
+ Cuanto más lejos está una isla de otras, menor es la probabilidad de que a la primera llegen individuos de otras islas. 

Estos preceptos de la biogeografía de islas se aplican bien al diseño de redes de espacios protegidos. La siguiente figura muestra alguna de las ideas que se aplican en este sentido:

<img src="https://github.com/aprendiendo-cosas/P_corredores_ecologia_ccaa/raw/main/images/04_enps_islas.jpg" alt="naturaleza" style="zoom:100%;" />



En esta práctica nos centraremos en el concepto de [corredor ecológico](https://es.wikipedia.org/wiki/Corredor_ecol%C3%B3gico). Según la teoría de islas, es buena idea conectar los espacios naturales entre sí para maximizar el flujo de genes y con ello asegurar la conservación de la biodiversidad. 




## Diseño de corredores ecológicos en Andalucía



Andalucía cuenta con una amplia red de espacios naturales protegidos. No en vano, es considerada como un punto caliente de biodiversidad en la región Mediterránea. Cuenta con una gran superficie forestal y una riqueza específica notable. El siguiente mapa muestra la distribución de los espacios de la red [Natura 2000](http://www.juntadeandalucia.es/medioambiente/site/portalweb/menuitem.220de8226575045b25f09a105510e1ca/?vgnextoid=d0e77b32b31f4310VgnVCM1000001325e50aRCRD), que puede considerarse como la red de espacios protegidos de Andalucía. 



![Mapa 1: Espacios de la Red Natura en Andalucía](https://github.com/aprendiendo-cosas/P_corredores_ecologia_ccaa/raw/main/images/05_enp.png)



Esta red de espacios protegidos incluye buena parte de todo el territorio considerado como "natural" en la región. Es decir, la mayoría de los bosques, matorrales o pastos naturales se encuentran dentro de la red de espacios protegidos. Estos espacios protegidos son las islas de naturaleza que hemos comentado en el apartado anterior. El siguiente mapa muestra la superficie ocupada por "vegetación natural" (verde) y por zonas no "naturales" (naranja. Cultivos, infraestructuras humanas, etc.). También se superponen el contorno de la red Natura 2000 y el de las principales infraestructuras viarias y núcleos urbanos.

![Mapa 2: distribución de vegetación natural en Andalucía](https://github.com/aprendiendo-cosas/P_corredores_ecologia_ccaa/raw/main/images/06_infraestructuras.png)



El fin último de este ejercicio es analizar en qué medida los espacios protegidos se comportan como islas de biodiversidad en medio de una matriz ocupada por cultivos e infraestructuras. Se trata de evaluar cómo se podrían conectar los espacios protegidos de Andalucía usando como marco conceptual la biogeografía de islas.

Para empezar, recuerda que la biogeografía de islas describe cómo cambia la riqueza de especies de una serie de fragmentos aislados en función de su distancia y de su tamaño. La distancia afecta a la tasa de inmigración de especies y el tamaño afecta fundamentalmente a la tasa de extinción de especies. En este caso, evaluaremos cómo se pueden combinar una serie de criterios ecológicos con otros relacionados con la distribución de infraestructuras humanas para planificar la creación de una red de corredores ecológicos. 

Dicho esto, tienes que generar un mapa que asigne un valor de idoneidad a cada punto del territorio no protegido en función de su capacidad de servir como corredor ecológico. El siguiente mapa muestra nuestra zona de estudio, que comprende todo el territorio andaluz no ocupado por la [Red Natura 2000](https://es.wikipedia.org/wiki/Red_Natura_2000). Ver mapa inferior.

![Zona de estudio](https://github.com/aprendiendo-cosas/P_corredores_ecologia_ccaa/raw/main/images/07_zona_estudio.png)

Para hacer este análisis tendrás que aplicar la técnica de evaluación multicriterio que aprendimos en la sesión sobre competencia intraespecífica. En este ejercicio, usaremos las siguientes variables ambientales:



## Variables a utilizar



### Biodiversidad (índice de Shannon)

Como sabes, el índice de Shannon permite conocer la diversidad de una comunidad biológica dada. De manera parecida a como haremos para generar el mapa de biodiverisidad de Sierra Nevada, se ha obtenido un mapa de biodiversidad de nuestra zona de estudio. Para ello se han usado los datos de ocurrencia de especies que hay disponibles en [GBIF](https://www.gbif.org/) (se trata de una organización internacional que almacena datos de biodiversidad). 

Desde el punto de vista del objetivo de este trabajo, asumiremos que la idoneidad de un punto del territorio aumenta al hacerlo su biodiversidad. Los lugares con mayor índice de Shannon tienen más capacidad de albergar ecosistemas funcionales y por tanto de servir como corredores ecológicos. **Así que a más diversidad de Shannon, más idoneidad**. Es decir, para obtener el mapa de idoneidad se usa una función de transferencia directa y lineal. Abajo puedes descargar el mapa de idoneidad desde el punto de vista de la biodiversidad. El mapa muestra la distribución de la aptitud de cada punto de estudio en función del índice de Shannon. Los colores más azules indican más aptitud (mayor índice de Shannon). El color rojo indica menor aptitud (muy bajo índice de Shannon)

![Mapa aptitud biodiversidad](https://github.com/aprendiendo-cosas/P_corredores_ecologia_ccaa/raw/main/images/08_apt_biodiv.png)



### **Distancia a espacios protegidos**

Según la biogeografía de islas, la distancia entre dos "islas" condiciona la probabilidad de que exista la inmigración. En nuestro caso las islas son los espacios protegidos (incluidos en la red Natura 2000), por lo que podemos asumir que un punto determinado del territorio funcionará tanto mejor como corredor cuanto más cerca esté de un espacio protegido. **A más distancia, menor idoneidad**. Es decir, para obtener este mapa de idoneidad se usó una función de transferencia indirecta y lineal. A continuacón puedes ver el mapa de idoneidad desde el punto de vista de la distancia a espacios de la red Natura 2000. Y [aquí](http://www.juntadeandalucia.es/medioambiente/site/portalweb/menuitem.220de8226575045b25f09a105510e1ca/?vgnextoid=d0e77b32b31f4310VgnVCM1000001325e50aRCRD) tienes información general sobre la red Natura 200 en Andalucía. 

![Mapa de aptitud respecto a distancia a Red Natura 2000](https://github.com/aprendiendo-cosas/P_corredores_ecologia_ccaa/raw/main/images/09_apt_dist_natura.png)

### Tamaño de los espacios protegidos
Según la biogeografía de islas, al aumentar el tamaño de un fragmento natural también lo hace la capacidad del mismo de "exportar" especies a la matriz que lo rodea. De esta forma, dos puntos que se encuentren a la misma distancia de una isla (espacio protegido en nuestro caso) tendrán diferente aptitud para actuar como corredor en función del tamaño de la isla que tienen cerca. **Es decir, los puntos de la matriz que estén cerca de una isla grande podrán comportarse como corredores con más probabilidad que los que estén cerca de una isla pequeña.** Implementa esto en un SIG no es fácil. Para hacerlo hemos generado un mapa que asigna a cada píxel ocupado por matriz la superficie del espacio protegido (isla) más cercano. Puedes verlo a continuación:

![Mapa de aptitud respecto al tamaño del ENP más cercano](https://github.com/aprendiendo-cosas/P_corredores_ecologia_ccaa/raw/main/images/10_apt_dist_tamanio_ENP.png)

### Grado de naturalidad

En este trabajo consideramos que un criterio importante para que un punto pueda ser considerado como corredor ecológico, es su grado de naturalidad. Distinguimos lugares con vegetación natural de otros que no tienen vegetación natural. Esta información procede del mapa [forestal español](https://www.mapa.gob.es/es/cartografia-y-sig/ide/descargas/desarrollo-rural/mfe.aspx). Para transformar esta variable de naturalidad en un criterio de aptitud, se considera que **a más naturalidad, más aptitud**. Como solo hay dos tipos de valores (natural o no natura), el mapa de aptitud generado tiene solo valores de 1 (zonas naturales) y 0 (zonas no naturales). El mapa de abajo muestra la distribuicón del grado de naturalidad.

![Mapa de aptitud según naturalidad](https://github.com/aprendiendo-cosas/P_corredores_ecologia_ccaa/raw/main/images/11_apt_naturalidad.png)



### Distancia a infaestructuras viarias

Los criterios descritos anteriormente reflejan los aspectos ecológicos del problema que nos ocupa (biodiversidad, distancia a espacios protegidos, naturalidad de cada punto). Los tres criterios están relacionados con la biogeografía de islas. Sin embargo, además de la ecología, en este caso intervienen otros aspectos clave relacionados con la forma en la que el ser humano modifica el territorio y altera el funcionamiento de las infraestructuras naturales. Uno de los impactos principales procede de las infraestructuras viarias, que fragmentan el territorio e impiden en muchas ocasiones el libre tránsito de la fauna. En este sentido, se considera que la aptitud de un punto del territorio para actuar como corredor ecológico depende de su distancia a una infraestructura viaria. **A más distancia mayor aptitud**. De esta manera, abajo puedes ver un mapa de aptitud desde este punto de vista. Dicho mapa se muestra con la misma paleta de colores que en los demás mapas. 

![Aptitud desde el punto de vista de la distancia a carreteras](https://github.com/aprendiendo-cosas/P_corredores_ecologia_ccaa/raw/main/images/12_apt_dist_carreteras.png)

### **Distancia a zonas urbanas**

Otro elemento espacial de gran importancia para caracterizar la presencia de corredores ecológicos, son los núcleos urbanos. En este sentido, consideramos que la idoneidad de un punto del territorio para comportarse como corredor es tanto **mayor cuanto mayor sea la distancia al núcleo urbano más cercano**. Abajo puedes ver este mapa de aptitud.

![Mapa de aptitud respecto a la distancia a zonas urbanas](https://github.com/aprendiendo-cosas/P_corredores_ecologia_ccaa/raw/main/images/13_apt_dist_zona_urbana.png)



### **Presencia de vías pecuarias**

Por último, además de las "infraestructuras naturales" y las creadas por el ser humano, se incluye en este análisis un elemento que podría ser clave para nuestro objetivo: las vías pecuarias. Se trata de rutas lineales que se usaban en la antigüedad (todavía hoy se usan algunas) para el movimiento de ganado desde las zonas de pasto de invierno hasta las de verano (la llamada trashumancia). Resulta que las vías pecuarias son de titularidad pública y por tanto no pueden ser ocupadas por usos distintos a aquellos por las cuales fueron concebidas. Si te interesa el asunto de las vías pecuarias, puedes empezar leyendo [esto](http://www.juntadeandalucia.es/medioambiente/site/portalweb/menuitem.7e1cf46ddf59bb227a9ebe205510e1ca/?vgnextoid=720e1035e45d6410VgnVCM2000000624e50aRCRD&vgnextchannel=ffd439b8301f4310VgnVCM1000001325e50aRCRD) 

En este ejercicio se considera que un punto ocupado por una vía pecuaria tiene una idoneidad alta desde el punto de vista de su capacidad para ser usado como corredor ecológico. Esto ocurre independientemente de si en ese punto hay o no unas buenas condiciones ecológicas (según los tres criterios descritos más arriba). El hecho de que estos terrenos sean de titularidad pública, permite plantear la posibilidad de que se restauren para transformarse en corredores ecológicos. Éste es uno de los aspectos sobre los que tendrás que reflexionar en este ejercicio. 

Abajo puedes mapa el mapa de idoneidad desde el punto de vista de la presencia de vías pecuarias. 

![Mapa de aptitud respecto a la presencia de vías pecuarias](https://github.com/aprendiendo-cosas/P_corredores_ecologia_ccaa/raw/main/images/14_apt_vias_pecuarias.png)

## Integración de todas las capas para generar un mapa de corredores ecológicos

Una vez leído lo descrito más arriba deberás de seleccionar los criterios que consideres más adecuados para idenficar sitios potencialmente útiles como corredores ecológicos. Puedes usar todos los que hemos descrito arriba o solo algunos. Justifica tu decisión. Una vez hecho esto tienes que integrar los criterios y obtener una capa única. En las siguientes secciones se describen dos métodos que ya vimos en la práctica sobre competencia intraespecífica.

### Evaluación multicriterio

El análisis multicriterio es una técnica muy sencilla que permite conciliar en un mismo mapa criterios diferentes. Es una forma de espacializar criterios decisionales basados en conocimiento experto. Es decir, gracias a esta técnica podemos obtener mapas que recojan los criterios de un centro decisor concreto con relación a un aspecto determinado.  En nuestro ejemplo tenemos varios criterios y se trata de unificarlos en un único mapa que asigne un valor de aptitud global a cada punto ocupado por pinares de repoblación. Por ejemplo:

+ Criterio de densidad: a más densidad más aptitud.
+ Criterio de profundidad del suelo: a más profundidad más aptitud.
+ Criterio de distancia a manchas donadoras de semillas: A más distancia menos aptitud.

Para agregar los criterios empezaremos asignando un peso a cada uno de ellos. La suma de los pesos ha de ser 1. El criterio que tenga más peso contribuirá en mayor medida al mapa final. Procedemos en dos pasos:

El proceso de integración se hace fácilmente con la calculadora de mapas de QGIS u operando con las capas raster en el caso de que trabajemos con R o con Python. El resultado final es la suma del producto de cada criterio (capa _apt_) por su peso. Introducimos la siguiente ecuación en la calculadora raster:

```python  
  ("apt_densidad@1"*0.6)+("apt_cti@1"*0.1)+("apt_distancia@1"*0.3)
 
```

La siguiente imagen muestra el método con otro ejemplo diferente:

<img src="https://github.com/aprendiendo-cosas/P_corredores_ecologia_ccaa/raw/main/images/15_pesos_ponderados.png" alt="imagen" style="zoom:40%;" />

Uno de los problemas del análisis multicriterio es que ocurre una compensación de criterios. Si una variable tiene un valor muy alto en un lugar determinado, puede que el resultado final en ese punto sea alto aunque el valor de un criterio importante en ese punto sea bajo. Esto puede hacer que lugares no adecuados sean etiquetados como sí adecuados. Un ejemplo que ilustra esta situación: imaginemos que queremos montar un equipo de baloncesto. Un buen jugador de baloncesto ha de tener las siguientes características:

+ Altura.
+ Fortaleza en los brazos.
+ Tobillos resistentes.

Si le damos distintos pesos a esas variables y con eso "puntuamos" la idoneidad de una lista de personas para entrar en nuestro equipo, puede darse la situación de que una persona tenga alta puntuación final aún teniendo los tobillos débiles. Eso implica tomar una decisión equivocada puesto que estaríamos incluyendo en el equipo a una persona que no rendiría bien. Esta situación denota que hay criterios que no solo tienen más peso que otros, sino que además deben satisfacerse **necesariamente** para tomar una decisión acertada. Y esto nos lleva a la segunda técnica de análisis de la decisión:

### Operadores booleanos

En esta segunda técnica no se asignan pesos a los criterios que combinamos sino que se establecen condiciones que deben cumplir los lugares de nuestra zona de estudio para ser idoneos según el objetivo del proceso decisiona en cuestión. Volviendo al ejemplo del jugador de baloncesto ideal, diríamos algo así: debe de tener los tobillos fuertes **y** **o bien** ser fuerte **o bien** ser alto. De alguna forma estamos diciendo que hay una condición **necesaria** para ser buen jugador, pero no suficiente. Necesita tener los tobillos resistentes y luego una de las otras dos condiciones. Esta forma de combinar criterios decisionales recibe el nombre de integración mediante operadores booleanos porque implican el uso de las conjunciones **o** e **y**. 

En el ejemplo que nos ocupa, usaremos operadores lógicos para integrar las tres capas. Consideraremos que un lugar es adecuado para satisfaer nuestros objetivos si cumple un criterio específico y una combinación de los otros dos. Es decir, pondremos como criterio fundamental que los lugares adecuados tengan una **alta densidad de pinos**. Si no se cumple este criterio, nunca se podrá obtener un valor alto al final del proceso de integración de las variables. Los otros dos criterios serán optativos entre sí. Es decir, seleccionaremos como lugares adecuados aquellos que **o bien están cerca de una mancha de vegetación natural, o bien tienen suelos potencialmente húmedos**. Es decir, en conjunto aplicaremos los siguientes criterios concatenados: Un lugar es considerado como adecuado si:

+ Tiene una alta densidad de pinos **Y**:
+ Está cerca de una mancha de vegetación natural **O** tiene suelos potencialmente húmedos. 

Para implementar esta operación en un SIG, usamos dos operadores matemáticos muy sencillos:

+ Valor **máximo** entre dos capas: es el equivalente al operador **O**. Si en un píxel hay valores altos de aptitud en una capa y bajos en otra, el resultado será alto, puesto que estamos eligiendo el máximo de ambos. Si la aptitud es alta en los dos casos, también seleccionaremos un valor alto. Es decir, se trata de un operador poco restrictivo.
+ Valor **mínimo** entre dos capas: es el equivalente al operador **Y**. Si en un píxel hay valores altos de aptitud en una capa y bajos en otra, el resultado será bajo, puesto que estamos eligiendo el mínimo de ambos. Solo si la aptitud es alta en los dos casos, seleccionaremos un valor alto. Es decir, se trata de un operador poco restrictivo.

La siguiente figura muestra el funcionamiento de estos operadores:

<img src="https://github.com/aprendiendo-cosas/P_corredores_ecologia_ccaa/raw/main/images/16_operadores_booleanos.png" alt="imagen" style="zoom:40%;" />

Para aplicar estos operadores a nuestras capas, puedes usar el comando [mosaic de SAGA](https://gis.stackexchange.com/questions/150312/combining-multiple-overlapping-rasters-retain-maximum-value). Este comando está disponible en QGIS. En algunas versiones de QGIS los operadores **Y** y **O** están disponibles en la calculadora de mapas. 

## Reclasificación de los resultados obtenidos

Tras aplicar cualquiera de las técnicas anteriores obtendremos un mapa con valores de aptitud que van de 0 a 1. Este mapa puede ser muy útil para comprender mejor el proceso socioecológico en el que estamos trabajando. Pero normalmente cuando se toman decisiones es necesario seleccionar una serie de zonas concretas en las que se va a realizar una actuación determinada. Por eso es útil simplificar el mapa resultante para elegir solo los lugares (=píxeles) que resulten más idoneos para nuestro objetivo. El resto los descartaremos porque no reunen los requisitos que hemos impuesto. Para hacer esta selección aplicaremos una operación muy común en análisis raster: [reclasificación](https://docs.qgis.org/3.4/en/docs/user_manual/processing_algs/qgis/rasteranalysis.html#qgisreclassifybytable). Consiste en reducir la diversidad de valores de un raster asigando nuevos en función de un rango. Por ejemplo, asignaremos el valor de 1 a todos los píxeles que tengan una aptitud igual o mayor de 0.8. Para hacer esto, construimos una tabla de reclasificación.

Para reclasificar una capa rastser en QGIS, buscamos el algoritmo "reclassify by table" en el buscador de procesos de QGIS. Añadimos los siguientes parámetros:

- _raster layer_: _apt\_final.tif_
- _reclassification table_: Abrimos la tabla y añadimos las siguientes filas:


| Desde (Mínimo) | hasta (Máximo) | Valor nuevo |
| -------------: | -------------: | ----------: |
|              0 |            0.9 |           0 |
|            0.9 |              1 |           1 |

 - _reclassified raster_ (capa de salida): _apt\_final\_re.tif_



## Secuencia de acciones a realizar

Una vez leído con atención las secciones anteriores deberás de:

1. Selecciona los criterios que consideres más adecuados para idenficar sitios potencialmente útiles como corredores ecológicos. Puedes usar todos los que hemos descrito arriba o solo algunos. Justifica tu decisión. También puedes incorporar otras que no se hayan tenido en cuenta, por supuesto. 
1. Integra todos los criterios seleccionados usando una o las dos técnicas descritas más arriba. Puedes combinar las dos o usar solo una. O definir distintos escenarios y usar una de ellas en cada uno. En cada escenario obtendrás un mapa en el que cada píxel de la matriz tiene un valor de idoneidad para convertirse en corredor según los criterios que hayas seleccionado. Es muy importante que justifiques tu decisión.
1. Reflexiona sobre los resultados obtenidos. Imagina que tienes que tomar la decisión de definir un corredor ecológico en Andalucía y los resultados del análisis anterior son la única información que tienes para adoptarla. Puedes seleccionar zonas candidatas a declararse como corredores ecológicos a partir de los mapas obtenidos en los escenarios que hayas considerado. Es decir, puedes considerar que los criterios para construir corredores ecológicos cambian según la zona. No es lo mismo definir corredores ecológicos en Sierra Morena que en Cabo de Gata, por ejemplo. Una vez hecha la selección, deberás de describir cada zona. Aquí tienes un ejemplo de cómo hacerlo:

     + Nombre del corredor: invéntate un nombre para el corredor que aluda a sus características principales. Ej. corredor entre Sierra Morena y la Subbética cordobesa.

   * Espacios protegidos que conecta: Esta capa vectorial contiene todos los espacios de la Red Natura 2000. Puedes consultar el nombre de cada uno de ellos en QGIs. Justifica por qué, según tu criterio es importante conectar estos espacios protegidos.

   * Características de la zona propuesta como corredor: indica cuáles son las principales características de la zona seleccionada atendiendo a los criterios utilizados en el análisis. Por ejemplo, la zona XX se caracteriza por tener una alta biodiversidad y también por tener muchas vías pecuarias. Esto hace que ya tenga funcionalidad como corredor ecológico. O también, la zona YY tiene muchas vías pecuarias, pero también está cerca de núcleos urbanos. Es decir, tiene mucha potencialidad como corredor, pero no es funcional aún. Debería de restaurarse el funcionamiento ecosistémico, etc. Para apoyar tu caracterización puedes incluir imágenes de la zona en cuestión. Bien imágenes aéreas o bien fotos de campo.




## Material a entregar

Una vez que hayas hecho lo anterior, deberás de preparar un informe que contenga la siguiente información:

* Justificación y descripción de los escenarios de pesos que has utilizado y las variables que has tenido en cuenta.
* Una ficha descriptiva de cada uno de los corredores que hayas propuesto. Haz referencia en la ficha al escenario que ha permitido la "creación" del corredor seleccionado.
* Análisis crítico: indica qué variables echas en falta o qué aspectos de la metodología utilizada son mejorables según tu criterio. 

Una vez concluido el informe, deberás subirlo [aquí](https://www.turnitin.com/?svr=25&session-id=&lang=en_us&r=36.292252621169) en formato **word**, **libre office** o equivalente. No en formato **pdf**, por favor.



## Información necesaria para hacer el ejercicio

+ [Este](https://github.com/aprendiendo-cosas/P_corredores_ecologia_ccaa/raw/main/geoinfo/criterios.zip) archivo .zip tiene las siguientes capas que necesitarás para hacer el trabajo.:
  * Capa de aptitud desde el punto de vista de la biodiversidad.
  * Capa de aptitud desde el punto de vista de la distancia a carreteras.
  * Capa de aptitud desde el punto de vista de la distancia a espacios de la red Natura 2000.
  * Capa de aptitud desde el punto de vista de la distancia a zonas urbanas.
  * Capa de aptitud desde el punto de vista de la naturalidad
  * Capa de aptitud desde el punto de vista de la presencia de vías pecuarias.
  * Capa de aptitud desde el punto de vista del tamaño del ENP más cercano a cada píxel de matriz.
* [Aquí](https://github.com/aprendiendo-cosas/P_corredores_ecologia_ccaa/raw/main/geoinfo/Red_Natura_2000_andalucia.zip) puedes descarar la delimitación de los espacios de la Red Natura 2000 en Andalucía.





## Criterios de evaluación

En el moodle hay una rúbrica (pincha [aquí](https://es.wikipedia.org/wiki/R%C3%BAbrica_(docencia)) si no sabes lo que es una rúbrica) que describe de manera detallada los criterios de calificación. También puedes verlos en la siguiente tabla:




| Criterio de evaluación                                       | 0 puntos        | 1 punto                                                      | 2 puntos                                                     | 3 puntos                                                     | 4 puntos                                                     | 5 puntos                                                     |
| ------------------------------------------------------------ | --------------- | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ | ------------------------------------------------------------ |
| **Selección de variables**: Se refiere a si las variables elegidas para tu análisis se ajustan a la lógica del problema planteado. | No entrega nada | El conjunto de variables elegido no se alinea con el objetivo del trabajo. | No se tienen en cuenta los dos grupos de variables propuestas. | Incluye todas las variables sin justificar la decisión.      | Excelente selección de variables.                            | Además de lo anterior, incorpora variables nuevas no propuestas inicialmente en el ejercicio. |
| **Justificación de las decisiones adoptadas**: Se refiere sobre todo a la combinacion de pesos en los dos escenarios requeridos y a la selección de corredores. | No entrega nada | No justifica en ningún caso los pesos adoptados ni las zonas propuestas como corredores ecológicos. | La justificación no se alinea con nada conocido (por este humilde profesor) | Buena parte de las decisiones adoptadas están correctamente justificadas. | Tanto tu selección de pesos como la propuesta de zonas de corredores es muy convincente. | No estoy en absoluto de acuerdo con lo que propones, pero está tan bien justificado que me has convencido. |
| **Adecuación**: Este criterio evalúa en qué medida los conceptos mostrados en el trabajo están relacionados con la biogeografía de islas. | No entrega nada | No se observa nada relacionado con la biogeografía de islas. | Los conceptos teóricos en los que se basa el ejercicio aparecen tangencialmente. | Incorpora adecuadamente la biogeografía de islas y la fragmentación. | Además de lo anterior, mencionas adecuadamente la interferencia de las actividades humanas con las redes de "infraestructuras naturales" | Excelente integración de marcos conceptuales diferentes. Además de los requeridos has incluido otros. |
| **Legibilidad:** hace referencia a lo bien escrito que está el texto y a su legibilidad | No entrega nada | Apenas entiendo lo que has escrito                           | He tenido que reinterprestar casi cada frase para entenderlo | Se entiende bien todo, pero el texto no es fluido            | Muy buena redacción. La lectura fluye fácilmente, cual novela. | Impecable estilo de escritura.                               |






## Material útil para hacer la tarea

* [*An integrated approach for studying the land suitability for ecological corridors through spatial multicriteria evaluations*](https://github.com/aprendiendo-cosas/P_corredores_ecologia_ccaa/raw/main/biblio/ecological_corridors_multicriteria.pdf). Artículo científco en el que se inspira este ejercicio.
* [*Natura 2000 sites, public forests and riparian corridors: The connectivity backbone of forest green infrastructure*](https://github.com/aprendiendo-cosas/P_corredores_ecologia_ccaa/raw/main/biblio/ecological_corridors_spain.pdf). Artículo científico en el que se habla de corredores ecológicos en España.
* [*Multi-criteria decision analysis for nature conservation: A review of 20 years of applications*.](https://github.com/aprendiendo-cosas/P_corredores_ecologia_ccaa/raw/main/biblio/MCE_review.pdf) Revisión sobre el uso de la técnica de evaluación multicriterio aplicada a cuestiones ambientales.

