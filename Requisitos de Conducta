
#### 6.3.3 	Requisitos de Conducta del Sistema

A continuación se pasan a detallar aquellos requisitos de las acciones que deberá realizar el sistema de manera independiente y sin una acción especifica del usuario. Estas acciones serán automatizdadas por el sistema y se lanzarán, normalmente, cuando se ejecute otra acción.

_Esta sección debe contener los requisitos de conducta que se hayan identificado, especificados mediante las plantillas de requisitos de conducta que se muestran a continuación.
Estos requisitos deben especificar cualquier otro comportamiento deseado del sistema que no se haya especificado mediante los casos de uso del sistema, como generación de informes, funcionalidades transversales a varios casos de uso del sistema, etc._

| **\<id>999** | Comprobar la ubicación del usuario en cuarentena |
| -- | -- |
| **[Versión]** | 1.0 (10/12/2020) |
| **[Dependencias]** | Este requisito tiene dependencia directa con el caso de uso 2.1 "Control automático por el sistema del cumplimiento cuarentena" y tambien depende de el el caso de uso 2.3 "Enviar alerta autoridades incumplimiento cuarentena" |
| **Descripción** | El sistema deberá verificar el cumplimiento de la cuarentena por medio de la ubicación. Tendrá automatizada la tarea de comprobar de una manera frecuente que los cuidadanos que tienen que estar cumpliendo cuarentena lo estén haciendo. Para ello filtrará los cuidadanos que tenemos almacenados por el estado "en cuarentena"
y comprobará cual es la ubicación de su dispositivo móvil, en caso de que la ubicación no coincida con la de su domicilio se enviará una alerta al cuidadano y las autoridades por incumplimiento de la cuarentena para que, estas, procedan con las acciones necesarias.|
|  |  |
| **Subobjetivos** | En caso de ubicación erronea se autoimatizará el aviso al cuidadano y a las autoridades |
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **Comentarios** | Si la ubicación se comprueba que es la misma que la de la vivienda el sistema no hará nada y volverá a realizar la comprobación cuando pase el tiempo establecido |

| **\<id>999** |Solicitar los datos de localizacio de los ciudadanos|
| -- | -- |
| **[Versión]** | \<nº versión> (<fecha de versión>) |
| **[Dependencias]** | De este requisito dependerá el "Rastreo de positivos por parte del sistema" ya que para realizarlo hará uso de los datos aquí adquiridos. Además los datos de los cuidadanos en cuanto al tipo de móvil que tienen y a cual es su domicilio tambien serán usados en en control de las cuarentenas|
| **Descripción** | El sistema deberá solicitar los datos relevantes de la localización de los ciudadanos a las operadoras. Para poder llevar a cabo los rastreos una vez se detecte un positivo se deberá disponer de la localización de los cuidadanos para detectar aquellos que puedan haber mantenido el contacto con el positivo.
Estas localizaciones de los ciudadanos serán suministradas cada poco tiempo por parte de las operadoras móviles. Para ello el sistema solicitará con una determinada frecuencia estos datos a las operadoras que los introducirán o proporcionaran para su inclusión y/o actualización en el sistema|
|  |  |
| **Subobjetivos** | Estos datos serán usados en el rastreo de positivos de manera automática por el sistema |
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **Comentarios** | El volumen de datos será inmenso y por lo tanto debemos disponer de servidores lo suficientemente grandes como para alamcenarlos y procesarlos |

| **\<id>999** ||
| -- | -- |
| **[Versión]** | \<nº versión> (<fecha de versión>) |
| **[Dependencias]** | |
| **Descripción** | |
|  |  |
| **Subobjetivos** | |
| **[Importancia]** |  |
| **[Prioridad]** |  |
| **Comentarios** |  |


(QUEDAN)

El sistema debera realizar un rastreo de contactos de forma automática con cada positivo registrado.
El sistema deberá de enviar alertas vía sms con cada alteración del estado del ciudadano.
El sistema deberá diferenciar como llevar a cabo el cumplimiento de la cuaentena en e función del tipo de movil del ciudadano tipos de movil (o si no dispone de el).
El sistema deberá enviar estadísticas generales al gobierno de forma automática cada 3 días
-AFINAR DPENDENCIAS-CITAR casos de uso o requisitos de manera más concreta
