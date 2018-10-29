# Dataton_BC_2018

 ## ZenAI 
	
    Ana Isabel Rúa G. 
    Julián Andrés Aranzalez  
    Sebastián Uribe O.
#### Para ampliación de la información aquí contenida remitirse al documento ***Informe Final ZenAI***, de manera análoga, remitirse al documento *descriptipo.ipynb*    


# Descripción del reto
Los datos entregados en este reto corresponden a transacciones realizadas por clientes persona del banco vía PSE. Estas transacciones, a diferencia de las transacciones realizadas vía POS, no cuentan con un código MCC atado a la transacción, que permite conocer la categoría de comercio a la que pertence el establecimiento de comercio donde se realiza la transacción. Adicionalmente, muchas de estas transferencias por PSE corresponden a transferencias de pagos de servicios públicos, seguros, colegios, arrendamientos, y otros gastos que pueden ser denominados como gastos grandes. En el marco de un sistema de gestión de finanzas personales, poder categorizar adecuadamente estas transacciones que se realizan por PSE es de suma importancia para contar con una foto completa de la actividad de gastos de los clientes. Para este reto, los equipos participantes tendrán acceso a una muestra de transacciones PSE que corresponden a algo más de 300 mil clientes (persona), seleccionados de manera aleatoria. La tabla de transacciones cuenta con 11.8 millones de registros (uno para cada transacción), realizados entre septiembre de 2016 y octubre de 2018.

***NOTA*** Los datos han pasado por un proceso relativamente simple de curación, pero se han dejado algunos ruidos en la calidad de éstos con el fin de que los equipos también lleven a cabo un proceso de inspección y limpieza.

# Metodología de la Solución Propuesta

Para la solución a este reto se utilizará la metodología CRISP-DM, mediante la cual se busca generar un resultado que haga un uso adecuado de los datos y permita resolver de forma efectiva el problema inicial planteado. De esta forma, se seguirán los siguientes pasos:

	Entendimiento del Negocio
	Entendimiento de los Datos
	Preparación de los Datos
	Modelamiento
	Evaluación
	Despliegue
	
Se debe tener presente también que a partir del entendimiento del negocio se plantearán varias soluciones diferentes, que puedan aportar desde diferentes perspectivas tanto a los clientes del banco (pagadores) como al banco por sí mismo.

# Desarrollo

El reto que se tiene es lograr clasificar las transacciones en una serie de categorías definidas por el banco, para lo cual el proceso que se seguirá es:

•	**Categorización de las transacciones**, para lo cual se utilizarán varias metodologías asociadas a minería de texto para asignar una categoría a cada transacción. Para esto se utilizarán metodologías como: Aplicación de relación campo categoría (específicamente para el campo "subsector"), Clasificación de transacciones que no tienen información, Web Scraping para obtener categorías de páginas que tengan información relevante, y uso de matrices TF para aplicarlas bolsas de palabras al set de datos, y finalmente clusterización.

Una vez clasificados los 12M de registros iniciales según las categorías definidas (se partió de las categorías propuestas por Bancolombia, y se agregaron dos adicionales), se procederá a generar un modelo que permita clasificar nuevas transacciones que entregue el banco, de tal forma que el proceso pueda llevarse a producción sobre nuevos registros, y se pueda generar valor tanto para el banco como para los clientes.

•	**Categorización de los clientes**, para lo cual se hará uso de la información de los clientes para realizar un proceso de correlación que indique qué tipos de clientes son más propensos a realizar cada tipo de transacción, es decir, no analizar solo cuáles atributos son relevantes frente a cada clasificación, sino las categorías específicas de cada atributo.

Esta información se utilizará también para crear clusters que permitan agruparlos y a partir de ello poder implementar modelos que le permitan al banco generar valor mediante estrategias como cross-selling, y al cliente tener una base de comparación sobre la cual pueda recibir recomendaciones si su comportamiento de gasto es superior al de personas con características similares.

Cabe resaltar que todo el procesamiento de los datos estará acompañado de los respectivos procesos de exploración y preparación, para asegurar que los datos tengan una adecuada calidad y presentación, para que así puedan ser utilizados de la forma más precisa posible. Así mismo, se debe tener presente que se busca que el procesamiento sea eficiente, para que así se haga un óptimo uso de los recursos disponibles.

Finalmente, se proponen una serie de mockups que permitan llevar los modelos propuestos a la práctica. Aunque esto es algo que posiblemente requiera trabajos más profundos de co-creación, se hace esta aproximación para lograr que los modelos propuestos vayan más allá de solo el procesamiento de datos, y llegue a una propuesta de valor para el banco y sus clientes.

# PFM APP (PROACTIVE FINANCIAL MANAGEMENT)

Como se ha comentado, lo que se busca con este ejercicio es lograr aplicar los diferentes modelos propuestos, para lo cual se diseñaron una serie de mockups que sirvan como base para una definición de cómo llevar algunos de los modelos diseñados a la aplicación MFP del cliente. 

El siguiente link brinda acceso al mockup diseñado. También es posible descargar el aplicativo y evaluar de manera preliminar su potencial de funcionamiento y apropiación de cara a los clientes. https://marvelapp.com/3831cd3

Es importante resaltar en este punto que una de las causas por las cuales los aplicativos de PMF no suelen tener mucho éxito es el ingreso manual por parte de los clientes de la información correspondiente a las transacciones.
Es así como se evidencia una gran oportunidad si consideramos la posible integración de los servicios actualmente ofrecidos por el Banco y otras plataformas e información que puede ser recaudada.


![alt text](https://github.com/anarua1203/Dataton_BC_2018/blob/master/Imagenes/comportamiento_mes.jpg)


## Descripción
 
**Histórico de datos:** por medio de esta aplicación es posible brindar al usuario (quien en un principio no deberá ingresar ningún tipo de información relativa a sus gastos e ingresos) la información de comportamiento financiero para diferentes periodos. Adicionalmente es posible brindarle información de la distribución de sus gastos y visualizarlos en el aplicativo.

	 Cada uno de los movimientos que se hagan ya sea vía medio de pago Redeban o PSE, pueden ser categorizados y dispuestos para hacer uno de ellos mendiante los diferentes modelos y aplicaciones ya expuestos

  **Perfilamiento de clientes:** en ocasiones, la mejor manera de aprender es viendo como otras personas lo realizan. Es así pues, como basado en la información de los clientes y en la implementación de diferentes técnicas de Inteligencia artificial, machine learning, entre otras, es posible realizar una comparación del usuario, con otras personas que tengan características similares a las suyas e incluso tener acceso a diferentes  combinaciones  de presupuestos que le puedan orientar.
 **Sueños:** reconocer en los clientes sus metas y aspiraciones mayores siempre será importante. Este tipo de aplicativos, permite tener una relación de mayor cercanía con el cliente, quién verá en el banco, más que el lugar en el cual deposita su dinero, un aliado estratégico.
	
**Presupuesto:** Definición y seguimiento. 


	
	

