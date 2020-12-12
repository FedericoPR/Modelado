#### 6.3.1 Requisitos de Reglas de Negocio del Sistema
Aunque contemos con el apoyo del ministro, nuestra aplicación debe cumplir con aquellas limitaciones y leyes impuestas por el entorno. Nos centraremos principalmente en el tratamiento de los datos de los ciudadanos al ser información sensible.

Esta sección debe contener las reglas de negocio que deba cumplir el sistema a desarrollar, especificadas mediante las plantillas para reglas de negocio que se muestran a continuación.
Estos requisitos deben especificar qué reglas de negocio debe respetar el sistema, evitando que se incumplan durante su funcionamiento.

| **\<id>001** | Cumplimiento de la Ley de protección de datos |
| -- | -- |
| **[Versión]** | 1.0 (11/12/2020) |
| **[Dependencias]** | El requisito depende del requisito general gestionar información recopilada y proporcionar estadisticas al gobierno. También depende del requisito 1 de información (Datos de los ciudadanos) |
| **Descripción** | El sistema deberá cumplir con la ley de proteccion de datos para que la información sensible del ciudadano, no se pueda compartir o utilizar indebidamente. |
| **[Importancia]** | Muy alta |
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | [Ley Orgánica 3/2018, de 5 de diciembre, de Protección de Datos Personales y garantía de los derechos digitales.](https://www.boe.es/buscar/act.php?id=BOE-A-2018-16673) |
<p align="center"> <b>Tabla 14.1: Requisitos de reglas de negocio.</b> <br> </p>

| **\<id>002** | Anonimozar datos ciudadanos |
| -- | -- |
| **[Versión]** | 1.0 (11/12/2020) |
| **[Dependencias]** | El requisito depende del requisito general gestionar información recopilada y proporcionar estadisticas al gobierno. También depende del requisito 1 de información (Datos de los ciudadanos) |
| **Descripción** | El sistema deberá anonimizar los datos de los ciudadanos a aquellos que no tengan la autorización. |
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | Como llevamos comentando a lo largo de la práctica, el hecho de poder acceder a los datos de los ciudadanos por las operadoras no obliga a gestionar dichos datos y evitar que sea visibles a agentes externos sin autorizar que podrían aprovecharse de estos. Además del derecho fundamental a la intimidad |
<p align="center"> <b>Tabla 14.2: Requisitos de reglas de negocio.</b> <br> </p>

| **\<id>003** | Destruir información inservible del ciudadano |
| -- | -- |
| **[Versión]** | 1.0 (11/12/2020) |
| **[Dependencias]** | El requisito depende del requisito general gestionar información recopilada y proporcionar estadisticas al gobierno. También depende del requisito 1 de información (Datos de los ciudadanos), tambien en el requisito de Rastreo de contactos con positivo que en el caso de que el ciudadano de negativo en las pruebas se borrará de la lista que genera dicho requisito.|
| **Descripción** | El sistema deberá destruir la información relativa al ciudadano una vez sea inservible para facilitar su uso y busqueda a la hora de crear listas o de generar notificaciones a los actores correspondientes. |
| **[Importancia]** | Alta |
| **[Prioridad]** | Media/Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | Este requisito es de vital importancia para evitar la saturación del sistema ya que contamos con un gran volumen de datos a manejar. Este requisito aumentara la organización y eficacia en la gestión de los datos de lso ciudadanos. |
<p align="center"> <b>Tabla 14.3: Requisitos de reglas de negocio.</b> <br> </p>

| **\<id>004** | Adaptación de la información según la autonomía |
| -- | -- |
| **[Versión]** | 1.0 (11/12/2020) |
| **[Dependencias]** | Este requisito depende del requisito general gestionar la información recopilada y proporcionar estadísticas al gobierno |
| **Descripción** | El sistema deberá adaptar su comunicación con los sistemas de información de cada autonomía. |
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | Este requisito viene dado por la naturaleza de la gestión de las autonomías. Donde cada una esta en diferentes fases para combatir el virus y además cuentan con una distribución urbana diferente. Es decir la organización y recopilación de datos afecta a como estos se van a organizar según en que atutonomía nos encontremos. |
<p align="center"> <b>Tabla 14.4: Requisitos de reglas de negocio.</b> <br> </p>

