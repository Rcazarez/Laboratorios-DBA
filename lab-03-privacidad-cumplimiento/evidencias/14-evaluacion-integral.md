|Problema|Principio afectado|	Riesgo|	Control propuesto|
|--------|---------------|---------|--------------|
| Todos los usarios pueden consultar la tabla clientes |Control de acesos  |Filtración de datos |Limitar el acceso a ciertos usuarios|
|Los usuarios consultan directamente la tabla  | confidencialidad | Filtraciones | Crear una tabla clientes con los datos modificados para su analisis  |
|Los datos se conservan 12 años   | Politica de retencion |Sobrecarga de la base de datos con datos inútiles  |Realizar una eliminación periódica |  
| No existe una política documentada de retención |Política de retención  |Se eliminan datos sin tener un por qué o no se eliminan  |  Crear una política de retención y documentarla.|  
|Los desarrolladores reciben copias completas de la base de datos para realizar pruebas  |Privacidad por diseño  | Filtracion de datos |Crear bases de datos para uso de desarrollo  |  
|Las copias de desarrollo contienen información real.  |Minimizacion y confidencialidad  | Los desarrolladores accesan a la informacion personal del cliente |Compartir datos seudonimizados o falsos para el desarrollo  |  
|  El área de marketing utiliza los correos electrónicos para campañas promocionales|Privacidad y consentimiento |Correos no deseados de parte de la empresa para los usuarios  |consultar a los usuarios si quieren recibir correos promocionales |  
|No existe documentación clara sobre qué finalidad corresponde a cada dato.|Finalidad |Se almacenan datos innecesarios|Analizar la finalidad de los datos y documentarla|
|La tabla contiene más datos de los que el área de analítica necesita|Separacion por finalidad|El área tiene acceso a más información sobre los clientes de la que debería|Proporcionar solo los campos necesarios para el área|
|La empresa tiene una base de datos con información de 50,000 clientes y se comparte una copia con el equipo de desarrollo|minimizacion|Se crean copias innecesarias de un gran volumen de datos|Compartir tablas de prueba específicas para el área de desarrollo|
