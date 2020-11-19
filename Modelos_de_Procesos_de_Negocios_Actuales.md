# 3.2 Modelos de Procesos de Negocios Actuales

En este apartado representaremos y describiremos todos aquellos procesos que se llevarán acabo para gestionar los contagios que se producen en la pandemia, asi como los procesos que se emplearán para controlar el cumplimiento de la cuarentena obligatoria por parte de los ciudadanos positivos. También se tendrán en cuenta todos aquellos procesos en los que se gestionen las distintas pruebas médicas que se deben realizar los ciudadanos, asi como informales a estos de los resultados.Por otro lado, se especificará como debe ser la comunicación con el resto de actores que intervienen en la plataforma como los agentes de la autoridad o el gobierno al que se le proporcionarán todos los datos obtenidos con la plataforma para que puedan tomarse las medidas oportunas por parte de los expertos correspondientes.

## 3.2.1 Descripción de los Actores de Negocio Actuales

Los actores de negocio de nuestra aplicación o toda aquella persona interesada en está serán: ciudadanos, gobierno, autoridades y ambulatorios. Necesarios para que la información se transmita de manera segura.

| **\<id>1** | Ciudadano |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | * \<procesos de negocio actuales en los que participa> <br> * ... |
| **Descripción** | Este actor de negocio actual es el actor principal de la plataforma y representa a cada uno de los ciudadanos, de dicho actor se van a obtener todos los datos que se gestionarán por medio de la plataforma. De ellos por medio de sus dispositivos móviles, se va a poder acceder a cual ha sido su localización, las personas con las que ha estado en contacto, el tiempo que ha permanecido en un determinado lugar, etc. Toda esta información será procesada por la plataforma pandemio para poder obtener la información "depurada" y poderla suministrar a los distintos actores interesados como el gobierno, las autoridades o los ambulatorios.|
| **Comentarios** | De dicho actor se van a obtener sus datos por medio de los datos suministrados por las compañias telefónicas. |

<p align="center"> <b>Tabla 3.1: Actores de negocio.</b>

| **\<id>2** | Gobierno |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | * \<procesos de negocio actuales en los que participa> <br> * ... |
| **Descripción** | Este actor de negocio actual representa al gobierno, en concreto al ministro de sanidad, al que se le suministrarán todos los datos y estadísticas que se han obtenido por medio del procesamiento de los datos capturados de los ciudadanos y procesados por parte de nuestra plataforma pandemio. Dicho actor se encargará como entidad de tomar las decisiones oportunas en función de los datos suministrados por la plataforma, en base a diferentes criterios.
| **Comentarios** | El objetivo de nuestra plataforma es proporcionar los datos lo mejor procesados y "depurados" a este actor para que puedan tomar decisiones. |

<p align="center"> <b>Tabla 3.2: Actores de negocio.</b> 

| **\<id>3** | Autoridades |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | Dicho actor participa en los procesos de negocio 3 Rastreo por contacto con positivo y en el proceso 4 llevar seguimiento del paciente y control de su cuarentena.|
| **Descripción** | Este actor de negocio actual representa a las fuerzas del orden (policía local, nacional, guardia civil y el ejército) que se encargan de rastrear cuales han sido los contactos directos con los positivos y proveer dicha información a los ambulatorios para que sean los encargados de llamar a dichos contactos directos para que se les realicen las pruebas médicas oportunas. También son los encargados de controlar el cumplimiento de las cuarentenas obligatorias por parte de los ciudadanos que deban de cumplirlas, para ello se encargan de hacer llamadas telefónicas o videollamadas con los pacientes positivos para comprobar que se encuentran en casa cumpliendo la cuarentena.|
| **Comentarios** | A este actor en determinadas ocasiones se les llama rastreadores, y llevaran a cabo la misión de rastrear el como se producen los contagios entre los positivos, asi como obtener cuales son los brotes de dichos contagios, para ello tan solo disponen de la información proporcionada por los pacientes positivos.|

<p align="center"> <b>Tabla 3.3: Actores de negocio.</b> </p>

| **\<id>4** | Ambulatorio |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | Este actor entra en juego en la mayoría de los procesos de negocio, dado que es el conocedor de como se debe gestionar la pandemia y se encarga de mediar en como se debe actuar en los distintos casos. Los procesos de negocio en los que particicipa son 1 Hacer prueba PCR, 2 Registrar resultado de la prueba PCR, 3 rastreo por contacto con positivo, 4 llevar seguimiento del paciente y control de su cuarentena y 5 interpretción de los datos. |
| **Descripción** | Este actor de negocio actual representa al centro de salud, asi como los responsables médicos, se encargan de determinar si se les debe de realizar las pruebas a los pacientes ante la aparición de síntomas o por contacto directo, también se encargan de concretar las citas para la realización de las pruebas médicas con los pacientes, así como informarles de los resultados obtenidos en dichas pruebas y en caso de ser positivos solicitan los datos de los contactos directos. <br> Por otra parte, se encargan de registrar los resultados de dichas pruebas en la base de datos del centro de salud, para que posteriormente pueda ser proporcionada esta información al gobierno. También se encargan de realizar un seguimiento de la evolución del estado del paciente durante la cuarentena por medio de las llamadas telefónicas.|
| **Comentarios** | Dicho actor en determinadas ocasiones se les llama responsable Covid y es el encargado de realizar todas las acciones anteriormente comentadas respecto a la gestión de los casos covid en cada uno de los ambulatorios.|

<p align="center"> <b>Tabla 3.4: Actores de negocio.</b> <br> </p>


## 3.2.2 Descripción de Procesos de Negocio Actuales

En este apartado se comentarán cuales son los procesos de negocio que se llevan a cabo en la actualidad para gestionar la pandemia. Dichos procesos son en los que se basará nuestra plataforma para agilizarlos y poder ser llevadas a cabo de una forma más automatizada. De forma general, se comentará cual es el flujo de procesos que se han de llevar a cabo cuando se detectan los sintomas compatibles con la enfermedad. Dichos procesos son los siguientes:

| **\<id>1** | Hacer prueba PCR |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | En algunos casos depende del proceso de negocio 3, Rastreo de contacto con el positivo, sin embargo en otros casos no hay ninguna dependencia cuando se registra un caso aislado. |
| **Descripción** | En la actualidad, cuando un ciudadano presenta síntomas compatibles con la enfermedad, debe de llamar al centro de salud al que esté asignado e indicará cuales son los síntomas que presenta. El responsable Covid de cada centro de salud, será el encargado de tomar la decisión de si se le debe realizar las pruebas oportunas, en la mayoría de los casos se realizan. El centro de salud, concretará una cita médica con el paciente para realizarle las pruebas oportunas. <br> El paciente acudirá al centro médico el día de la cita y se le realizarán las pruebas necesarias, en la mayoría de los casos son una pueba PCR o una prueba de sangre, según el criterio del responsable médico. Después de esto, el paciente debe de dirigirse a su residencia y debe permanecer en cuarentena hasta el resultado de las pruebas realizadas, que en general, no tardarán mas de 24-48 horas.|
| **[Importancia]** | Alta |
| **[Actores]** | * Ciudadano <br> * Ambulatorio |
| **Comentarios** | El medio de comunicación en todo momento son las llamadas telefónicas.|

<p align="center"> <b>Tabla 4.1: Procesos de Negocio actuales.</b> <br> </p>

| **\<id>2** | Registrar resultado prueba PCR |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | Este proceso de negocio depende del proceso 1 hacerse prueba PCR, dado que si no se ha realizado previamente una prueba PCR el paciente, no se puede tener una base en la que basarse para actuar de una forma u otra. |
| **Descripción** | Una vez que el paciente se ha realizado las pruebas oportunas, y se encuentra confinado en su casa, el ambulatorio le llamará para informarle del resultado de las pruebas lo antes posible y en cuanto se conozca el resultado de estas. Además, el ambulatorio se encargará de registrar en su base de datos el resultado de dicha prueba, para que así esta información sea procesada por parte de los responsables sanitarios y se puedan obtener las estadísticas oportunas. <br> Dependiendo del resultado de dicha prueba, se tomarán distintas medidas, si el resultado es positivo, el paciente deberá permanecer aislado y no podrá salir de cas, si convive con mas personas, dichas personas serán detectadas como contacto directo (ver proceso de negocio 3 Rastreo de contacto con positivo) y se les realizarán las pruebas oportunas, si son negativas o hasta que se conozca el resultado de dichas pruebas deberá permanecer aislado en su habitación y no podrá salir de esta a no ser que sea necesario (y con mascarilla siempre). Si el resultado es negativo pero al paciente se le considera contacto directo con un positivo confirmado, deberá permanecer en cuarentena durante 10 días. Si el paciente es negativo,y no es un contacto directo con un caso positivo confirmado, podrá hacer vida normal a no ser que los síntomas persistan que se le repetirá las pruebas por si es un caso de falso negativo.|
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Actores]** | * Ambulatorio> <br> * Ciudadano |
| **Comentarios** | La comunicación se realiza por medio de llamadas telefónicas. Se tienen en cuenta numerosos factores para decidir cual es la forma de actuar en cada caso. |

<p align="center"> <b>Tabla 4.2: Procesos de Negocio actuales.</b> <br>  </p>

| **\<id>3** | Rastreo por contacto con positivo |
| -- | -- |
| **[Versión]** | 1.0(19/11/2020) |
| **[Dependencias]** | Este porceso de negocio depende totalmente del proceso 2, "Registrar resultado de la prueba PCR", ya que unicamente entra en juego con un resultado positivo de la prueba realizada al ciudadano. |
| **Descripción** | A día de hoy en la llamada que se realiza con el usuario susceptible de ser positivo se le solicitan a este los nombres de todas aquellas personas con las que ha mantenido contacto directo a lo largo de las úlitmas horas, normalmente las 48 horas previas a la manifestación de síntomas. En  caso de confirmarse el positivo del usuario los sanitarios y/o las autoridades proceden a contactar con aquellos cuidadanos que el positivo suministró en un primer momento para poder realizarles las pruebas pertinentes a cada uno de ellos y volver a comenzar con el proceso|
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Actores]** | * Ambulatorio <br> * Cuidadano <br> * Autoridades |
| **Comentarios** | Actualmente tenemos que confiar en que el usuario nos proporcione todos los contactos que ha tenido en las horas previas. En este sentido tenemos el handicap de que el usuario puede no recordarlos todos y/o no querer proporcionarlos todos por conveniencia|

<p align="center"> <b>Tabla 4.3: Procesos de Negocio actuales.</b> <br> </p>


| **\<id>4** | Llevar seguimiento del paciente y control de su cuarentena |
| -- | -- |
| **[Versión]** | 1.1(19/11/2020) |
| **[Dependencias]** | Este porceso de negocio depende totalmente del proceso 2, "Registrar resultado de la prueba PCR", ya que unicamente entra en juego con un resultado positivo de la prueba realizada al ciudadano. |
| **Descripción** | Actualmente una vez se detecta un positivo, este queda automaticamente puesto en cuarentena de 10 a 15 días dependiendo del caso. Para poder llevar a cabo un seguimiento de esta cuarentena los sanitarios y/o las autoridades realizan llamadas con frecuencia al paciente. Con esta llamada se pretede controlar que el usuario está cumpliendo las restricciones impuestas así como llevar a cabo un seguimiento sobre su estado de salud|
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Actores]** | * Ambulatorio <br> * Cuidadano <br> * Autoridades |
| **Comentarios** | Este proceso de negocio finalizaría una vez termine esta cuarentena, dando por hecho que, pasado el tiempo estimado, el paciente estará sano y no puede contagiar|

<p align="center"> <b>Tabla 4.4: Procesos de Negocio actuales.</b> <br>  </p>


| **\<id>5** | Interpretación de los datos |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | Dicho proceso de negocio depende sobre todo del proceso 2 registrar casos positivos (para conocer los positivos que hay en cada centro de salud) y del proceso 3 Rastreo por contacto con positivo (para conocer de donde provienen dichos contagios).|
| **Descripción** | Una vez que los casos positivos han sido registrados en las bases de datos de los ambulatorios, estos pueden proporcionar dicha información al gobierno, para que estos tomen las medidas oportunas en función de estos datos proporcionados y las estadísticas obtenidas. |
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Actores]** | * Gobierno <br> * Ambulatorios |
| **Comentarios** | El gobierno debe de pedir los datos sanitarios a los ambulatorios "en crudo" y por medio de los expertos del gobierno se realizarán las estadísticas oportunas con la escasa información que se dispone de cada caso, para posteriormente tomar decisiones. Pero los ambulatorios no disponen de dicha información de forma directa.|

<p align="center"> <b>Tabla 4.5: Procesos de Negocio actuales.</b> <br> </p>

# 3.3 Entorno Tecnológico Actual


Pandemio surge como necesidad de mejorar diferentes aspectos negativos encontrados en la ya existente aplicación Radar Covid, aparte de introducir nueva funcionalidad para poder gestionar los datos acerca de la pandemia. Además a parte de esta aplicación en la actualidad se encuentran otras con una funcionalidad parecida, como se ha comentado en el apartado 3.0.

Dado que en la actualidad, la sociedad está muy concienciada con las nuevas tecnologías y cada vez está mas acostrumbrada al uso de la tecnología en su vida diaria, hace que sea interesante aprovechar este entorno tecnológico en el que vivimos para poder obtener datos e información acerca de la pandemia.


## 3.3.1 Descripción del Entorno de Hardware Actual

Hoy en día, cerca del 90% de la población española dispone de un teléfono móvil y en la mayoría de los casos se tratan de smartphones. Aprovechando de que la mayoría de la población dispone de tal dispositivo y lo lleva siempre consigo, podemos beneficiarnos de toda la información que se está compartiendo por la red mientras estamos conectados o disponemos de cobertura o señal GPS.

Por otra parte, hoy en dia disponemos de unas buenas infraestructuras de redes de comunicación en la que se pueden sustentar todo este intercambio de información constante.

Dado que pandemio va a gestionar también información y datos médicos relativos a los pacientes que se deben realizar las pruebas oportunas en los ambulatorios en los que estén asigandos, se necesita disponer de tal información la cual se encuentra en las bases de datos y servidores del sistema sanitario de cada comunidad autónoma.Por lo que resulta conveniente que se pueda acceder a tal información de dichas bases de datos por medio de nuestra plataforma pandemio.

## 3.3.2 	Descripción del Entorno de Software Actual

A día de hoy y como consecuencia de la relevancia a nivel mundial y de la alteración de la normalidad que ha supuesto la pandemia del COVID-19 se han implementado numerosas aplicaciones en torno a la resolución de este problema o simplemente para poder obtener un mejor conocimiento sobre sus efectos en la población de cara a tomar medidas que nos puedan ayudar a revertir poco a poco esta situación. Observando el estado del arte en este campo podemos orientar mejor nuestro trabajo. Tomaremos como referencia algunas aplicaciones, además de _Radar Covid_ en este ambito que creemos que nos pueden ayudar en nuestro proyecto:

__CoronaMadrid:__ La aplicación permite a sus usuarios poder detectar, informarse y contactar con las autoridades en cualquier fase de la concepción de la enfermedad COVID-19. CoronaMadrid tiene la misión de ayudar a los ciudadanos a poder detectar si están siendo afectados por la enfermedad y obtener las mejores recomendaciones dependiendo de su estado. En caso de estado grave las autoridades serán conocedoras de la situación y podrán comunicarse directamente con el afectado.

De _CoronaMadrid_ nos resulta interesante la capacidad del usuario para informarse y poner en conocimiento de las autoridades su estado.

__COVID-19.eus:__ Es una aplicación colaborativa en el ámbito de la comunidad autónoma vasca. La aplicación permite hacer un autodiagnóstico del contagio de COVID-19. En caso de ser positivo, el usuario se considerará _POSIBLE contagio_ (según terminología de la OMS) y avisará a todo el cículo de personas, de tal forma que se considerarán en riesgo. Junto a esta información el sistema registrará ese dato, de tal forma que se puede seguir un rastro de contagios con esta funcionalidad de círculos. Junto con esta información, se pide el Código Postal, y en caso de infección comunitaria, se podrían también detectar focos de contagio.

Con respecto a _COVID-19.eus_ creemos que puede ser útil la manera de prevenir la extension de los contagios por medio del aviso al círculo de personas cercanas a un positivo y la relativa capacidad de detectar focos de contagio.

__STOP COVID19 CAT:__ Es una aplicación móvil de salud con un doble objetivo: Dar respuesta a las necesidades de información de la ciudadanía en relación al Covid 19, a través de un cuestionario que les indica si tienen posibilidad de tener Covid. Recoger datos de la población para poder crear estadisticas.

De _STOP COVID19 CAT_ nos parece buena idea el uso de los datos de la población para llevar a cabo estadísticas de las cuales obtener conclusiones a utilizar.

De Radar Covid, ya se ha comentado en secciones previas de este documento, como surge la necesidad de desarrollar esta nueva plataforma Pandemio, ante los errores detectados en la anterior aplicación del ministerio. Los cuales son el uso de bluetooth y que su uso no es obligatorio por parte de los usuarios. Sin embargo, resulta interesante la idea de como rastrear los contagios entre los ciudadanos, por lo que usaremos esta idea como base en nuestra plataforma Pandemio, pero realizando las modificaciones de oportunas en su implementación para mitigar los problemas de implementación encontrados en Radar Covid.

