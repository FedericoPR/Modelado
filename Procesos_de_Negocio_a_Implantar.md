### 4.2 Modelos de Procesos de Negocio a Implantar

En este apartado representaremos y describiremos todos aquellos procesos que se llevarán acabo en nuestra plataforma PANDEMIO para gestionar los contagios que se producen en la pandemia, asi como los procesos que se emplearán para controlar el cumplimiento de la cuarentena obligatoria por parte de los ciudadanos positivos. También se tendrán en cuenta todos aquellos procesos en los que se gestionen las distintas pruebas médicas que se deben realizar los ciudadanos, asi como informales a estos de los resultados.Por otro lado, se especificará como debe ser la comunicación con el resto de actores que intervienen en la plataforma como los agentes de la autoridad o el gobierno al que se le proporcionarán todos los datos obtenidos con la plataforma para que puedan tomarse las medidas oportunas por parte de los expertos correspondientes.

#### 4.2.1 Descripción de los Actores de Negocio a Implantar
Los actores de negocio de nuestra plataforma PANDEMIO, son todas aquellas personas, entidades u organizaciones que están involucrados en los procesos de negocio a implantar, en este caso los actores de negocio de nuestra plataforma son los siguientes: ciudadanos, gobierno, autoridades y ambulatorios.

| **\<id>001** | Ciudadano |
| -- | -- |
| **[Versión]** | 1.0(28/11/2020) |
| **[Dependencias]** | * \<procesos de negocio actuales en los que participa> <br> * ... |
| **Descripción** | Este actor de negocio actual es el actor principal de la plataforma y representa a cada uno de los ciudadanos, de dicho actor se van a obtener todos los datos que se gestionarán por medio de la plataforma. De ellos por medio de sus dispositivos móviles, se va a poder acceder a cual ha sido su localización, las personas con las que ha estado en contacto, el tiempo que ha permanecido en un determinado lugar, etc. Toda esta información será procesada por la plataforma pandemio para poder obtener la información "depurada" y poderla suministrar a los distintos actores interesados como el gobierno, las autoridades o los ambulatorios.|
| **Comentarios** | De dicho actor se van a obtener sus datos por medio de los datos suministrados por las compañias telefónicas. |

<p align="center"> <b>Tabla 6.1: Actores de negocio a implantar.</b>

| **\<id>002** | Gobierno |
| -- | -- |
| **[Versión]** | 1.0(28/11/2020) |
| **[Dependencias]** | * \<procesos de negocio actuales en los que participa> <br> * ... |
| **Descripción** | Este actor de negocio actual representa al gobierno, en concreto al ministerio de sanidad y el comité de expertos, al que se le suministrarán todos los datos y estadísticas que se han obtenido por medio del procesamiento de los datos capturados de los ciudadanos y procesados por parte de nuestra plataforma pandemio. Dicho actor se encargará como entidad de tomar las decisiones oportunas en función de los datos suministrados por la plataforma, en base a diferentes criterios.
| **Comentarios** | El objetivo de nuestra plataforma es proporcionar los datos lo mejor procesados y "depurados" a este actor para que puedan tomar decisiones. |

<p align="center"> <b>Tabla 6.2: Actores de negocio a implantar.</b> 

| **\<id>003** | Autoridades |
| -- | -- |
| **[Versión]** | 1.0(28/11/2020) |
| **[Dependencias]** | * \<procesos de negocio actuales en los que participa> <br> * ... |
| **Descripción** | Este actor de negocio actual representa a las fuerzas del orden (policía local, nacional, guardia civil y el ejército) que deberán de ser informados del cumplimiento de la cuarentena y poder verificar que se está cumpliendo esta. Dicho actor podrá acceder a la información de los ciudadanos que estén en cuarentena para poder controlar que se cumplen dichas cuarentenas así como intervenir en el caso de que dejen de cumplirse o no se realicen las pruebas médicas oportunas.|
| **Comentarios** | Las autoridades dispondrán de dispositivos por medio de los cuales se les podrá notificar cuando un ciudadano no se ha presentado a hacerse las pruebas médicas, para que actuen en consecuencia. Por otra parte, también se les informará cuando deben de realizar los controles periódicos de que se cumple la cuarentena entre aquellos ciudadanos que deben cumplirla, será con la minoría de la población que no disponde de teléfono móvil o con aquellos que sí disponen de teléfono móvil pero que no es posible verificar que se encuentran en casa o es imposible contactar con ellos.|

<p align="center"> <b>Tabla 6.3: Actores de negocio a implantar.</b> </p>

| **\<id>004** | Ambulatorio |
| -- | -- |
| **[Versión]** | 1.0(28/11/2020) |
| **[Dependencias]** | * \<procesos de negocio actuales en los que participa> <br> * ... |
| **Descripción** | Este actor de negocio actual representa al centro de salud que dispondrá de listados donde se informarán del estado de los ciudadanos, así como de las distintas pruebas médicas que se les debe de realizar a cada uno de ellos. También se encargarán de notificar a los ciudadanos las citas en las que se les realizarán las pruebas, asi como las medidas que deben de tomar en caso de dar positivo y cual es la duración de la cuarentena que deben de cumplir.|
| **Comentarios** | Este actor podrá acceder a los datos de los ciudadanos (a sus datos médicos), también será el encargado de registrar el resultado de las pruebas realizadas a los ciudadanos en la plataforma pandemio, para que finalmente se pueda contabilizar dicho positivo y poder hacer un seguimiento de los contactos de dicho positivo, así como proporcionar los datos al gobierno. |

<p align="center"> <b>Tabla 6.4: Actores de negocio a implantar.</b> <br> </p>

#### 4.2.2 Descripción de Procesos de Negocio a Implantar
Esta sección debe contener información sobre los procesos de negocio a implantar, tal y como se espera que se realicen en la organización del cliente una vez que el sistema software a desarrollar esté en producción. Para cada proceso de negocio se incluirá una descripción textual usando las plantillas para procesos de negocio a implantar que se muestran a continuación, y un diagrama en la notación que se considere oportuna, por ejemplo diagramas BPMN (Business Process Model and Notation) o diagramas de actividad UML (Unified Modeling Language).

| **\<id>999** | \<nombre descriptivo> |
| -- | -- |
| **[Versión]** | <nº versión>(<fecha versión>) |
| **[Dependencias]** | * \<procesos de negocio actuales que modifica o sustituye> <br> * ... |
| **Descripción** | <descripción del proceso de negocio a implantar en términos del dominio del problema> |
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Actores]** | * \<actor que participa en el proceso de negocio> <br> * ... |
| **Comentarios** | \<comentarios adicionales sobre el proceso de negocio a implantar> |

<p align="center"> <b>Tabla 7: Procesos de Negocio a implantar.</b> <br> </p>
