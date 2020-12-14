#### Requisitos de Eficiencia

| **RNF 09** | Rastreo de contactos positivos |
| -- | -- |
| **[Versión]** | 1.0 (13/12/2020)|
| **[Dependencias]** | Este requisito depende del requisito general 1 (rastrear contactos entre positivos y gestionar la realización de pruebas médicas). Depende del erquisito de informacion 4 (Datos de localización de los ciudadanos), del requisito de conducta  (Rastreo de contactos positivos).  |
| **Descripción** | El sistema deberá de rasterar los contactos entre casos positivos en un tiempo no superior a 15 minutos en el 90% de los casos. |
| **[Importancia]** |Alta |
| **[Prioridad]** |Alta |
| **[Estado]** | Pendiente|
| **Comentarios** | Se ha establecido un tiempo limite de 15 para así dar tiempo al algoritmo a buscar los contactos de manera más efecetiva y con menor tasa de fallo dado el gran volumen de datos resulta un tiempo razonable. |

<p align="center"> <b>Tabla 16.9: Requisitos no funcionales del sistema</b> <br> </p>

| **RNF 10** | Generar informes |
| -- | -- |
| **[Versión]** | 1.0 (13/12/2020)|
| **[Dependencias]** | Este requisito depende del requisito general 3 (Gestionar información recopilada y proporcionar estadísticas al gobierno), del requisito de información 7 (Informe de las estadísticas generadas), requisito de reglas de negocio 1 (Cumplimiento de la Ley de protección de datos), requisito de reglas de negocio 2 (Adaptación de la información según la autonomía).  |
| **Descripción** | El sistema deberá generar informes con las estadísticas de los datos en un tiempo no superior a 30 minutos en el 80% de los casos. |
| **[Importancia]** |Alta |
| **[Prioridad]** |Alta |
| **[Estado]** | Pendiente|
| **Comentarios** |  Los informes generados son de vital importacia para el misnisterio, gobierno puedan tomar as decisiones correctas en bas a la situación e impacto actal del virus en una zona afectada. |

<p align="center"> <b>Tabla 16.10: Requisitos no funcionales del sistema</b> <br> </p>

| **RNF 11** | Enviar aviso incumplimiento cuarentena |
| -- | -- |
| **[Versión]** | 1.0 (13/12/2020)|
| **[Dependencias]** | Este requisito depende del requisito general 2 (Gestionar el cumplimiento de cuarentena), depende del requisito de conducta del sistema (Comprobar la ubicación del usario en cuarentena) |
| **Descripción** | El sistema deberá mandar un aviso del incumplimiento de la cuarentena a las autoridades en un tiempo inferior a 1 minuto desde que es detectado. |
| **[Importancia]** |Alta |
| **[Prioridad]** |Alta |
| **[Estado]** | Pendiente|
| **Comentarios** | Una vez no hemos asegurado que el ciudadano está ncumpliendo la cuarentena debemos enviar la alerta lo más rápido posible para que las fuerzas del orden tomen medidas nada más conocerse dicho incumplimiento. |

<p align="center"> <b>Tabla 16.11: Requisitos no funcionales del sistema</b> <br> </p>

| **RNF 12** | Tiempo de respuesta |
| -- | -- |
| **[Versión]** | 1.0 (13/12/2020)|
| **[Dependencias]** | Ninguna |
| **Descripción** | El sistema deberá tener un tiempo máximo de respuesta de 10 segundos para cualquier consulta que se realice en él. |
| **[Importancia]** |Alta |
| **[Prioridad]** |Alta |
| **[Estado]** | Pendiente|
| **Comentarios** | De cara a tener una experiencia como usuario fluida y agradable se busca que el resultado de las consultas no tarden demasiado, bien sea por la urgencia de obtener dichos datos como de evitar esperas incesesarias. |

#### Requisitos de seguridad

<p align="center"> <b>Tabla 16.12: Requisitos no funcionales del sistema</b> <br> </p>

| **RNF 17** | Autenticación de los usuarios |
| -- | -- |
| **[Versión]** | 1.0 (13/12/2020)|
| **[Dependencias]** | El requisito depende del requisito general gestionar información recopilada y proporcionar estadisticas al gobierno. |
| **Descripción** | El sistema deberá disponer de métodos de autenticación de los que dependerán las vistas a mostrar y la información a la que será accesible. |
| **[Importancia]** |Alta |
| **[Prioridad]** |Alta |
| **[Estado]** | Pendiente|
| **Comentarios** | Los datos de los ciudadanos serán visibles solo a quellos actores que esten autorizados y registrados en la aplicación. Una vez autenticados sabremos que tipo de actor esta accediendo a la aplicación, lo que nos determinará un sistema de vistas donde el actor podrá acceder a la información que se le esta permitido visualizar. |

<p align="center"> <b>Tabla 16.17: Requisitos no funcionales del sistema</b> <br> </p>

| **RNF 18** | Destruir información inservible del ciudadano |
| -- | -- |
| **[Versión]** | 1.0 (13/12/2020) |
| **[Dependencias]** | El requisito depende del requisito general gestionar información recopilada y proporcionar estadisticas al gobierno. También depende del requisito 1 de información (Datos de los ciudadanos), tambien en el requisito de Rastreo de contactos con positivo que en el caso de que el ciudadano de negativo en las pruebas se borrará de la lista que genera dicho requisito. Por otro lado depende del requisito de reglas de negocio 1 (Cumplimiento de la Ley de protección de datos).|
| **Descripción** | El sistema deberá destruir la información relativa al ciudadano una vez sea inservible para facilitar su uso y busqueda a la hora de crear listas o de generar notificaciones a los actores correspondientes. |
| **[Importancia]** | Alta |
| **[Prioridad]** | Media/Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | Este requisito es de vital importancia para evitar la saturación del sistema ya que contamos con un gran volumen de datos a manejar. Este requisito aumentara la organización y eficacia en la gestión de los datos de los ciudadanos. Tambien eliminando los datos  evitamos que alguien ajeno a la aplicación acceda a dichos datos. |

<p align="center"> <b>Tabla 16.18: Requisitos no funcionales del sistema</b> <br> </p>

| **RNF 19** | Anonimozar datos ciudadanos |
| -- | -- |
| **[Versión]** | 1.0 (13/12/2020) |
| **[Dependencias]** | El requisito depende del requisito general gestionar información recopilada y proporcionar estadisticas al gobierno, depende del requisito 1 de información (Datos de los ciudadanos). también depende del requisito de reglas de negocio 1 (Cumplimiento de la Ley de protección de datos) |
| **Descripción** | El sistema deberá anonimizar los datos de los ciudadanos a aquellos que no tengan la autorización. |
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | Como llevamos comentando a lo largo de la práctica, el hecho de poder acceder a los datos de los ciudadanos por las operadoras no obliga a gestionar dichos datos y evitar que sea visibles a agentes externos sin autorizar que podrían aprovecharse de estos. Además del derecho fundamental a la intimidad y de permanecer anónimo en la red. |

<p align="center"> <b>Tabla 16.19: Requisitos no funcionales del sistema</b> <br> </p>





