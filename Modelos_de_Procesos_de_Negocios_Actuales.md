# 3.2 Modelos de Procesos de Negocios Actuales

En este apartado representaremos y describiremos todos aquellos procesos que se llevarán acabo para poder mantener un control del estado de los usuarios de nuestra aplicación. Así podremos informar a los actores interesados del estado de los usuarios registrados. 

_(Esta sección debe contener información sobre los modelos de procesos de negocio actuales,
que suelen ser la base de los modelos de procesos de negocio a implantar.
Se divide en las secciones que se describen a continuación.)_

## 3.2.1 Descripción de los Actores de Negocio Actuales

Los actores de negocio de nuestra aplicación o toda aquella persona interesada en está serán: usuarios, ministerio de sanidad, autoridades (policia, guardia civil, ...), ambulatorios. 
- Los usuarios: se podrán registrar en la aplicación para asi llevar un seguimiento de su estado asi como de poder acceder a estadísticas de su zona.
- Ministerio de sanidad: podrá acceder a los listados y estadísticas generadas por la aplicación, lo que les servirá para tomar medidas e informarse de la situacion sanitaria.
- Autoridades: podrán verificar que los ciudadanos están cumpliendo los periodos de cuarentena.
- Ambulatorios: dispondrán de listados donde se informarán del estado de los usuarios, pudiendo preveer que servicios pueden ofrecer. Asi como un medio, para comunicarle al
usuario que medidas debe tomar, periodo de cuarentena, pruebas a realizar, etc.

_(Esta sección debe contener información sobre los actores de negocio (organizaciones, roles
o responsabilidades) de los modelos de procesos de negocio actuales especificados mediante
las plantillas para actores del negocio actual que se muestran a continuación.)_

| **\<id>999** | \<nombre descriptivo> |
| -- | -- |
| **[Versión]** | <nº versión>(<fecha de versión>) |
| **[Dependencias]** | * \<procesos de negocio actuales en los que participa> <br> * ... |
| **Descripción** | Este actor de negocio actual representa a <descripción de la organización, rol o responsabilidad  a la que representa  el actor de negocio actual> |
| **Comentarios** | \<comentarios adicionales sobre el actor de negocio actual> |

<p align="center"> <b>Tabla 3: Actores de negocio.</b> <br> <i>Los atributos entre corchetes son opcionales</i> </p>


## 3.2.2 Descripción de Procesos de Negocio Actuales

Aquí se especificarán los procesos que debe llevar a cabo nuestra aplicación que llevarán un diagrama donde se detallarán los pasos a seguir. Según finalicen las entrevitas se irán añadiento y modificando los procesos. Inicialmente podemos pensar en estos como los procesos principales del programa:
- **Registrar un Usuario**: almacenaremos ¿localización?, estado y demás datos que trataremos de manera anónima para mantener un seguimiento que sea fácil de acceder pero que garantice que no se vulnera la protección de datos de dicho usuario.
- **Crear listados**: distintas listas con información útil sobre los usuarios para que los ambulatorios puedan acceder a ellas, de manera fácil y rápida.
- **Notificar a la autoridad**: proceso necesario en caso de incumplimiento del tiempo de cuarentena o falta de un prueba medica por parte de algún usuario.
- **Crear estadísticas**: En este procesos se almacenará toda la información útil para que las autoridades tanto sanitarias como fuerzas de seguridad puedan actuar a corte al impacto actual del coronavirus. También ayudará al usuario a ver de manera clara como está de afectada su zona o el país en general.
- **Contacto**: en este procedimiento se detallarán los pasos que deberá dar el usuario para comunicarse con las autoridades sanitarias, o fuerzas de seguridad para una mejor información de las medidas de seguridad.

_(Esta sección debe contener información sobre los procesos de negocio actuales, tal y como se realizan en la organización del cliente antes del comienzo del desarrollo del sistema software. Para cada proceso de negocio se incluirá una descripción textual usando las plantillas para procesos de negocio actuales que se muestran a continuación, y un diagrama en la notación que se considere oportuna, por ejemplo, diagramas BPMN (Business Process Model and Notation) o diagramas de actividad UML (Unified Modeling Language).)_

| **\<id>999** | \<nombre descriptivo> |
| -- | -- |
| **[Versión]** | <nº versión>(<fecha de versión>) |
| **[Dependencias]** | * \<procesos de negocio actuales en los que participa>  <br> * ... |
| **Descripción** | <descripción del proceso de negocio actual en términos del dominio del problema> |
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Actores]** | * \<actor que participa en el proceso de negocio> <br> * ... |
| **Comentarios** | \<comentarios adicionales sobre el actor de negocio actual> |

<p align="center"> <b>Tabla 4: Procesos de Negocio actuales.</b> <br> <i>Los atributos entre corchetes son opcionales</i> </p>

# 3.3 Entorno Tecnológico Actual



_(Esta sección debe contener información general sobre el entorno tecnológico en la organización del cliente antes del comienzo del desarrollo del sistema software, incluyendo hardware, redes, software, etc. Se prestará especial atención a la arquitectura de servicios (servicios web SOAP, REST, buses de servicios, etc.) en funcionamiento o en desarrollo que puedan tener impacto en el sistema software a desarrollar. El objetivo es ofrecer una visión general, por lo que para los detalles más técnicos se debe remitir al lector a los documentos técnicos oportunos. Para facilitar la comprensión, se recomienda el uso de diagramas donde sea posible. Esta sección se divide en las secciones que se describen a continuación, que pueden fusionarse si se considera oportuno.)_

## 3.3.1 Descripción del Entorno de Hardware Actual

Para que Radar Covid funcione es necesario un terminal (teléfonos de los usuarios), base de datos con datos anonimos que tienen identificadores de casos cofirmados. Incuimos tambien todo el soporte de red y la propia tecnologia Bluetooth.

_(Esta sección debe contener información sobre el entorno de hardware actual, incluyendo servidores, estaciones de trabajo, redes, etc., que pueda tener impacto sobre el sistema software a desarrollar. Para los detalles más técnicos se debe remitir al lector a los documentos técnicos oportunos. Para facilitar la comprensión, se recomienda el uso de diagramas donde sea posible.)_

## 3.3.2 	Descripción del Entorno de Software Actual

La antigüa aplicación está disponible tanto para android como para ios.

_(Esta sección debe contener información sobre el entorno de software actual, incluyendo sistemas operativos, sistemas de gestión de bases de datos, servidores de aplicaciones, etc., que pueda tener impacto sobre el sistema software a desarrollar. Para los detalles más técnicos se debe remitir al lector a los documentos técnicos oportunos. Para facilitar la comprensión, se recomienda el uso de diagramas donde sea posible.)_
