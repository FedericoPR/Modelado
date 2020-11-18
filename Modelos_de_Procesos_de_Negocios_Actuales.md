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
| **[Dependencias]** | * \<procesos de negocio actuales en los que participa> <br> * ... |
| **Descripción** | Este actor de negocio actual representa a las fuerzas del orden (policía local, nacional, guardia civil y el ejército) que deberán de ser informados del cumplimiento de la cuarentena y poder verificar que se esta cumpliendo esta. Dicho actor puede acceder a la información de los ciudadanos que estén encuarentena para poder controlar que se cumplen dichas cuarentenas así como intervenir en el caso de que dejen de cumplirse o no se realicen las pruebas médicas oportunas.|
| **Comentarios** | Las autoridades dispondran de dispositivos por medio de los cuales se les podrá notificar cuando un ciudadano no se ha presentado a hacerse las pruebas médicas, para que actuen en consecuencia. Por otra parte, también se les informará cuando deben de realizar los controles periódicos de que se cumple la cuarentena entre aquellos ciudadanos que deben cumplirla, será con la minoría de la población que no disponde de teléfono móvil o con aquellos que si disponen de teléfono móvil pero que no es posible verificar que se encuentran en casa o es imposible contactar con ellos.|

<p align="center"> <b>Tabla 3.3: Actores de negocio.</b> </p>

| **\<id>4** | Ambulatorio |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | * \<procesos de negocio actuales en los que participa> <br> * ... |
| **Descripción** | Este actor de negocio actual representa al centro de salud que dispondrá de listados donde se informarán del estado de los ciudadanos, así como de las distintas pruebas médicas que se les debe de realizar a cada uno de ellos. También se encargarán de notificar a los ciudadanos las citas en las que se les realizarán las pruebas, asi como las medidas que deben de tomar en caso de dar positivo y cual es la duración de la cuarentena que deben de cumplir. |
| **Comentarios** | Este actor podrá acceder a los datos de los ciudadanos (a sus datos médicos), también será el encargado de registrar el resultado de las pruebas realizadas a los ciudadanos en la plataforma pandemio, para que finalmente se pueda contabilizar dicho positivo y poder hacer un seguimiento de los contactos de dicho positivo, así como proporcionar los datos al gobierno. |

<p align="center"> <b>Tabla 3.4: Actores de negocio.</b> <br> </p>


## 3.2.2 Descripción de Procesos de Negocio Actuales

Aquí se especificarán los procesos que debe llevar a cabo nuestra aplicación que llevarán un diagrama donde se detallarán los pasos a seguir. Según finalicen las entrevistas se irán añadiento y modificando los procesos. Inicialmente podemos pensar en estos como los procesos principales del programa.

| **\<id>1** | Registrar Caso Positivo |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | * \<procesos de negocio actuales en los que participa>  <br> * ... |
| **Descripción** | Se espera que la aplicación mantenga un registro de los usuarios que han dado positivo en coronavirus, alamacenándolos en registros que podrán ver tanto los ambulatorios como las autoridades. |
| **[Importancia]** | Alta |
| **[Actores]** | * Ciudadano <br> * ... |
| **Comentarios** | \<comentarios adicionales sobre el actor de negocio actual> |

<p align="center"> <b>Tabla 4.1: Procesos de Negocio actuales.</b> <br> <i>Los atributos entre corchetes son opcionales</i> </p>

| **\<id>2** | Notificar a la autoridad |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | * \<procesos de negocio actuales en los que participa>  <br> * ... |
| **Descripción** | El sistema será capaz de enviar un mensaje a la autoridad en caso de que un paciente no este cumpliendo el periodo de cuarentena. Así los agentes podrán tomar medidas lo más breve posible. |
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Actores]** | * Ambulatorio> <br> * Autoridad |
| **Comentarios** | \<comentarios adicionales sobre el actor de negocio actual> |

<p align="center"> <b>Tabla 4.2: Procesos de Negocio actuales.</b> <br> <i>Los atributos entre corchetes son opcionales</i> </p>

| **\<id>3** | Generar listas pacientes |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | * \<procesos de negocio actuales en los que participa>  <br> * ... |
| **Descripción** | La aplicación guardará a los usuarios en listados filtrados en función del parámetro deseado. Tanto con pacientes que han dado positivo, los que están pendientes de la prueba. Almacenados de manera anónima solo podrán ser accedidos por aquellos que tengan permiso para verlos como el ambulatorio. O las autoridades en caso de incumplimiento del periodo de cuarentena.  |
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Actores]** | * Ciudadano <br> * Ambulatorio <br> * Autoridad |
| **Comentarios** | \<comentarios adicionales sobre el actor de negocio actual> |

<p align="center"> <b>Tabla 4.3: Procesos de Negocio actuales.</b> <br> <i>Los atributos entre corchetes son opcionales</i> </p>

| **\<id>4** | Llevar seguimiento |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | * \<procesos de negocio actuales en los que participa>  <br> * ... |
| **Descripción** | El sistema podrá verificar que el paciente está cumpliendo con el periodo de cuarentena. Enviando avisos y realizando las comprobaciones oportunas (peticion de desbloqueo por huella, llamadas telefónicas, mensajes de texto, etc...)  |
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Actores]** | * Ciudadano <br> * ... |
| **Comentarios** | \<comentarios adicionales sobre el actor de negocio actual> |

<p align="center"> <b>Tabla 4.4: Procesos de Negocio actuales.</b> <br> <i>Los atributos entre corchetes son opcionales</i> </p>

# 3.3 Entorno Tecnológico Actual


Pandemio surge como necesidad de mejorar diferentes aspectos negativos encontrados en la ya existente aplicación Radar Covid, aparte de introducir nueva funcionalidad para poder gestionar los datos acerca de la pandemia. Además a parte de esta aplicación en la actualidad se encuentran otras con una funcionalidad parecida, como se ha comentado en el apartado 3.0.

Dado que en la actualidad, la sociedad está muy concienciada con las nuevas tecnologías y cada vez está mas acostrumbrada al uso de la tecnología en su vida diaria, hace que sea interesante aprovechar este entorno tecnológico en el que vivimos para poder obtener datos e información acerca de la pandemia.


## 3.3.1 Descripción del Entorno de Hardware Actual

Hoy en día, cerca del 90% de la población española dispone de un teléfono móvil y en la mayoría de los casos se tratan de smartphones. Aprovechando de que la mayoría de la población dispone de tal dispositivo y lo lleva siempre consigo, podemos beneficiarnos de toda la información que se está compartiendo por la red mientras estamos conectados o disponemos de cobertura o señal GPS.

Por otra parte, hoy en dia disponemos de unas buenas infraestructuras de redes de comunicación en la que se pueden sustentar todo este intercambio de información constante.

Dado que pandemio va a gestionar también información y datos médicos relativos a los pacientes que se deben realizar las pruebas oportunas en los ambulatorios en los que estén asigandos, se necesita disponer de tal información la cual se encuentra en las bases de datos y servidores del sistema sanitario de cada comunidad autónoma.Por lo que resulta conveniente que se pueda acceder a tal información de dichas bases de datos por medio de nuestra plataforma pandemio.

## 3.3.2 	Descripción del Entorno de Software Actual

**Se puede añadir aquí el estudio del arte de la descripcion del entrono actual**

La antigüa aplicación está disponible tanto para android como para ios. Utiliza como kit de desarrollo DP-3T (Decentralized Privacy-Preserving Proximity Tracing) que es un protocolo para el rastreo digital de los contactos de manera anónima donde cada terminal se conecta a través de un token con el servidor. Por otro lado contamos con otras aplicaciones como por ejemplo Coronamadrid.
