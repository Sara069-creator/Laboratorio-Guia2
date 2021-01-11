# Laboratorio-Guia2
### PRÁCTICA No. 2 ANÁLISIS DE MALLAS

#### OBJETIVO GENERAL
- Comprender el método llamado (análisis de malla), aplicando la ley de Kirchhoff para voltajes de una trayectoria cerrada y establecer una relación entre el uso de la Ley de Ohm y la Ley de Kirchoff

#### OBJETIVO ESPECIFICO
-	Identificar la forma correcta de medición de voltaje y corriente con el multímetro en circuitos analizados con mallas.

-	Comparar los cálculos teóricos con los prácticos de medición de tensión, intensidad de corriente eléctrica y resistencias.

-	Entender la forma de uso del protoboard, multímetro, resistencias y de los demás materiales de laboratorio para hacer un uso correcto de ellos.


#### MARCO TEORICO

![image](https://user-images.githubusercontent.com/76060654/104211327-f2321100-5401-11eb-8c60-01d9a0e458c7.png)

|De acuerdo con el tipo de circuito y la forma en que se seleccionan las mallas se pueden tener distintas posibilidades de conexión de las fuentes:|
|---|

•Fuentes de corriente controladas.

• Fuentes de voltaje independientes.

• Fuentes de voltaje controladas.

• Fuentes de corriente independientes no
compartidas por varias mallas.

• Fuentes   de   corriente   independientes
compartidas por varias mallas.


#### DIAGRAMA

![image](https://user-images.githubusercontent.com/76060654/104211602-41784180-5402-11eb-86c7-f3f549dd4afc.png)

### INFORMACION GENERAL

En este documento se ilustrará el uso de LVK para poder expresar voltajes en función de corrientes, se procede a realizar un montaje de un circuito resistivo con resistencias en serie y paralelo de diferentes valores, que formen mallas para realizar su respectivo análisis midiendo los valores de voltaje, corriente y potencia de cada elemento del circuito.

#### LISTA DE COMPONENTES
|CANTIDAD|MATERIAL O EQUIPO|
|:---:|:---:|
|1|Fuente de voltaje de C.D|
|1|Multímetro Digital|
|1|Resistor de 820 Ω|
|1|Resistor de 390 Ω|
|1|Resistor de 1 kΩ|
|1|Resistor de 1.2 kΩ|
|1|Resistor de 2.2 kΩ|
|1|Protoboard|
#### Explicación

Armamos muestro circuito mixto con 3 mallas en el simulador tinkerkat 
Para calcular la corriente de cada malla, procedemos armando 3 ecuaciones con 3 incógnitas, empezamos con la primera malla tomando en cuenta que la corriente que entra va hacer positiva y sale negativa, en este caso va a entrar 18 positivo le restamos 820(I1) le restamos 1 y le multiplicamos (I1-I2) ya que esa resistencia 1 está entre la malla 1 y la malla 2 y a esa respectiva ecuación la igualamos a 0, hacemos los respectivos procedimientos matemáticos donde nos va a salir la primera ecuación : -1.82(I1)+1(I2)= -18.
Hacemos lo mismo con la malla 2, en este caso la corriente va a salir -1.2(I2) le restamos 2.2 y le multiplicamos (I2-I3) ya que esa resistencia está compartiendo la malla 2 y la malla 3 procedemos restando la siguiente resistencia que es 1 que multiplica (I2-I1) por el mismo motivo que comparte la malla 2 y la malla 1, hacemos el respectivo procedimiento matemático e igualamos a 0 y nos va a salir nuestra segunda ecuación: -4.4(I2)+2.2(I3)+1(I1)=0.
Hacemos el mismo procedimiento con la malla 3 donde la corriente saliente va hacer -0,39(I3) le restamos 5 y le restamos los 2.2que multiplica(I3-I2), hacemos los procedimientos matemáticos e igualamos a 0.
-2.59(I3)+2.2(I2)= 5
Con esas tres respectivas ecuaciones con 3 incógnitas hacemos sistema de ecuaciones en la cual nos va a salir el resultado de cada incógnita en este caso, el resultado de las 3 corrientes.
### TABLA
|MALLAS|RESULTADOS ANALITICOS|RESULTADOS EXPERIMENTALES|RESULTADOS SIMULADOS|
|---|---|---|---|
|Cm1|11,45 mA|10.6 mA|11,45 mA|
|Cm2|2,84 mA|3.25 mA|2,84 mA|
|Cm3|488 mA|-875µA|488 mA|

### CALCULOS:

![image](https://user-images.githubusercontent.com/76060654/104212848-a718fd80-5403-11eb-8e86-b5bafed97908.png)

#### DESCRIPCIÓN DE PRERREQUISITOS Y CONFIGURACIÓN

Las aplicaciones secundarias necesarias para la realización del proyecto tenemos simuladores que de igual forma nos permite realizar las practicas de los laboratorios en Fundamentos de Circuitos:

-	La segunda ley de Kirchhoff nos dice que la suma algebraica de todos los voltajes en una malla o bucle cerrado, debe ser igual a cero. Al referirnos a la suma algebraica, implica el cuidado de las polaridades de la fuente de energía, así como todos los signos de las caídas de tensión de cada uno de los componentes eléctricos. De modo que, al momento de aplicar la segunda ley de Kirchhoff, hay que ser muy precavidos en sentido de la orientación de la corriente y, por ende, con los signos de los voltajes de los componentes contenidos dentro de la malla.

-	Esta ley está fundamentada en la ley de la conservación de la energía, ya que establece que cada malla es un camino conductor cerrado, en el cual no se genera ni se pierde potencial. Por ello, la corriente no puede aparecer ni desaparecer de la nada. En consecuencia, la suma de todos los voltajes alrededor de este camino debe ser nula, para mantener el balance energético dentro del lazo..

-	La ventaja de usar esta técnica es que crea un sistema de ecuaciones para resolver el circuito, en este caso serian tres ecuaciones con tres incógnitas. 

Y obtendríamos lo que son las corrientes de cada malla.

#### APORTACIONES

Gracias al análisis de mallas se puede determinar la tensión o corriente de cualquier elemento en un circuito plano ya que esta es una técnica que hace uso de la LVK (ley de voltaje de Kirchhoff)

La gran ayuda que solventa esta técnica, es sobre la resolución de un circuito ya que proporciona un sistema de ecuaciones, evitándonos en gran medida (en algunos casos) muchos pasos en el procedimiento de una corriente o alguna tensión de un circuito.

En el análisis de mallas, usamos las “mallas” para crear las ecuaciones LVK de un circuito eléctrico.
Para usar esta técnica se procede de la siguiente manera: se asigna a cada una de las mallas del circuito una corriente imaginaria que circula en el sentido que nosotros elijamos; se prefiere asignarles a todas las corrientes de malla el mismo sentido. De cada malla del circuito, se plantea una ecuación que estará en función de la corriente que circula por cada elemento. En un circuito de varias mallas resolveríamos un sistema lineal de ecuaciones para obtener las diferentes corrientes de malla.

En la técnica de análisis de malla existen dos casos especiales: supermallas y fuentes dependientes.


 1. (Supermallas:) Existe una supermalla cuando una fuente de corriente está entre dos mallas esenciales. Para tratar la supermalla, se trata el circuito como si la fuente de corriente no estuviera allí. Esto produce una ecuación que incorpora las dos corrientes de malla. Una vez que se plantee esta ecuación, se necesita una ecuación que relacione las dos corrientes de malla con la fuente de corriente, esto será una ecuación donde la fuente de corriente sea igual a una de las corrientes de malla menos la otra

 2. Fuentes dependientes: Una fuente dependiente es una fuente de corriente o de tensión que depende de la tensión o de la corriente de otro elemento en el circuito.
Cuando una fuente dependiente está en una malla esencial, la fuente dependiente debería ser tratada como una fuente normal. Después de que se haya planteado la ecuación de malla, se necesita una ecuación para la fuente dependiente. Esta es una ecuación que relaciona la variable de la fuente dependiente con la corriente o tensión de la fuente de la que depende del circuito.


#### Conclusiones


-	Esta práctica dio a reconocer los entendimientos sobre la resolución de ejercicios de mallas y cómo proceder a analizarlos y poder recordar/razonar las fórmulas para poder realizarlos sin ninguna pérdida de tiempo. 

- Para poder proceder a realizar la práctica de laboratorio de circuitos, se necesitó previamente una introducción a los materiales sin obviar la necesidad de un conocimiento previo acerca de los materiales y elementos usados, pero no se elimina el requisito de tener bases acerca de nuestro proyecto. 

- La práctica realizada fue con relación al análisis de mallas que al realizarlas nos dio resultados prácticos y exactos sobre todo el diagrama, aunque existió problemas leves sobre conocimientos en el ejercicio el resultado final dio los resultados esperados y correctos.


#### Bibliografía

El método de la corriente de malla (artículo). (2015). Khan Academy. https://es.khanacademy.org/science/electrical-engineering/ee-circuit-analysis-topic/ee-dc-circuit-analysis/a/ee-mesh-current-method

P. (2020, 10 abril). Ley de Kirchhoff: Análisis de mallas. HETPRO/TUTORIALES. https://hetpro-store.com/TUTORIALES/ley-de-kirchhoff-analisis-de-mallas/

Trejo, R. (2018). 1.6. Análisis de Mallas. - Circuitos Eléctricos I. mediosdiitalesricardotrejo. https://sites.google.com/site/e91mediosdiitalesricardotrejo/home/1-6-analisis-de-mallas

Zapata, F. (2019, 1 noviembre). Análisis de mallas: conceptos, métodos, ejemplos. Lifeder. https://www.lifeder.com/analisis-de-mallas/

Colaboradores de Wikipedia. (2020, 14 octubre). Análisis de mallas. Wikipedia, la enciclopedia libre. https://es.wikipedia.org/wiki/An%C3%A1lisis_de_mallas

P. (2020, 10 abril). Ley de Kirchhoff: Análisis de mallas. HETPRO/TUTORIALES. https://hetpro-store.com/TUTORIALES/ley-de-kirchhoff-analisis-de-mallas/


#### Anexos



![image](https://user-images.githubusercontent.com/76060654/104234477-7b0c7500-5421-11eb-8129-f930199877ff.png)                         ![image](https://user-images.githubusercontent.com/76060654/104234472-7942b180-5421-11eb-9fb0-48298e062871.png)

![image](https://user-images.githubusercontent.com/76060654/104234482-7cd63880-5421-11eb-806d-78535ff5f832.png)
