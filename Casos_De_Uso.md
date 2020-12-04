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
*  SUBSISTEMA GESTIÓN DEL CUMPLIMIENTO DE CUARENTENA:
    * CU 2.1: Control automático por el sistema del cumplimiento cuarentena.(Ciudadanos con móvil).
    * CU 2.2: Control humano por las autoridades (Ciudadanos sin móvil).
    * CU 2.3: Enviar alerta autoridades incumplimiento cuarentena.
* SUBSISTEMA GESTIÓN DE INFORMACIÓN Y ESTADÍSTICAS AL GOBIERNO:
    * CU 3.1: Informar caso positivo.
    * CU 3.2: Generar estadísticas.
    * CU 3.3: Informar estadísticas.
    * CU 3.4: Informar foco de contagio. 


A continuación, se especificarán aquellos casos de uso que hemos considerado de menos importancia para el sistema: