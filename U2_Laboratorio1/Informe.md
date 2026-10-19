# Clasificación

Los datos que requieren protección son aquellos datos que pueden identificar al usuario y vulneran su derecho a la privacidad, además de comprometer la operación de la empresa y poner en riesgo la información almacenada. El nombre, rfc, correo, teléfono y código postal.

# Enmascaramiento

Se ocultaron los datos de carácter personal.  
Para el rol soporte.  
Para salvaguardar la privacidad de los clientes y reducir la superficie de vulnerabilidad.  
Se utilizó el enmascaramiento.

# Seudonimización

Se generó un número de identificación único de usuario referenciándose en el ID original del cliente.  
En pii.mapa_cliente.  
El Analista.  
Para que los usuarios que no necesiten ciertos datos para desempeñar sus funciones no tengan acceso a ellos y reducir las posibilidades de filtraciones o errores como eliminar los datos, etc.

# Anonimización

Se eliminaron los atributos de nombre, número telefónico, correo, rfc y ciudad.  
El rango de edad y la zona aproximada.  
Los grupos que permiten la identificación del usuario.  
Se puede lograr una reidentificación a través de la combinación de diferentes fuentes de datos.

# Retención

Se valoró la relevancia de mantener los registros si los registros exceden los 5 años de haberse creado. Si superaba ese periodo, entonces se eliminaban.  
Aquella información que sea relevante para los procesos operativos de la empresa.  
Se puede eliminar toda información que no sea necesaria para los procesos de la empresa.  
Se necesita una verificación de parte de roles superiores, respaldos, históricos, etc.

# Conclusiones

## ¿Qué técnica utilizarías para un área de soporte?

- Utilizaría el enmascaramiento debido a que este departamento requiere acceso a información de los clientes para realizar verificaciones, sin embargo no necesita conocer todos los datos personales del usuario.

## ¿Qué técnica utilizarías para un área de analítica?

- Utilizaría la anonimización ya que no se necesita información específica de los usuarios si no rangos y aproximados para realizar los análisis.

## ¿Qué técnica utilizarías para publicar estadísticas?

- Anonimización. No se requiere brindar datos específicos, solo rangos y estimaciones.

## ¿Por qué ninguna de estas técnicas sustituye al control de acceso?

- Porque el control de acceso es la herramienta que nos permite asegurarnos de que las personas adecuadas tengan acceso a la información pertinente a sus funciones, en caso de no requerir ese acceso, se les niegan los permisos completamente y se reduce significativamente el riesgo.

# Preguntas de reflexión

## ¿Cuál es la diferencia entre enmascaramiento y seudonimización?

- Enmascarmiento aplica una sustitución de los valores del dato almacenado, no es reversible ya que solo es una sustitución sobre los valores directamente. Mientras que la seudonimización sustituye el valor almacenado utilizando un seudónimo para el valor, el proceso para generar ese seudónimo puede variar pero debe estar referenciando al valor original y se puede revertir si se tiene acceso al mapa de seudónimos.

## ¿Por qué la seudonimización no significa anonimización?

- Porque la seudonimización sustituye el valor referenciando el valor original. En la anonimización por otro lado, se debe modificar el valor para que no sea identificable.

## ¿Por qué eliminar nombre y RFC no garantiza que un conjunto de datos sea anónimo?

- A pesar de que se eliminen esos datos se puede reidentificar un conjunto de datos mediante la combinación de otros valores identificadores, a pesar de no ser identificadores directos como lo pueden ser el nombre y el rfc.

## ¿Qué función tienen los cuasi-identificadores?

- No son identificadores directos, por lo que promueven la anonimización del conjunto a menos que se combinen con otros cuasi-identificadores.

## ¿Por qué es importante separar el mapa de seudonimización?

- Para que no se tenga acceso al mismo y no se pueda acceder a los valores referenciados originales.

## ¿Qué principio de seguridad se aplica al impedir que el analista acceda al mapa?

- Separación de funciones.

## ¿Por qué una vista puede ser preferible a entregar acceso directo a la tabla?

- Al no entregar acceso a la tabla eliminamos el riesgo de que el usuario modifique valores o los elimine.

## ¿Qué diferencia existe entre proteger un dato para visualización y protegerlo contra acceso no autorizado?

- Cuando se protege contra acceso no autorizado denegamos cualquier posibilidad de filtración o modificaión de los datos directa, si el rol no requiere el uso de esos datos es mejor negarlo directamente. En cambio cuando protegemos para visualización es porque el rol necesita acceso a los datos para cumplir sus funciones pero no debe acceder a la información sensible del conjunto de datos.

## ¿Por qué la retención forma parte de la protección de datos?

- Para asegurarse de que registros innecesarios no queden almacenados en la base de datos, reduciendo la superficie de ataque. A menos datos, menor peligro de reidentificación y menor peligro de filtraciones por negligencia, etc.

## ¿Qué riesgo existe si una organización conserva información indefinidamente?

- Puede exponerse a reidentificaciones, mientras más datos almacene, más sencillo sería hacer la relación entre valores; aumenta la carga de la base de datos, mayor probabilidad de filtraciones, riesgos legales.
