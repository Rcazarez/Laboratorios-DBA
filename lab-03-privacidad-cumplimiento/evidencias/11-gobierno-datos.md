| Dato           | Finalidad | Responsable | Usuarios autorizados | Protección | Retención | Acción al finalizar |
|----------------|-----------|-------------|----------------------|------------|-----------|---------------------|
| nombre         |identificar al usuario|DBA|Atencion al cliente, facturacion, DBA|Encriptacion|Periodo de inactividad de 2 años|DELETE|
| correo         |Contacto con el usuario|DBA|Atencion al cliente, facturacion, Dirección, DBA|Enmascaramiento            |Periodo de inactividad de 2 años           |DELETE                       |
| telefono       |2do medio de contacto con el usuario|DBA|Atencion al cliente, facturacion, DBA|Enmascaramiento|Periodo de inactividad de 2 años| DELETE|
| rfc            |Procesos relacionados con facturacion|DBA|Facturacion, DBA                      |Enmascaramiento            |5 años|DELETE                     |
| edad           |Estadísticas y análisis|DBA|Analítica, Atención al cliente, DBA                       |Anonimizacion            |10 años           |Registros históricos|
| ciudad         |Análisis por localidades |DBA|Analítica|Anonimizacion            |3 años|anonimización general|
| codigo_postal  |Ubicacion apróximada de los clientes|DBA|Atencion al cliente, Analítica, DBA, Facturacion| anonimizacion            |Mientras la cuenta continue activa|DELETE|



