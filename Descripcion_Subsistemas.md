## 5. DESCRIPCIÓN DE LOS SUBSISTEMAS DEL SISTEMA A DESARROLLAR
Para la mejor compresión de la plataforma PANDEMIO que se deseea implementar, dividiremos dicha plataforma en distintos módulo que agruparán las funcionalidades necesarias. Estos subsistemas estarán descritos con mayor detalle en las siguientes tablas. Nos basamos en el diagrama de características del apartado de alcance (1.1).

Esta sección opcional debe contener una descripción de los subsistemas del sistema a desarrollar, especificados mediante las plantillas para subsistemas que se muestran
a continuación. En el contexto de este documento, los subsistemas son agrupaciones lógicas de requisitos cuya finalidad es facilitar la comprensión de los mismos,
por lo que no implican necesariamente la existencia de subsistemas o módulos software correspondientes en las siguientes fases de desarrollo. Para facilitar la comprensión,
se recomienda el uso de diagramas donde sea posible.
Los subsistemas a los que se hace referencia en esta sección puede que ya se hayan definido total o parcialmente en documentación previa como el Pliego de Prescripciones Técnicas,
la Oferta seleccionada o el Estudio de Viabilidad del Sistema, en cuyo se podrán reutilizar y se hará referencia a dichos documentos como fuente de los mismos.

| **\<id>001** | Rastreo de contacto entre casos positivos y Gestion de Pruebas Médicas|
| -- | -- |
| **[Versión]** | 1.0 (29/11/2020) |
| **[Dependencias]** | * Rastreo del contacto con un positivo> <br> * Identificar posibles focos de contagio <br> Rastrear contactos con los casos positivos. |
| **Descripción** | Este subsistema agrupa los requisitos relacionados con el seguimiento de aquellos que han dado positivo en las pruebas, para así crear una lista de las personas afectada y todo aquello que tenga que ver con el rastreo de casos positivos para poder identificar posibles focos de contagio.  |
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Prioridad]** | * Alta |
| **Comentarios** | \<comentarios adicionales sobre el subsistema> |

<p align="center"> <b>Tabla 8.1: Subsistemas a desarrollar.</b> <br> </p>

| **\<id>002** | Gestión de cumplimiento de cuarentena |
| -- | -- |
| **[Versión]** | 1.0 (29/11/2020) |
| **[Dependencias]** | * Asegurar el cumplimineto de la cuarentena <br> Suministrar información y estadísticas al gobierno <br> * Gestionar el cumplimiento de la cuarentena |
| **Descripción** | Este subsistema agrupa los requisitos relacionados con el control de aquellos que han dado positivo en la prueba y asegurandose que los pacientes cumplen el periodo de cuarentena. En caso de incumplimiento se notificara a las autoridades. |
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Prioridad]** | * Alta |
| **Comentarios** | \<comentarios adicionales sobre el subsistema> |

<p align="center"> <b>Tabla 8.2: Subsistemas a desarrollar.</b> <br> </p>

| **\<id>003** | Gestión de información y estadísticas al gobierno |
| -- | -- |
| **[Versión]** | 1.0 (29/11/2020) |
| **[Dependencias]** | * Identificar posibles focos de contagio <br> Suministrar información y estadísticas al gobierno <br> * ... |
| **Descripción** | Este subsistema agrupa los requisitos relacionados con la información que se proporcionará al gobierno por parte de los ambulatorios. Estos datos generan las distintas estadísticas que permitirán localizar los focos de contagio para que así el gobierno pueda tomar las decisiones oportunas. |
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Prioridad]** | * Media |
| **Comentarios** | \<comentarios adicionales sobre el subsistema> |

<p align="center"> <b>Tabla 8.3: Subsistemas a desarrollar.</b> <br> </p>

Esta sección podrá omitirse si el sistema software a desarrollar es lo suficientemente sencillo como para no ser dividido en subsistemas.
