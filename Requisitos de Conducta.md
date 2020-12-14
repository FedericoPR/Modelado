
#### 6.3.3 	Requisitos de Conducta del Sistema

A continuación se pasan a detallar aquellos requisitos de las acciones que deberá realizar el sistema de manera independiente y sin una acción especifica del usuario. Estas acciones serán automatizdadas por el sistema y se lanzarán, normalmente, cuando se ejecute otra acción.

_Esta sección debe contener los requisitos de conducta que se hayan identificado, especificados mediante las plantillas de requisitos de conducta que se muestran a continuación.
Estos requisitos deben especificar cualquier otro comportamiento deseado del sistema que no se haya especificado mediante los casos de uso del sistema, como generación de informes, funcionalidades transversales a varios casos de uso del sistema, etc._

| **RF 10** | Comprobar la ubicación del usuario en cuarentena |
| -- | -- |
| **[Versión]** | 1.0 (10/12/2020) |
| **[Dependencias]** | Este requisito tiene dependencia directa con el caso de uso 2.1 "Control automático por el sistema del cumplimiento cuarentena" y tambien depende de el el caso de uso 2.3 "Enviar alerta autoridades incumplimiento cuarentena" |
| **Descripción** | El sistema deberá verificar el cumplimiento de la cuarentena por medio de la ubicación. Tendrá automatizada la tarea de comprobar de una manera frecuente que los cuidadanos que tienen que estar cumpliendo cuarentena lo estén haciendo. Para ello filtrará los cuidadanos que tenemos almacenados por el estado "en cuarentena" y comprobará cual es la ubicación de su dispositivo móvil, en caso de que la ubicación no coincida con la de su domicilio se enviará una alerta al cuidadano y las autoridades por incumplimiento de la cuarentena para que, estas, procedan con las acciones necesarias.|
|  |  |
| **Subobjetivos** | En caso de ubicación erronea se autoimatizará el aviso al cuidadano y a las autoridades |
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **Comentarios** | Si la ubicación se comprueba que es la misma que la de la vivienda el sistema no hará nada y volverá a realizar la comprobación cuando pase el tiempo establecido |

| **RF 11** |Solicitar los datos de localización de los ciudadanos|
| -- | -- |
| **[Versión]** | 1.0 (10/12/2020) |
| **[Dependencias]** | De este requisito dependerá el CU 1.3 "Rastrear contactos directos con el postivo" ya que para realizarlo hará uso de los datos aquí adquiridos. Además los datos de los cuidadanos en cuanto al tipo de móvil que tienen y a cual es su domicilio tambien serán usados en en control de las cuarentenas|
| **Descripción** | El sistema deberá solicitar los datos relevantes de la localización de los ciudadanos a las operadoras. Para poder llevar a cabo los rastreos una vez se detecte un positivo se deberá disponer de la localización de los cuidadanos para detectar aquellos que puedan haber mantenido el contacto con el positivo. Estas localizaciones de los ciudadanos serán suministradas cada poco tiempo por parte de las operadoras móviles. Para ello el sistema solicitará con una determinada frecuencia estos datos a las operadoras que los introducirán o proporcionaran para su inclusión y/o actualización en el sistema|
|  |  |
| **Subobjetivos** | Estos datos serán usados en el rastreo de positivos de manera automática por el sistema |
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **Comentarios** | El volumen de datos será inmenso y por lo tanto debemos disponer de servidores lo suficientemente grandes como para alamcenarlos y procesarlos |

| **RF 12** | Rastreo de contactos con positivo |
| -- | -- |
| **[Versión]** | 1.0 (11/12/2020) |
| **[Dependencias]** | Este requisito depende en gran medida del CU 1.3 "Rastrear contactos directos con el postivo" ya que el restreo automático por parte del sistema para sacar una lista con los posibles infectados es el primer paso y por tanto imprescindible del CU "Rastrear contactos directos con el postivo"|
| **Descripción** | El sistema deberá realizar un rastreo de contactos de forma automática con cada positivo registrado. Una vez se obtengan los resultados de la prueba realizada a un cuidadano y se registre el resultado de la prueba como "positivo", el sistema lo detectará y de manera automática comenzará a rastrear, usando los datos disponibles de las operadoras, todos aquellos cuidadanos que han mantenido un contacto suficiente con el positivo para ser considerados como posibles contagiados. Una vez finalice el rastreo proporcionará una lista con los nombres de los cuidadanos obtenidos, que se registrarán para que puedan ser contactados y concretar una cita en la que realizarse las pruebas |
|  |  |
| **Subobjetivos** | El sistema proporcionará una lista de nombres, también de manera automática, tras realizar el rastreo|
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **Comentarios** | Será de vital importancia para este requisito que se cumpla también y con eficacia el de "Solicitar los datos de localización de los ciudadanos" a las operadoras |

| **RF 13** | Envio de alertas de estado al usuario|
| -- | -- |
| **[Versión]** | 1.0 (11/12/2020) |
| **[Dependencias]** | Este requisito dependerá del CU 0.2 "Informar al ciudadano" donde se le informa de todo aquello que sea relevante para el y con respecto a su situación |
| **Descripción** | El sistema deberá de enviar alertas vía sms con cada alteración del estado del ciudadano. En numerosos puntos de los diferentes flujos que pueden darse en el sistema, el estado del cuidadano se verá alterado y el sistema se encargará de informarlo via sms del nuevo estado. Se distinguen diferentes ocasiones en las que el sistema enviará un sms al usuario para informarle de su nuevo estado: Cuando el cuidadano salte con motivo de un rastreo, este será registrado en el sistema con el estado "Pendiente de cita" y se le comunicará esta situación para que sepa que en breve será contactado para concretar una cita para las pruebas. Una vez se le registre una cita al usuario y se cambie su estado a "Pendiente de realizar las pruebas" el sistema enviará un sms al cuidadano con la fecha y hora de la cita para que no lo olvide y para que se mantenga en la medida de lo posible en cuarentena hasta la cita. En caso de no acudir a la cita se le notificará al cuidadano que no ha acudido y que dispone de 24h para infomrar al ambulatorio de su situación y para cambiar la cita, si pasan 24h desde la hora de la cita prevista (por no haberse actualizado con una nueva cita) se le comunicará al cuidadano y a las autoridades de esta situación. Tras conocerse los resultados de las pruebas se le comunicará al cuidadano cuales han sido estos, en caso de ser positivo se cambiará el estado a "positivo", se pondrá al cuidadano en cuarentena estableciendo una fecha de final de la misma y se le enviará una notificación via sms con toda esta información. En caso de ser negativo tambien se le informará vía sms. |
|  |  |
| **Subobjetivos** | El subobjetivo principal de este requisito es que en todo momento el usuario tenga infomación de su estado para poder justificar una intervención de las autoridades en caso de incumplimiento.
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **Comentarios** | En todo momento se le informará al usuario de que sus datos están siendo tratados siguiendo la ley de proteccion de datos |

| **RF 14** | Adaptar el cumplimiento de la cuarentena al tipo de movil del cuidadano o a la ausencia del mismo |
| -- | -- |
| **[Versión]** | 1.0 (11/12/2020) |
| **[Dependencias]** | Este requisito depende sobre todo del CU 2.1 "Control automático por el sistema del cumplimiento cuarentena" |
| **Descripción** | El sistema deberá diferenciar como llevar a cabo el cumplimiento de la cuarentena en función del tipo de móvil del ciudadano (o si no dispone de el). Haciendo uso de los datos de los cuidadanos proporcionados por las operadoras y una vez se detecte un caso como positivo el sistema deberá adaptar el contro de la cuarentena del mismo al móvl del que disponga el cuiadano. La localización cada 10 minutos se realizará siempre igual entre los usuarios con movil, pero además de esto se realizará una comprobación, con menos frecuencia, ya que el usuario puede estar fuera de su domicilio sin portar el móvil. Para los usuarios con movil por desbloqueo con huella el sistema enviará en un periodo de tiempo aleatorio desbloquear el móvil al ciudadano por medio de la huella dactilar y al hacerlo se tomará una foto del ciudadano. El sistema actuará de distinta forma si los ciudadanos que deben cumplir cuarentena disponen de teléfono móvil sin desbloqueo por huella dactilar. En este caso el sistema permitirá que un agente de la autoridad realice una videollamada con el ciudadano comprobando que es él, y se obtendrá la localización del teléfono móvil en ese momento|
|  |  |
| **Subobjetivos** | El subobjetivo principal es que complementar la verificacion de loaclización automática ya que esta puede ser evadida |
| **[Importancia]** | Media |
| **[Prioridad]** | Media |
| **Comentarios** | En caso de que el usuario tenga movil con huella, realizará el sistema las comprobaciones de manera automática y en caso de ser sin huella permitirá a las aurtoridades de manera automática la realización de videollamadas periódicamente. |

| **RF 15** | Envío de estadisticas al gobierno|
| -- | -- |
| **[Versión]** | 1.0 (11/12/2020) |
| **[Dependencias]** | Este requisito depende de todos los casos de uso del subsistema de gestión e información y estadísticas al gobierno ya que engloba el envio al gobierno de todo tipo de información y estadísticas que puedan ser relevantes para ellos como los casos positivos, los posibles focos y las estadísticas por zonas, edades...etc |
| **Descripción** | El sistema deberá enviar estadísticas generales al gobierno de forma automática cada 3 días. Con todos los datos recopilados y registrados en el sistema, este realizará informes con las estadísticas más relevantes, como el número de contagios al día, los focos de contagio, el cumplimiento de las cuarentenas...etc, para proporcionarselas al gobierno en vistas a tomar decisiones. |
|  |  |
| **Subobjetivos** | El subobjetivo es porporcionar al gobierno de un respaldo, por medio de nuestros datos, de todas aquellas decisiones que se vayan a tomar |
| **[Importancia]** | Alta  |
| **[Prioridad]** | Alta |
| **Comentarios** | El sistema será configurado para poder extraer todas las estadísticas posibles y luego podremos modificar las que queremos que aparezcan en los informes en funcion de las necesidades, ya que dependiendo de la situación podemos considrerar más importantes unos datos u otros  |

