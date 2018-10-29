# Dataton_BC_2018

 ## ZenAI 
	
    Ana Isabel Rúa G. 
    Julián Andrés Aranzalez  
    Sebastián Uribe O.

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

# PFM APP (PROACTIVE FINANCIAL MANAGEMENT)

Basado en los resultados de la categorización, proporcionamos servicios que favorecen la adhesión a aplicativos PFM.
Los modelos desarrollados permiten la implementación de una amplia gama de casos de uso de PFM.
La funcionalidad incluye (ejemplos):

* Históricos: muestra el comportamiento histórico de las transacciones del usuario por periodos de tiempo flexibles
* Gastos por categorías:  datos de gastos que se utilizarán en gráficos circulares
* División de transacciones en varias categorías: asignación de categoría a una transacción (por ejemplo, pago de pensión educativa, pago de servicios públicos, etc.) una vez finalizado el pago, de esta manera el usuario no tendrá que ingresar los datos de manera manual sino que estos se irán procesesando.

