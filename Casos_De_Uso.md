### 6.2 Casos de uso del sistema:

En el siguiente apartado, se especificarán los distintos casos de uso del sistema. Se describirá como los usuarios utilizarán el sistema a desarrollar para llevar a cabo los procesos de negocio.Para ello se incluirá el diagrama de casos de uso, la especificación de los actores del sistema y la especificación de los casos de uso del sistema.

#### 6.2.1 Diagrama de casos de uso del sistema


#### 6.2.2 Especificación de actores del sistema
| **\<id>001** | Ciudadano |
| -- | -- |
| **[Versión]** | 1.0(04/12/2020) |
| **[Dependencias]** | Casos de uso en los que participa este actor:<br>   |
| **Descripción** | Este actor del sistema recibirá una salida por parte del sistema y no participará en los casos de uso es decir no tiene que interactuar con el sistema. Esto nos permite primero solventar la no obligatoriedad que comentamos en las debilidades y  Sin embargo como vemos en las dependencias, los casos de uso estarán condicionados a la información y el estado de este actor. |
| **Comentarios** | De la información obtenida por medio de los ciudadanos positivos, como la residencia, los puntos de visita frecuentes o las personas con las que ha mantenido contacto se sacan conclusiones por medio de su análisis que puedan dar lugar a toma de decisiones. |
<p align="center"> <b>Tabla 10.1: Actores del sistema.</b> </p>

| **\<id>002** | Autoridades |
| -- | -- |
| **[Versión]** | 1.0(04/12/2020) |
| **[Dependencias]** | Casos de uso en los que participa este actor:<br> |
| **Descripción** | Este actor recibirá del sistema los listados de aquellos ciudadanos que se encuentren en estado de cuarentena para así cuando les llegue una notificación por incumplimiento de esta, puedan actuar lo más rápido posible.|
| **Comentarios** | A este actor en determinadas ocasiones se les llama rastreadores, y llevaran a cabo la misión de rastrear el cómo se producen los contagios entre los positivos, asi como obtener cuales son los brotes de dichos contagios, para ello tan solo disponen de la información proporcionada por los pacientes positivos. |
<p align="center"> <b>Tabla 10.2: Actores del sistema.</b> </p>

| **\<id>003** | Gobierno |
| -- | -- |
| **[Versión]** | 1.0(04/12/2020) |
| **[Dependencias]** | Casos de uso en los que participa este actor:<br> |
| **Descripción** | Este actor de negocio actual representa al gobierno, en concreto al ministerio de sanidad y el comité de expertos, al que se le suministrarán todos los datos y estadísticas que se han obtenido por medio del procesamiento de los datos capturados de los ciudadanos y procesados por parte de nuestra plataforma pandemio. Dicho actor se encargará como entidad de tomar las decisiones oportunas en función de los datos suministrados por la plataforma, en base a diferentes criterios.
| **Comentarios** | El objetivo de nuestra plataforma es proporcionar los datos lo mejor procesados y "depurados" a este actor para que puedan tomar decisiones. |

<p align="center"> <b>Tabla 10.3: Actores del sistema</b> 

| **\<id>004** | Ambulatorio |
| -- | -- |
| **[Versión]** | 1.0(04/12/2020) |
| **[Dependencias]** |Casos de uso en los que participa este actor:<br> |
| **Descripción** | Este actor de negocio actual representa al centro de salud que dispondrá de listados donde se informarán del estado de los ciudadanos, así como de las distintas pruebas médicas que se les debe de realizar a cada uno de ellos. También se encargarán de notificar a los ciudadanos las citas en las que se les realizarán las pruebas, asi como las medidas que deben de tomar en caso de dar positivo y cual es la duración de la cuarentena que deben de cumplir.|
| **Comentarios** | Este actor podrá acceder a los datos de los ciudadanos (a sus datos médicos), también será el encargado de registrar el resultado de las pruebas realizadas a los ciudadanos en la plataforma pandemio, para que finalmente se pueda contabilizar dicho positivo y poder hacer un seguimiento de los contactos de dicho positivo, así como proporcionar los datos al gobierno. |

<p align="center"> <b>Tabla 10.4: Actores del sistema.</b> <br> </p>

| **\<id>005** | Compañia telefónica |
| -- | -- |
| **[Versión]** | 1.0(04/12/2020) |
| **[Dependencias]** |Casos de uso en los que participa este actor:<br> |
| **Descripción** | Este actor del sistema representa a las distintas compañias telefónicas de los ciudadanos, las cuales serán las encargadas de proporcionarnos los datos relativos a la localización de los ciudadadanos en los últimos 15 días para que se pueda procesar dichos datos por nuestro sistemas para rastrear los posibles contactos directos o los posibles focos de contagio.|
| **Comentarios** | Suponderemos que los datos proporcionados por este actor serán correctos y nuestra plataforma solo se preocupa de procesarlos, no de como se han de obtener por la compañias telefónicas.|

<p align="center"> <b>Tabla 10.5: Actores del sistema.</b> <br> </p>

#### 6.2.3 Especificación de casos de uso del sistema

En este apartado se especificarán los casos de uso del sistema a desarrollar identificados. Para ello se utilizará un nivel de detalle distinto dependiendo de la importancia de cada uno de los casos de uso. A continuación, se mostrará un listado de los casos de uso identificados en el sistema, divididos por subistemas.

* CASOS DE USO GENERALES AL SISTEMA: 
     * CU 0.1: Listar ciudadanos por estado.
     * CU 0.2: Informar al ciudadano. 

* SUBSISTEMA RASTREO DE CONTACTO ENTRE CASOS POSITIVOS Y GESTIÓN DE PRUEBAS MÉDICAS:
    * CU 1.1: Registrar ciudadano en el sistema.
    * CU 1.2: Registrar resultado de la prueba en el sistema.
    * CU 1.3: Rastrear contactos directos con el postivo.
    * CU 1.4: Adquirir datos de los ciudadanos.
    * CU 1.5: Registrar contactos directos en el sistema.
    * CU 1.6: Registrar cita pruebas en el sistema
    * CU 1.7: Enviar alerta a las autoridades de incumplmiento de realizarse la prueba
*  SUBSISTEMA GESTIÓN DEL CUMPLIMIENTO DE CUARENTENA:
    * CU 2.1: Control automático por el sistema del cumplimiento cuarentena.(Ciudadanos con móvil).
    * CU 2.2: Control humano por las autoridades (Ciudadanos sin móvil).
    * CU 2.3: Enviar alerta autoridades incumplimiento cuarentena.
* SUBSISTEMA GESTIÓN DE INFORMACIÓN Y ESTADÍSTICAS AL GOBIERNO:
    * CU 3.1: Informar caso positivo.
    * CU 3.2: Generar estadísticas.
    * CU 3.3: Informar estadísticas.
    * CU 3.4: Informar foco de contagio. 


A continuación, se especificarán aquellos casos de uso que hemos considerado de menor importancia para el sistema:

| **\<id> CU 0.1** | Listar ciudadanos por estado |
| -- | -- |
| **[Versión]** | 1.0 (04/12/2020) |
| **[Dependencias]** | Este caso de uso depende del CU 1.1 (Registrar ciudadano en el sistema) ya que necesita que recopilar la información de los ciudadanos ya registrados en el sistema que filtrará según su estado. Este caso de uso interactua con los actores ambulatorio y fuerzas del orden dado que estos podrán acceder a las listas creadas por el sistema. |
| **Precondición** | El sistema debe tener ciudadanos ya registrados con sus respectivos datos |
| **Descripción** | El sistema deberá recopilar la información de los ciudadanos en forma de listas que iran filtradas por el estado de los ciudadanos. Es de vital importancia pues será la base para gestionar los procesos y decisiones que deberán tomar los actores relacionados con la salida de este caso de uso ya que el conocimiento del estado de los ciudadanos nos dará perspectiva a la hora de tomar acción. |
| **Postcondición** | Se habran creado una lista de todos los ciudadanos registrados según su estado, esta información será accesible tanto para los ambulatorios como para las fuerzas del orden. |
| **[Importancia]** | Muy alta |
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | Debemos tener siempre encuenta la enorme catidad de datos que maneja este caso de uso como explicamos en las debilidades. Ya que una mala gestión del flujo de datos afectaría a la efectividad y no tendriamos en estas listas un fiel reflejo de la situación actual lo que derivaría en no poder tomar la decisión óptima. |

<p align="center"> <b>Tabla 11.1: Plantilla simplificada de Casos de Uso.</b> <br> </p>

| **\<id> CU 0.2** | Informar al ciudadano |
| -- | -- |
| **[Versión]** | 1.0 (04/12/2020) |
| **[Dependencias]** | Este caso de uso depende del CU 1.2 (Registrar resultado de la prueba en el sistema) ya que si el ciudadano da positivo, el sistema notificará este para que sepa que pasos debe realizar, si se debe realizar alguna otra prueba o  iniciar el CU 2.1 o bien el CU 2.2 para llevar acabo el control del cumplimiento del periodo de cuarentena. |
| **Precondición** | El ciudadano tiene que estar registrado en el sistema ya que se debe obtener su numero de télefono para así contactar con la mayor rapidez posible.|
| **Descripción** | El sistema debera notificar al ciudadano de que precauciones debe tomar y que pasos a seguir si debe cumplir el periodo de cuarentena o realizar alguna prueba médica. Cuanta más completa sea la información mejor reaccionará el ciudadano y será menos propenso a cometer cualquier error que pueda poner en riesgo a sí mismo y a los que le rodean.|
| **Postcondición** | El ciudadano tendrá instrucciones claras de como debe proceder en caso de tener que realizarse una prueba médica o de cumplir el periodo de cuarentena establecido. |
| **[Importancia]** | Muy alta |
| **[Prioridad]** | alta |
| **[Estado]** | Pendiente |
| **Comentarios** | Aunque no necesitemos de la intervención del ciudadano en el sistema es muy importante que esté bien informado dado que todo gira en torno a su bienestar y salud. |

<p align="center"> <b>Tabla 11.2: Plantilla simplificada de Casos de Uso.</b> <br> </p>

| **\<id> CU 1.1** | Registrar ciudadano en el sistema |
| -- | -- |
| **[Versión]** | 1.0 (04/12/2020) |
| **[Dependencias]** | Este caso de uso depende del CU 1.6 (Registrar cita pruebas en el sistema) ya que un ciudadano sospechoso de tener el virus debe realizarse una prueba por lo que se debe guardar información sobre él en caso de que diera un resultado positivo. Lo que iniciaria el CU 0.1 (Listar ciudadanos por estado) con los datos que proporciona este caso de uso con la información del ciudadano y estado. En este caso de uso interactutuará con el actor ambulatorio que tendrá permiso para introducir la información necesaria del ciudadano al sistema. |
| **Precondición** | El usuario debe presentar sintomas de la enfermedad para así considerarlo caso sospechoso y empezar el seguimiento de su situación. |
| **Descripción** | Este caso de uso supone el inicio del proceso de seguimiento de un ciudadano del cual se sospecha que tenga la enfermedad, para tener disponibe su información y poder contactar rapidaente con dicho ciudadano en caso de dar positivo, asi como poder almacenarlo en nuestros listados de ciudadanos por estado. La información del ciudadano tras su resgistro se considerá vital para el funcionamiento del sistema en cuanto a generar estadisticas estadisticas y dar su acceso a aquellosactores autorizados ..  |
| **Postcondición** | Habrá un nuevo ciudadano registrado en el sistema con sus correspondientes datos. |
| **[Importancia]** | Muy Alta> |
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | La información del ciudadano registrado es únicamente accesible a los actores autorizados de cara a proteger su privacidad y que agentes externos no se puedan aprovechar de dichos datos |

<p align="center"> <b>Tabla 11.3: Plantilla simplificada de Casos de Uso.</b> <br> </p>

| **CU 1.4** | Adquirir datos de los ciudadanos |
| -- | -- |
| **[Versión]** | 1.0 (04/12/2020) |
| **[Dependencias]** |  |
| **Precondicion** | Las operadoras deberán tener acceso al sistema para poder suministrar los datos de los cuidadanos o bien el administrador del sistema los recibirá de las operadoras y los incorporará al sistema  |
| **Descripción** | Este caso de uso consiste en el aporte de todos los datos de los cuidadanos por parte de la operadora telefónica. Más adelante estos datos serán imprescindibles para hacer el rastreo de los posibles contactos |
| **Postcondicion** | Los datos de los cuidadanos quedarán reflejados en el sitema de manera que puedan ser utilizados por los algoritmos para poder realizar los cruces de información y rastrear los posibles contagiados |
| **[Importancia]** | Muy Alta |
| **[Prioridad]** | Alta |
| **Estado** |  |
| **Comentarios** | Debido a la importancia de esta información para poder realizar la mayor parte de las funciones del sistema esta deberá estar lo más actualizada posbible. Por ello el encargado de administrar esta información para el sistema deberá actualizar la misma con mucha frecuencia |

| **CU 1.5** | Registrar contactos directos en el sistema |
| -- | -- |
| **[Versión]** | 1.0 (04/12/2020) |
| **[Dependencias]** |  |
| **Precondicion** | El ciudadano a registrar habrá sido identificado anteriormente por el algoritmo como posible positivo |
| **Descripción** | Una vez el algoritmo nos proporciona aquellos ciudadanos que han tenido contacto suficiente con un positivo y, por tanto, son susceptibles de ser positivos pasaremos a registrar a estos ciudadanos en el sistema. En este primer registro se pondrá al ciudadano con el estado "Pendiente de cita" para que el responsable del ambulatorio sepa que deberá concretar una cita con él para realizarse las pruebas pertinentes |
| **Postcondicion** | El ciudadano quedará registrado en el sistema como pendiente de concretar una cita lo antes posible para realizarse las puebas y se le inromará de que deberá guardar cuarentena haste ese momento|
| **[Importancia]** | Alta |
| **[Prioridad]** | Media |
| **Estado** |  |
| **Comentarios** | Una vez se guarda el cuidadano como posible positivo los responsables de llamarlo y concretar cita deberán intentar que esa cita para la realización de las pruebas no tarde para ser lo más eficientes posibles en evitar la propagación de un usuario que puede que esté contagiado|

| **CU 1.6** | Registrar cita pruebas en el sistema |
| -- | -- |
| **[Versión]** | 1.0 (04/12/2020) |
| **[Dependencias]** |  |
| **Precondicion** | El usuario debe haber sido detectado por el algoritmo y registrado en el sistema para que aparezca como pendiente de cita al filtrar para que el ambulatorio se ponga en contacto |
| **Descripción** | Tras haber detectado un posible positivo con los datos de rastreo por parte del algoritmo y haber sido registrado el usuario en el sistema, el responsable sanitario del ambulatorio al que pertenece el cuidadano se pondrá en contacto con él para concretatar la cita en la que se le realizarán las pruebas. Una vez se concrete la cita el responsable lo registrará en el sistema|
| **Postcondicion** | El usuario quedará como pendiente de realizar las pruebas y se le infromará de que permanezca en cuarentena hasta la realización de las mismas. Esta cuarentena no será controlada por las fuerzas de seguridad debido a que no se trata de un positivo confirmado por lo que se intentará dar la cita lo antes posible |
| **[Importancia]** | Alta |
| **[Prioridad]** | Media |
| **Estado** |  |
| **Comentarios** | |

| **CU 1.7** | Enviar alerta a las autoridades de incumplmiento de realizarse la prueba|
| -- | -- |
| **[Versión]** | 1.0 (04/12/2020) |
| **[Dependencias]** |  |
| **Precondicion** | La fecha de cita deberá ser 24 h inferior a la fecha actual para que se alerte a las autoridades |
| **Descripción** | Una vez se registra una cita para el ciudadano, este deberá acudir en el día y la hora previstas para la realización de la prueba. En caso de no acudir a la cita el sistema alertará al usuario de que no se ha ralizado la prueba en la cita que se registró y que dispone de 24 h para volver a llamar en vistas a explicar su situación y/o los motivos por los cuales no ha acudido así como para coincretar una nueva cita. En caso de que finalice este plazo de 24 h y el ciudadano no se haya puesto en contacto para acordar una nueva cita, es decir, el registro siga teniendo una fecha de cita que ha vencido hace más de 24 h, el sistema de manera automática enviará otro mensaje al cuidadano y tambén alertará a las fuerzas del orden de esta situación de incumplimiento por parte del ciudadano. |
| **Postcondicion** | La fecha de cita seguirá siendo una fecha pasada hasta aclarar la situación por parte de las autoridades |
| **[Importancia]** | Media |
| **[Prioridad]** | Media |
| **Estado** |  |
| **Comentarios** | Si el usuario llamara para cambiar la cita pasadas 24 horas, bien por actuación de las autoridades, o bien por descuido personal durante las 24 h de plazo, las autoridades serían informadas también|

| **\<id> CU 2.2** | Control humano por las autoridades (Ciudadanos sin móvil) |
| -- | -- |
| **[Versión]** | 1.0(04/12/2020) |
| **[Dependencias]** |Este caso de uso depende del CU 0.1 (Listar ciudadanos por estado), ya que debe de incluir dicho caso de uso. Dicho caso de uso interactua con el actor autoridades y el actor ciudadano. Ya que por medio de este caso se llevará un control por parte de las autoridades sobre el ciudadano.|
| **Precondición** | En el sistema se encuentra registrado un ciudadano que debe de cumplir cuarentena y no dispone de teléfono móvil. |
| **Descripción** | Los agentes de la autoridad podrán realizar un listado de los ciudadanos registrados en el sistema cuyo estado sea en cuarentena y sin teléfono móvil (CU 0.1 Listar ciudadanos por estado). De esta forma de obtendrá el listado de todos aquellos ciudadanos a los cuales no se les puede realizar un control del cumplimiento de la cuarentena de forma automática por el sistema. Por lo que será responsabilidad de los agentes de la autoridad llevar a cabo un control de la cuarenta de esta parte de la población, para ello realizará controles aleatorios en los domicilios de estos ciudadanos comprobando de que se encuentren en casa cumpliendo la cuarentena, en caso de que no se cumpla actuarán en consecuencia.|
| **Postcondición** | Se comprobará si se está llevando a cabo la cuarentena por el ciudadano.|
| **[Importancia]** | Media|
| **[Prioridad]** | Media|
| **[Estado]** | Pendiente|
| **Comentarios** |Este caso de uso solo afectará al pequeño porcentaje del 10% de la población española que no disponde de teléfono móvil y que enla mayoría de los casos se corresponde con personas mayores o ancianos.|

<p align="center"> <b>Tabla 11.2.2: Plantilla simplificada de casos de uso.</b> <br> </p>

| **\<id> CU 2.3** | Enviar alerta autoridades incumplimiento cuarentena. |
| -- | -- |
| **[Versión]** | 1.0(04/12/2020) |
| **[Dependencias]** |Este caso de uso depende del CU 2.1 (Control automático por el sistema del cumplimiento cuarentena.(Ciudadanos con móvil)), ya que si se detecta alguna anomalía en dicho caso de uso se dispararía este caso de uso, y también depende del CU 0.2 (Informar al ciudadano) cuando se detecte esa anomalía. Dicho caso de uso interactua con el actor autoridades. Ya que por medio de este caso se informará a las autoridades de que ha ocurrido un evento.|
| **Precondición** | Un cidadano con móvil que debe de cumplir la cuarentena no la está cumpliendo y es detectado por el sistema (CU 2.1 Control automático por el sistema del cumplimiento cuarentena.(Ciudadanos con móvil)) |
| **Descripción** | Dicho caso de uso es disparado cuando el CU 2.1 (Control automático por el sistema del cumplimiento cuarentena.(Ciudadanos con móvil)), detecta que un ciudadano con móvil no se encuentra en su domicilio cumpliendo con la cuarentena obligatoria. En esta situación, el sistema enviará un mensaje de alerta a la autoridades informándolas de que un ciudadano no está cumpliendo con la cuarentena, proporcionando toda la información disponible del ciudadano, incluyendo la ubicación de su dispositivo móvil para que pueda ser localizado por los agentes (siempre y cuando el móvil del ciudadano no se encuentre en su casa), de esta forma los agentes de la autoridad actuarán en consecuencia localizando al ciudadano. Al mismo tiempo de que se envía la alerta a las autoridades, se dispara el CU 0.2 (Informar al ciudadano), informándole por medio de un SMS de que no está cumpliendo la cuarentena y ha sido avisado a la autoridad.|
| **Postcondición** | Las autoridades habrán recibido una alerta sobre el incumplimiento de la cuarentena, con la información del ciudadano y el ciudadano habrá sido informado de ello.|
| **[Importancia]** | Alta|
| **[Prioridad]** | Alta|
| **[Estado]** | Pendiente|
| **Comentarios** |El como se deberá actuar para localizar al ciudadano que no cumple la cuarentena es competencia de las autoridades responsables.|

<p align="center"> <b>Tabla 11.2.3: Plantilla simplificada de casos de uso.</b> <br> </p>

| **\<id> CU 3.1** | Informar caso positivo. |
| -- | -- |
| **[Versión]** | 1.0(04/12/2020) |
| **[Dependencias]** |Este caso de uso depende del CU 1.2 (Registrar resultado de la prueba en el sistema) y que dicho resultado sea positivo, ya que si se detecta algun nuevo caso positivo se dispararía este caso de uso. Dicho caso de uso interactua con el actor Gobierno, ya que por medio de este caso se informará al gobierno de la ocurrencia de un nuevo caso positivo .|
| **Precondición** | Un ciudadano ha dado positivo en la prueba realizada. |
| **Descripción** | Dicho caso de uso es disparado cuando el CU 1.2 (Registrar resultado de la prueba en el sistema) registra una prueba que ha sido positiva. En esta situación, el sistema añadirá un nuevo caso positivo a un contador de casos positivos por centro de salud (en el contador correspondiente al centro de salud donde se ha detectado el caso positivo), dicha información con los contadores de casos positivos por centro de salud será siempre accesible por el gobierno, para que pueda ser consultada en cualquier momento y se conozca la información en tiempo real.|
| **Postcondición** | Se habrá registrado el caso postivo en el sistema de contadores de casos positivos por centro de salud al que puede acceder el gobierno.|
| **[Importancia]** | Alta|
| **[Prioridad]** | Alta|
| **[Estado]** | Pendiente|
| **Comentarios** |Dicha información será actualizada constantemente, cada vez que un nuevo caso positivo es registrado en el sistema, a diferencia del CU 3.3 (Informar estadísticas), las cuales serán proporcionadas al gobierno de forma periódica cada 3 días o el tiempo fijado.|

<p align="center"> <b>Tabla 11.3.1: Plantilla simplificada de casos de uso.</b> <br> </p>

| **\<id> CU 3.3** | Informar estadísticas |
| -- | -- |
| **[Versión]** | 1.0(05/12/2020) |
| **[Dependencias]** |Este caso de uso depende del CU 3.2 (Generar estadísticas) ya que antes de poder informar las estadísitcas deben de ser generadas (dependencia de tipo include). Dicho caso de uso interactua con el actor Gobierno, ya que por medio de este caso se informará al gobierno de las estadísitcas generadas por el sistema .|
| **Precondición** | El sistema ha generado estadísticas a partir de los datos que dispone. CU 3.2 (Generar estadísticas) |
| **Descripción** | Dicho caso de uso es disparado cuando el CU 3.2 (Generar estadíticas) genera nuevas estadísticas a partir de los datos disponibles en el sistema. En esta situación, el sistema mostrará un informe estadístico con todas las estadísticas obtenidas en el CU 3.2 y se enviará un aviso al sistema del gobierno informándole de que están disponibles nuevas estadísiticas obtenidas a partir de los datos recopliados en los últimos 3 días o el tiempo marcado, para que las pueda visualizar en el sistema y a partir de ellas, el comité de expertos del gobierno puedan tomas las decisiones oportunas.|
| **Postcondición** | Se habrán proporcionado las estadísticas al gobierno y se le habrá mandado un aviso para que puedan visualizarlas en el sistema.|
| **[Importancia]** |Muy Alta|
| **[Prioridad]** | Alta|
| **[Estado]** | Pendiente|
| **Comentarios** |La información relevante a las estadísitcas será proporcionada al gobierno de forma periódica cada 3 días o el tiempo fijado. Dado que se necesita disponer de un gran volumen de datos recopilados durante varios dias para que dichas estadísticas sean lo mas fiables posibles.|

<p align="center"> <b>Tabla 11.3.3: Plantilla simplificada de casos de uso.</b> <br> </p>

| **CU 3.4** | Informar foco de contagio |
| -- | -- |
| **[Versión]** | 1.0 (04/12/2020) |
| **[Dependencias]** |  |
| **Precondicion** | Una vez se confirme un contagiado pos otro positivo, por medio de los datos de localizacion estableceremos cual ha sido el punto más probable donde se ha producido el contagio, en caso de haber más de uno. |
| **Descripción** | Con todos los datos de los que el sistema dispone, de contagios, lugar donde se produce el contagio, número de contagios...etc por medio de algoritmos generará una serie de estadísticas que nos permitiran averiguar cuales son los lugares donde más se contagian los ciudadanos. Cuando estos valores lleguen a ciertos parámetros previamente establecidos etiquetaremos este lugar como "foco de conagio" del cual se informará al gobierno para que tome las medidas oportunas|
| **Postcondicion** | Una vez se llegue a ciertos valores de numero de contagiados en una zona supondrá informar de esta situación al gobierno |
| **[Importancia]** | Alta |
| **[Prioridad]** | Media |
| **Estado** |  |
| **Comentarios** | |

A continuacion se especificarán de forma mas detallada aquellos casos de uso que tengan mayor relevancia en el sistema por medio de las siguientes tablas:

| **\<id> CU 1.2** | Registrar resultado de la prueba en el sistema |  |
| --- | --- | --- |
| **[Versión]** | 1.0 (05/12/2020) |
| **[Dependencias]** | Este caso de uso depende del CU 1.3 (Rastrear contactos directos con el postivo) que será necesario para poder llevar a cabo el CU 1.6 (Registrar cita pruebas en el sistema), de dichas citas se realizarán las pruebas pertinentes al ciudadano.  Este caso de uso  será el inicio del CU  3.1 (Registrar cita pruebas en el sistema) en caso de que las pruebas den positivo. Así como del CU 0.2 (Informar al ciudadano) notificandole a este el resultado de la prueba.|
| **Precondición** | La prueba ha sido realizada al ciudadano en la cita acordada. |
| **Descripción** | El sistema deberá almacenar los resultados de las pruebas realizadas a los ciudadanos, lo que ejecutará los procesos necesarios para saber si debemos iniciar un seguimiento del paciente en caso de tener la enfermedad. Basicamente informa a los distintos procesos de nuestro sistema el estado del ciudadano de cara  |
| **Secuencia Normal** | **Paso** | **Acción** |
|  | 1 |  El responsable del ambulatorio solicitará los resultados del ciudadano al que se le ha realizado la prueba  |
|  | 2 | El sistema devuelve los resultados de dicha prueba. |
|  | 3 | Si el resultado es positivo en coronavirus |
|  | 4 | Se inicia el CU 1.1 (Registrar ciudadano en el sistema) |
|  | 5 | Se inicia el CU 0.2 (Informar al ciudadano) |
|  | 6 | {El caso de uso termina con éxito} |
| **Postcondición** | El resultado de la prueba realizada se almacenará en el sistema. |
| **Excepciones** | **Paso** | **Acción** |
|  | 1 | Si el resultado de la prueba es negativo |
|  | 2 | El ambulatorio registrara al ciudadano como caso no positivo en las listas de estado del sistema.  |
|  | 3 | Se inicia el CU 0.2 (Informar al ciudadano) pero en este caso se le dira que no tiene coronavirus y que no debe cumplir la cuarentena. |
|  | 4 | El caso de uso termina |
| **Rendimiento** | **Paso** | **Cota de tiempo** |
| | q | k\<unidad de tiempo> no se| 
| **Frecuencia** | \<nº veces / unidad de tiempo> no se|
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** |  |
<p align="center"> <b>Tabla 12: Plantilla Completa de Casos de Uso.</b> <br> </p>

| **\<id> CU 1.3** | Rastrear contactos directos con el postivo |  |
| --- | --- | --- |
| **[Versión]** | 1.0 (09/12/2020)|
| **[Dependencias]** | Dicho caso de uso depende del CU 1.2 (Registrar resultado de la prueba en el sistema) para alertar al sistema de que se ha detectado un positivo y de que deberá utilizar los datos de los que dispone para identificar aquellos ciudadasno que puedan haber contactado lo suficiente con el postitivo. También depende del CU 1.4 (Adquirir datos de los ciudadanos), ya que necesitará de todos los datos de localización de los ciudadanos para que el algoritmo pueda realizar los cruces e identificar los ciudadanos susceptibles de haber sido contagiados|
| **Precondición** | En el sisteme deben estar los datos de los ciudadanos suministrados por las operadoras y deberá saltar un caso positivo para que el sistema empiece a trabajar en los rastreos|
| **Descripción** |  Una vez se registra un positivo en la pruebas realizadas a algún ciudadano, este resultado es introducido en el sistema. En ese momento el algoritmo de rastreo comenzará su trabajo. Para ello tendrá en cuenta y trabajará con todos los datos previamente suministrados por las operadoras móviles, cotejará y contrastará las ubicaciones de los ciudadanos que coincidan en lugar y momento con las del postivo para establecer cuales de ellos pueden haber sido contagiados por cumplir los parámetros de contacto necesarios para contagiarse. Cuando el sistema concluye su análisis suministrará los datos de aquellos ciudadanos que puedan ser positivos y para que sean registrados en el sistema como pendientes de realizar la prueba junto con  el lugar donde es más probable que se haya producido el contagio, para tenerlo en cuenta en las estadísticas. Una vez loa ambulatorios dispongan de los datos aportados por este rastreo comenzarán a informar a los cuidadanos de su situación y a concretar citas con los mismos|
| **Secuencia Normal** | **Paso** | **Acción** |
|  | 1 | El sistema detectará que se ha introducido un nuevo positivo en el sistema y comenzará el rastreo con respecto a él CU 1.2 (Registrar resultado de la prueba en el sistema) |
|  | 2 | El algoritmo detectará aquellos cuidadanos que puedan estar infectados teniendo en cuenta los datos de las operadoras CU 1.4 (Adquirir datos de los ciudadanos) |
|  | 3 | El sistema elaborará una lista de los cuidadanos que ha detectado para que se registren en el sistema así como el punto de contagio y los ambulatorios registrarán estos datos CU 1.1(Registrar resultado de la prueba en el sistema) |
|  | 4 | Los ambulatorios se encargarán de ponerse en contacto con los posibles positivos para concretar con ellos una cita en la cual realizarse la pureba CU 1.6 (Registrar cita pruebas en el sistema) que en caso de dar positivo empezaría de nuevo el caso de uso que se está tratando (CU 1.3 "Rastrear contactos directos con el postivo") |
| **Postcondición** | El sistema registrará todos los cuidadanos que puedan haber sido contagiados para que se les realicen las pruebas y continuará con el ciclo en cada uno de los postivos encontrados de esta manera |
| **Excepciones** | **Paso** | **Acción** |
|  | 1 | El sistema identificará en el rastreo aquellos cuidadanos a los cuales se ha establecido como positivos una única vez para no caer en bucles infinitos de positivos|
| **Rendimiento** | **Paso** | **Cota de tiempo** |
| | El rastreo como tal de cuidadanos que pueden estar contagiados no debe de tardar en ser ejecutado un tiempo superior a 100 segundos, que es bastante tiempo pero es un porceso muy complejo y seguramente el más importante del poryecto por lo que es mejor que sea preciso en sacrificio de su rapidez | 1'40''|
| **Frecuencia** | El CU debe de llevarse a cabo cada vez que se registre un positivo en el sistema|
| **[Importancia]** | Muy Alta|
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** ||

| **\<id> CU 2.1** | Control automático por el sistema del cumplimiento cuarentena.(Ciudadanos con móvil). |  |
| --- | --- | --- |
| **[Versión]** | 1.0 (05/12/2020)|
| **[Dependencias]** | Dicho caso de uso depende del CU 0.2 (Listar ciudadanos por estado) para obtener aquellos ciudadanos registrados en el sistema que deben de cumplir cuarentena. También depende del CU 2.3 (Enviar alerta autoridades incumplimiento cuarentena), ya que cuando se detecte un ciudadano que no está cumpliendo la cuarentena se informará a las autoridades. Este caso de uso deberá interactuar con las operadoras teléfonicas para poder obtener la localización en tiempo real del dispositivo móvil del ciudadano.|
| **Precondición** | En el sistema se encuentra registrado un ciudadano que debe de cumplir cuarentena y dispone de teléfono móvil.|
| **Descripción** | El sistema será capaz de detectar cuando un ciudadano que dispone de teléfono móvil esta incumpliendo la cuarentena, en dicho caso lo informará a las autoridades para que actuen en consecuencia.  |
| **Secuencia Normal** | **Paso** | **Acción** |
|  | 1 | El sistema obtendrá un listado con los ciudadanos que deban cumplir cuarentena y dispongan de teléfono móvil con desbloqueo por huella dactilar. CU 0.1 (Listar ciudadanos por estado). |
|  | 2 | Cada 10 minutos el sistema debe de hacer un sondeo, solicitando la localización del dispositivo del ciudadano a las operadoras telefónicas. Si la localización del dispostivo del ciudadano es distinta a la del domicilio del ciudadano se disparará el CU 2.3 (enviar alerta a las autoridades), y se informará al ciudadano de ello, y terminaría el CU. En caso contrario, se continuaría con el flujo normal del CU. |
|  | 3 | El sistema enviará en un periodo de tiempo aleatorio desbloquear el móvil al ciudadano por medio de la huella dactilar y al hacerlo se tomará una foto del ciudadano. |
|  | 4 | Si pasada una hora el ciudadano no desbloquea el teléfono móvil, se disparará el CU 2.3 (enviar alerta a las autoridades) y termina el CU actual. En caso contrario si se desbloquea el móvil se comprobará que la foto tomada al desbloquear el móvil se corresponde al ciudadano (sistema de reconocimiento facial) y se comprobará que el dispositivo se encuentra en el domicilio del ciudadano. |
|  | 5 | El sistema reconoce que el ciudadano se encuentra en su domicilio cumpliendo la cuarentena y termina. |
| **Postcondición** | El sistema habrá comprobado que el ciudadano se encuentra en casa cumpliendo la cuarentena y en caso contrario se habrá disparado el CU 2.3 (enviar alerta a las autoridades) para que actuen en consecuencia. |
| **Excepciones** | **Paso** | **Acción** |
|  | 1 | El sistema actuará de distinta forma si los ciudadanos que deben cumplir cuarentena disponen de teléfono móvil sin desbloqueo por huella dactilar.En este caso un agente de la autoridad realizará una videollamada con el ciudadano comprobando que es el, y se obtendrá la localización del teléfono móvil en ese momento. En caso de que no se corresponda con el ciudadano, o el ciudadano no responda a la llamada en un máximo de una hora, o el teléfono del ciudadano no se encuentra en su domicilio se disparará el CU 2.3|
| **Rendimiento** | **Paso** | **Cota de tiempo** |
| | El CU no debe de tardar en ser ejecutado un tiempo superior a  |10 segundos|
| **Frecuencia** | El CU debe de llevarse a cabo de forma constante en segundo plano, realizando sondeos cada 10 minutos de la localización de los teléfonos de los ciudadanos comprobando que se encuentra en su domicilio, o cada un periodo de tiempo aleatorio, se debe de pedir desbloquear el teléfono móvil del ciudadano.|
| **[Importancia]** | Muy Alta|
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | El CU afecta al 90% la población española que dispone de teléfono móvil. Dicho caso de uso es complemenatario al CU 2.2 Control humano por las autoridades (Ciudadanos sin móvil), el cual solo afecta a la población que no posee teléfono móvil.|
<p align="center"> <b>Tabla 12.2.1: Plantilla Completa de Casos de Uso.</b> <br> </p>

| **\<id> CU 3.2** | Generar estadísticas |  |
| --- | --- | --- |
| **[Versión]** | 1.0 (05/12/2020)|
| **[Dependencias]** | Dicho caso de uso depende del CU 1.2 (Registrar resultado de la prueba en el sistema) y el resultado es positivo. También depende del CU 1.3 ( Rastrear contactos directos con el postivo), ya que a partir de la información proporcionada por dichos casos de uso, el caso de uso generar estadísticas podrá obtener las estadísitcas sobre la población. De este caso de uso también depende el CU 3.3 (Informar estadísticas), dado que una vez que se han obtenido las estadísitcas, se disparará el CU 3.3.|
| **Precondición** | El sistema dispone de los datos de los casos positivos y de los contactos directos entre los positivos.|
| **Descripción** | El sistema deberá obtener estadísitcas a cerca de los contagios producidos, detectando los posibles focos de contagio entre los ciudadanos, las zonas que se encuentran más expuestas al virus, la población más proprensa a ser contagiada, etc para que se pueda disparar el CU 3.3 y se informen de todas estas estadísticas al comité de expertos del gobierno para que tomen las medidas necesarias. |
| **Secuencia Normal** | **Paso** | **Acción** |
|  | 1 | El sistema consultará los datos de los casos positivos registrados. |
|  | 2 | El sistema consultará los datos relativos a los contactos directos entre los casos positivos y si estos han sido positivos. |
|  | 3 | El sistema consultará el lugar donde se han producido los contactos entre los contagiados.|
|  | 4 | El sistema aplicará un algoritmo inteligente para obtener relaciones entre los contagios, los lugares de contagio, etc cruzando los datos para obtener las estadísticas oportunas. |
|  | 5 | Se almacenan en el sistema las estadísticas obtenidas como un informe al que podrá acceder el gobierno. |
|  | 6 | Se dispara el CU 3.3 (Informar estadísticas) |
|  | 7 | Se dispara el CU 3.4 (Informar foco de contagio) |
| **Postcondición** | El sistema habrá generado estadísticas a partir de los datos de contagios y contactos que disponía, detectando posibles focos de contagio, zonas más expuestas al virus, población más propensa a ser contagiada,etc. |
| **Excepciones** | **Paso** | **Acción** |
|  | 2 | Si el caso positivo registrado es un caso aislado, se comtabilizará en las estadísticas como un caso aislado.|
| **Rendimiento** | **Paso** | **Cota de tiempo** |
| | El CU debe de llevarse a cabo en un tiempo no superior a|1 hora|
| **Frecuencia** | El CU debe de llevarse a cabo una vez cada 3 días.|
| **[Importancia]** | Muy Alta|
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | El CU debe de realizarse con poca fecuencia para que las estadísticas obtenidas sean lo mas reales posibles obtenidas de grandes volúmenes de datos, por ello mismo el tiempo que implica llevar a cabo el caso de uso es grande. |
<p align="center"> <b>Tabla 12.3.2: Plantilla Completa de Casos de Uso.</b> <br> </p>