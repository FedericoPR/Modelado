# 3.2 Modelos de Procesos de Negocios Actuales

En este apartado representaremos y describiremos todos aquellos procesos que se llevarán acabo para poder mantener un control del estado de los usuarios de nuestra aplicación. Así podremos informar a los actores interesados del estado de la pandemia en su zona dotando de información útil para cada tipo de usuario. 

## 3.2.1 Descripción de los Actores de Negocio Actuales

Los actores de negocio de nuestra aplicación o toda aquella persona interesada en está serán: ciudadanos, gobierno, autoridades y ambulatorios. Necesarios para que la información se transmita de manera segura.

| **\<id>1** | Ciudadano |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | * \<procesos de negocio actuales en los que participa> <br> * ... |
| **Descripción** | Este actor de negocio actual representa a los usuarios de a pie que podrán llevar un seguimiento de su estado asi como de acceder a estadisticas de su zona |
| **Comentarios** | \<comentarios adicionales sobre el actor de negocio actual> |

<p align="center"> <b>Tabla 3.1: Actores de negocio.</b> <br> <i>Los atributos entre corchetes son opcionales</i> </p>

| **\<id>2** | Gobierno |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | * \<procesos de negocio actuales en los que participa> <br> * ... |
| **Descripción** | Este actor de negocio actual representa al gobiberno, en concreto al ministro de sanidad que podrá acceder a los listados y estadísticas generadas por la aplicación, lo que les servirá para tomar medidas e informarse de la situacion sanitaria |
| **Comentarios** | \<comentarios adicionales sobre el actor de negocio actual> |

<p align="center"> <b>Tabla 3.2: Actores de negocio.</b> <br> <i>Los atributos entre corchetes son opcionales</i> </p>

| **\<id>3** | Autoridades |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | * \<procesos de negocio actuales en los que participa> <br> * ... |
| **Descripción** | Este actor de negocio actual representa a las fuerzas del orden (policía local, nacional, guardia civil y el ejército) que deberán de ser informados del cumplimiento de la cuarentena y poder verificar que se esta cumpliendo esta. |
| **Comentarios** | \<comentarios adicionales sobre el actor de negocio actual> |

<p align="center"> <b>Tabla 3.3: Actores de negocio.</b> <br> <i>Los atributos entre corchetes son opcionales</i> </p>

| **\<id>4** | Ambulatorio |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | * \<procesos de negocio actuales en los que participa> <br> * ... |
| **Descripción** | Este actor de negocio actual representa al centro de salud que dispondrá de listados donde se informarán del estado de los usuarios, pudiendo preveer que servicios pueden ofrecer. Así como un medio, para comunicarle al usuario que medidas debe tomar, periodo de cuarentena, pruebas a realizar, etc  |
| **Comentarios** | \<comentarios adicionales sobre el actor de negocio actual> |

<p align="center"> <b>Tabla 3.4: Actores de negocio.</b> <br> <i>Los atributos entre corchetes son opcionales</i> </p>


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

Pandemio parte de una aplicación ya existente (Radar Covid), aparte de los servidores a los que se conecta dicha aplicación. Las bases de datos de cada autonomía. Aparte de la propia tecnologia Bluetooth (hardware y software) en la que se basa el funcionamiento de Radar Covid


## 3.3.1 Descripción del Entorno de Hardware Actual

Para que Radar Covid funcione es necesario un terminal (teléfonos de los usuarios), base de datos con datos anonimos que tienen identificadores de casos cofirmados. Incuimos tambien todo el soporte de red.

## 3.3.2 	Descripción del Entorno de Software Actual

La antigüa aplicación está disponible tanto para android como para ios. Utiliza como kit de desarrollo DP-3T (Decentralized Privacy-Preserving Proximity Tracing) que es un protocolo para el rastreo digital de los contactos de manera anónima donde cada terminal se conecta a través de un token con el servidor. Por otro lado contamos con otras aplicaciones como por ejemplo Coronamadrid.
