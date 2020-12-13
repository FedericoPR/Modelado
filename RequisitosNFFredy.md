#### Requisitos de Eficiencia

| **\<id>009** | Rastreo de contactos positivos |
| -- | -- |
| **[Versión]** | 1.0 (13/12/2020)|
| **[Dependencias]** |  |
| **Descripción** | El sistema deberá de rasterar los contactos entre casos positivos en un tiempo no superior a 15 minutos en el 90% de los casos. |
| **[Importancia]** |Alta |
| **[Prioridad]** |Alta |
| **[Estado]** | Pendiente|
| **Comentarios** |  |

<p align="center"> <b>Tabla 16.9: Requisitos no funcionales del sistema</b> <br> </p>

| **\<id>010** | Generar informes |
| -- | -- |
| **[Versión]** | 1.0 (13/12/2020)|
| **[Dependencias]** |  |
| **Descripción** | El sistema deberá generar informes con las estadísticas de los datos en un tiempo no superior a 30 minutos en el 80% de los casos. |
| **[Importancia]** |Alta |
| **[Prioridad]** |Alta |
| **[Estado]** | Pendiente|
| **Comentarios** |  |

<p align="center"> <b>Tabla 16.10: Requisitos no funcionales del sistema</b> <br> </p>

| **\<id>011** | Enviar aviso incumplimiento cuarentena |
| -- | -- |
| **[Versión]** | 1.0 (13/12/2020)|
| **[Dependencias]** |  |
| **Descripción** | El sistema deberá mandar un aviso del incumplimiento de la cuarentena a las autoridades en un tiempo inferior a 1 minuto desde que es detectado. |
| **[Importancia]** |Alta |
| **[Prioridad]** |Alta |
| **[Estado]** | Pendiente|
| **Comentarios** | Se considera que la frecuencia de realización de la copia de seguridad por parte de las bases de datos debe de ser de una hora, dado que se considera que como mucho se puedan perder los datos de nuevos positivos que se registren en el sistema en un periodo de tiempo de una hora. Los periodos de tiempo mayores a una hora se considera que son grandes pérdidas de información.|

<p align="center"> <b>Tabla 16.11: Requisitos no funcionales del sistema</b> <br> </p>

| **\<id>012** | Tiempo de respuesta |
| -- | -- |
| **[Versión]** | 1.0 (13/12/2020)|
| **[Dependencias]** |  |
| **Descripción** | El sistema deberá tener un tiempo máximo de respuesta de 10 segundos para cualquier consulta que se realice en él. |
| **[Importancia]** |Alta |
| **[Prioridad]** |Alta |
| **[Estado]** | Pendiente|
| **Comentarios** |  |

#### Requisitos de seguridad

<p align="center"> <b>Tabla 16.12: Requisitos no funcionales del sistema</b> <br> </p>

| **\<id>017** | Autenticación de los usuarios |
| -- | -- |
| **[Versión]** | 1.0 (13/12/2020)|
| **[Dependencias]** |  |
| **Descripción** | El sistema deberá disponer de métodos de autenticación de los que dependerán las vistas a mostrar y la información a la que será accesible. |
| **[Importancia]** |Alta |
| **[Prioridad]** |Alta |
| **[Estado]** | Pendiente|
| **Comentarios** | Se considera que la frecuencia de realización de la copia de seguridad por parte de las bases de datos debe de ser de una hora, dado que se considera que como mucho se puedan perder los datos de nuevos positivos que se registren en el sistema en un periodo de tiempo de una hora. Los periodos de tiempo mayores a una hora se considera que son grandes pérdidas de información.|

<p align="center"> <b>Tabla 16.17: Requisitos no funcionales del sistema</b> <br> </p>

| **\<id>018** | Destruir información inservible del ciudadano |
| -- | -- |
| **[Versión]** | 1.0 (13/12/2020) |
| **[Dependencias]** | El requisito depende del requisito general gestionar información recopilada y proporcionar estadisticas al gobierno. También depende del requisito 1 de información (Datos de los ciudadanos), tambien en el requisito de Rastreo de contactos con positivo que en el caso de que el ciudadano de negativo en las pruebas se borrará de la lista que genera dicho requisito. Por otro lado depende del requisito de reglas de negocio 1 (Cumplimiento de la Ley de protección de datos).|
| **Descripción** | El sistema deberá destruir la información relativa al ciudadano una vez sea inservible para facilitar su uso y busqueda a la hora de crear listas o de generar notificaciones a los actores correspondientes. |
| **[Importancia]** | Alta |
| **[Prioridad]** | Media/Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | Este requisito es de vital importancia para evitar la saturación del sistema ya que contamos con un gran volumen de datos a manejar. Este requisito aumentara la organización y eficacia en la gestión de los datos de los ciudadanos. Tambien eliminando los datos  evitamos que alguien ajeno a la aplicación acceda a dichos datos. |

<p align="center"> <b>Tabla 16.18: Requisitos no funcionales del sistema</b> <br> </p>

| **\<id>019** | Anonimozar datos ciudadanos |
| -- | -- |
| **[Versión]** | 1.0 (13/12/2020) |
| **[Dependencias]** | El requisito depende del requisito general gestionar información recopilada y proporcionar estadisticas al gobierno, depende del requisito 1 de información (Datos de los ciudadanos). también depende del requisito de reglas de negocio 1 (Cumplimiento de la Ley de protección de datos) |
| **Descripción** | El sistema deberá anonimizar los datos de los ciudadanos a aquellos que no tengan la autorización. |
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | Como llevamos comentando a lo largo de la práctica, el hecho de poder acceder a los datos de los ciudadanos por las operadoras no obliga a gestionar dichos datos y evitar que sea visibles a agentes externos sin autorizar que podrían aprovecharse de estos. Además del derecho fundamental a la intimidad y de permanecer anónimo en la red. |

<p align="center"> <b>Tabla 16.19: Requisitos no funcionales del sistema</b> <br> </p>





