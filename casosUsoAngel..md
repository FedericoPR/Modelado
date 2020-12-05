| **\<id> CU 2.2** | Control humano por las autoridades (Ciudadanos sin móvil) |
| -- | -- |
| **[Versión]** | 1.0(04/12/2020) |
| **[Dependencias]** |Este caso de uso depende del CU 0.1 (Listar ciudadanos por estado), ya que debe de incluir dicho caso de uso. Dicho caso de uso interactua con el actor autoridades y el actor ciudadano. Ya que por medio de este caso se llevará un control por parte de las autoridades sobre el ciudadano.|
| **Precondición** | En el sistema se encuentra registrado un ciudadano que debe de cumplir cuarentena y no dispone de teléfono móvil. |
| **Descripción** | Los agentes de la autoridad podrán realizar un listado de los ciudadanos registrados en el sistema cuyo estado sea en cuarentena y sin teléfono móvil (CU 0.1 Listar ciudadanos por estado). De esta forma de obtendrá el listado de todos aquellos ciudadanos a los cuales no se les puede realizar un control del cumplimiento de la cuarentena de forma automática por el sistema. Por lo que será responsabilidad de los agentes de la autoridad llevar a cabo un control de la cuarenta de esta parte de la población, para ello realizará controles aleatorios en los domicilios de estos ciudadanos comprobando de que se encuentren en casa cumpliendo la cuarentena, en caso de que no se cumpla actuarán en consecuencia.|
| **Postcondición** | Se comprobará si se está llevando a cabo la cuarentena por el ciudadano.|
| **[Importancia]** | Media|
| **[Prioridad]** | Media|
| **[Estado]** | Pendiente|
| **Comentarios** |Este caso de uso solo afectará al pequeño porcentaje del 10% de la población española que no disponde de teléfono móvil y que enla mayoría de los casos se corresponde con personas mayores o ancianos.|

<p align="center"> <b>Tabla 11.2.2: Plantilla simplificada de casos de uso.</b> <br> </p>

| **\<id> CU 2.3** | Enviar alerta autoridades incumplimiento cuarentena. |
| -- | -- |
| **[Versión]** | 1.0(04/12/2020) |
| **[Dependencias]** |Este caso de uso depende del CU 2.1 (Control automático por el sistema del cumplimiento cuarentena.(Ciudadanos con móvil)), ya que si se detecta alguna anomalía en dicho caso de uso se dispararía este caso de uso, y también depende del CU 0.2 (Informar al ciudadano) cuando se detecte esa anomalía. Dicho caso de uso interactua con el actor autoridades. Ya que por medio de este caso se informará a las autoridades de que ha ocurrido un evento.|
| **Precondición** | Un cidadano con móvil que debe de cumplir la cuarentena no la está cumpliendo y es detectado por el sistema (CU 2.1 Control automático por el sistema del cumplimiento cuarentena.(Ciudadanos con móvil)) |
| **Descripción** | Dicho caso de uso es disparado cuando el CU 2.1 (Control automático por el sistema del cumplimiento cuarentena.(Ciudadanos con móvil)), detecta que un ciudadano con móvil no se encuentra en su domicilio cumpliendo con la cuarentena obligatoria. En esta situación, el sistema enviará un mensaje de alerta a la autoridades informándolas de que un ciudadano no está cumpliendo con la cuarentena, proporcionando toda la información disponible del ciudadano, incluyendo la ubicación de su dispositivo móvil para que pueda ser localizado por los agentes (siempre y cuando el móvil del ciudadano no se encuentre en su casa), de esta forma los agentes de la autoridad actuarán en consecuencia localizando al ciudadano. Al mismo tiempo de que se envía la alerta a las autoridades, se dispara el CU 0.2 (Informar al ciudadano), informándole por medio de un SMS de que no está cumpliendo la cuarentena y ha sido avisado a la autoridad.|
| **Postcondición** | Las autoridades habrán recibido una alerta sobre el incumplimiento de la cuarentena, con la información del ciudadano y el ciudadano habrá sido informado de ello.|
| **[Importancia]** | Alta|
| **[Prioridad]** | Alta|
| **[Estado]** | Pendiente|
| **Comentarios** |El como se deberá actuar para localizar al ciudadano que no cumple la cuarentena es competencia de las autoridades responsables.|

<p align="center"> <b>Tabla 11.2.3: Plantilla simplificada de casos de uso.</b> <br> </p>

| **\<id> CU 3.1** | Informar caso positivo. |
| -- | -- |
| **[Versión]** | 1.0(04/12/2020) |
| **[Dependencias]** |Este caso de uso depende del CU 1.2 (Registrar resultado de la prueba en el sistema) y que dicho resultado sea positivo, ya que si se detecta algun nuevo caso positivo se dispararía este caso de uso. Dicho caso de uso interactua con el actor Gobierno, ya que por medio de este caso se informará al gobierno de la ocurrencia de un nuevo caso positivo .|
| **Precondición** | Un ciudadano ha dado positivo en la prueba realizada. |
| **Descripción** | Dicho caso de uso es disparado cuando el CU 1.2 (Registrar resultado de la prueba en el sistema) registra una prueba que ha sido positiva. En esta situación, el sistema añadirá un nuevo caso positivo a un contador de casos positivos por centro de salud (en el contador correspondiente al centro de salud donde se ha detectado el caso positivo), dicha información con los contadores de casos positivos por centro de salud será siempre accesible por el gobierno, para que pueda ser consultada en cualquier momento y se conozca la información en tiempo real.|
| **Postcondición** | Se habrá registrado el caso postivo en el sistema de contadores de casos positivos por centro de salud al que puede acceder el gobierno.|
| **[Importancia]** | Alta|
| **[Prioridad]** | Alta|
| **[Estado]** | Pendiente|
| **Comentarios** |Dicha información será actualizada constantemente, cada vez que un nuevo caso positivo es registrado en el sistema, a diferencia del CU 3.3 (Informar estadísticas), las cuales serán proporcionadas al gobierno de forma periódica cada 3 días o el tiempo fijado.|

<p align="center"> <b>Tabla 11.3.1: Plantilla simplificada de casos de uso.</b> <br> </p>

| **\<id> CU 3.3** | Informar estadísticas |
| -- | -- |
| **[Versión]** | 1.0(05/12/2020) |
| **[Dependencias]** |Este caso de uso depende del CU 3.2 (Generar estadísticas) ya que antes de poder informar las estadísitcas deben de ser generadas (dependencia de tipo include). Dicho caso de uso interactua con el actor Gobierno, ya que por medio de este caso se informará al gobierno de las estadísitcas generadas por el sistema .|
| **Precondición** | El sistema ha generado estadísticas a partir de los datos que dispone. CU 3.2 (Generar estadísticas) |
| **Descripción** | Dicho caso de uso es disparado cuando el CU 3.2 (Generar estadíticas) genera nuevas estadísticas a partir de los datos disponibles en el sistema. En esta situación, el sistema mostrará un informe estadístico con todas las estadísticas obtenidas en el CU 3.2 y se enviará un aviso al sistema del gobierno informándole de que están disponibles nuevas estadísiticas obtenidas a partir de los datos recopliados en los últimos 3 días o el tiempo marcado, para que las pueda visualizar en el sistema y a partir de ellas, el comité de expertos del gobierno puedan tomas las decisiones oportunas.|
| **Postcondición** | Se habrán proporcionado las estadísticas al gobierno y se le habrá mandado un aviso para que puedan visualizarlas en el sistema.|
| **[Importancia]** |Muy Alta|
| **[Prioridad]** | Alta|
| **[Estado]** | Pendiente|
| **Comentarios** |La información relevante a las estadísitcas será proporcionada al gobierno de forma periódica cada 3 días o el tiempo fijado. Dado que se necesita disponer de un gran volumen de datos recopilados durante varios dias para que dichas estadísticas sean lo mas fiables posibles.|

<p align="center"> <b>Tabla 11.3.3: Plantilla simplificada de casos de uso.</b> <br> </p>

| **\<id> CU 2.1** | Control automático por el sistema del cumplimiento cuarentena.(Ciudadanos con móvil). |  |
| --- | --- | --- |
| **[Versión]** | 1.0 (05/12/2020)|
| **[Dependencias]** | Dicho caso de uso depende del CU 0.2 (Listar ciudadanos por estado) para obtener aquellos ciudadanos registrados en el sistema que deben de cumplir cuarentena. También depende del CU 2.3 (Enviar alerta autoridades incumplimiento cuarentena), ya que cuando se detecte un ciudadano que no está cumpliendo la cuarentena se informará a las autoridades. Este caso de uso deberá interactuar con las operadoras teléfonicas para poder obtener la localización en tiempo real del dispositivo móvil del ciudadano.|
| **Precondición** | En el sistema se encuentra registrado un ciudadano que debe de cumplir cuarentena y dispone de teléfono móvil.|
| **Descripción** | El sistema será capaz de detectar cuando un ciudadano que dispone de teléfono móvil esta incumpliendo la cuarentena, en dicho caso lo informará a las autoridades para que actuen en consecuencia.  |
| **Secuencia Normal** | **Paso** | **Acción** |
|  | 1 | El sistema obtendrá un listado con los ciudadanos que deban cumplir cuarentena y dispongan de teléfono móvil con desbloqueo por huella dactilar. CU 0.1 (Listar ciudadanos por estado). |
|  | 2 | Cada 10 minutos el sistema debe de hacer un sondeo, solicitando la localización del dispositivo del ciudadano a las operadoras telefónicas. Si la localización del dispostivo del ciudadano es distinta a la del domicilio del ciudadano se disparará el CU 2.3 (enviar alerta a las autoridades), y se informará al ciudadano de ello, y terminaría el CU. En caso contrario, se continuaría con el flujo normal del CU. |
|  | 3 | El sistema enviará en un periodo de tiempo aleatorio desbloquear el móvil al ciudadano por medio de la huella dactilar y al hacerlo se tomará una foto del ciudadano. |
|  | 4 | Si pasada una hora el ciudadano no desbloquea el teléfono móvil, se disparará el CU 2.3 (enviar alerta a las autoridades) y termina el CU actual. En caso contrario si se desbloquea el móvil se comprobará que la foto tomada al desbloquear el móvil se corresponde al ciudadano (sistema de reconocimiento facial) y se comprobará que el dispositivo se encuentra en el domicilio del ciudadano. |
|  | 5 | El sistema reconoce que el ciudadano se encuentra en su domicilio cumpliendo la cuarentena y termina. |
| **Postcondición** | El sistema habrá comprobado que el ciudadano se encuentra en casa cumpliendo la cuarentena y en caso contrario se habrá disparado el CU 2.3 (enviar alerta a las autoridades) para que actuen en consecuencia. |
| **Excepciones** | **Paso** | **Acción** |
|  | 1 | El sistema actuará de distinta forma si los ciudadanos que deben cumplir cuarentena disponen de teléfono móvil sin desbloqueo por huella dactilar.En este caso un agente de la autoridad realizará una videollamada con el ciudadano comprobando que es el, y se obtendrá la localización del teléfono móvil en ese momento. En caso de que no se corresponda con el ciudadano, o el ciudadano no responda a la llamada en un máximo de una hora, o el teléfono del ciudadano no se encuentra en su domicilio se disparará el CU 2.3|
| **Rendimiento** | **Paso** | **Cota de tiempo** |
| | El CU no debe de tardar en ser ejecutado un tiempo superior a  |10 segundos|
| **Frecuencia** | El CU debe de llevarse a cabo de forma constante en segundo plano, realizando sondeos cada 10 minutos de la localización de los teléfonos de los ciudadanos comprobando que se encuentra en su domicilio, o cada un periodo de tiempo aleatorio, se debe de pedir desbloquear el teléfono móvil del ciudadano.|
| **[Importancia]** | Muy Alta|
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | El CU afecta al 90% la población española que dispone de teléfono móvil. Dicho caso de uso es complemenatario al CU 2.2 Control humano por las autoridades (Ciudadanos sin móvil), el cual solo afecta a la población que no posee teléfono móvil.|
<p align="center"> <b>Tabla 12.2.1: Plantilla Completa de Casos de Uso.</b> <br> </p>

| **\<id> CU 3.2** | Generar estadísticas |  |
| --- | --- | --- |
| **[Versión]** | 1.0 (05/12/2020)|
| **[Dependencias]** | Dicho caso de uso depende del CU 1.2 (Registrar resultado de la prueba en el sistema) y el resultado es positivo. También depende del CU 1.3 ( Rastrear contactos directos con el postivo), ya que a partir de la información proporcionada por dichos casos de uso, el caso de uso generar estadísticas podrá obtener las estadísitcas sobre la población. De este caso de uso también depende el CU 3.3 (Informar estadísticas), dado que una vez que se han obtenido las estadísitcas, se disparará el CU 3.3.|
| **Precondición** | El sistema dispone de los datos de los casos positivos y de los contactos directos entre los positivos.|
| **Descripción** | El sistema deberá obtener estadísitcas a cerca de los contagios producidos, detectando los posibles focos de contagio entre los ciudadanos, las zonas que se encuentran más expuestas al virus, la población más proprensa a ser contagiada, etc para que se pueda disparar el CU 3.3 y se informen de todas estas estadísticas al comité de expertos del gobierno para que tomen las medidas necesarias. |
| **Secuencia Normal** | **Paso** | **Acción** |
|  | 1 | El sistema consultará los datos de los casos positivos registrados. |
|  | 2 | El sistema consultará los datos relativos a los contactos directos entre los casos positivos y si estos han sido positivos. |
|  | 3 | El sistema consultará el lugar donde se han producido los contactos entre los contagiados.|
|  | 4 | El sistema aplicará un algoritmo inteligente para obtener relaciones entre los contagios, los lugares de contagio, etc cruzando los datos para obtener las estadísticas oportunas. |
|  | 5 | Se almacenan en el sistema las estadísticas obtenidas como un informe al que podrá acceder el gobierno. |
|  | 6 | Se dispara el CU 3.3 (Informar estadísticas) |
|  | 7 | Se dispara el CU 3.4 (Informar foco de contagio) |
| **Postcondición** | El sistema habrá generado estadísticas a partir de los datos de contagios y contactos que disponía, detectando posibles focos de contagio, zonas más expuestas al virus, población más propensa a ser contagiada,etc. |
| **Excepciones** | **Paso** | **Acción** |
|  | 2 | Si el caso positivo registrado es un caso aislado, se comtabilizará en las estadísticas como un caso aislado.|
| **Rendimiento** | **Paso** | **Cota de tiempo** |
| | El CU debe de llevarse a cabo en un tiempo no superior a|1 hora|
| **Frecuencia** | El CU debe de llevarse a cabo una vez cada 3 días.|
| **[Importancia]** | Muy Alta|
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | El CU debe de realizarse con poca fecuencia para que las estadísticas obtenidas sean lo mas reales posibles obtenidas de grandes volúmenes de datos, por ello mismo el tiempo que implica llevar a cabo el caso de uso es grande. |
<p align="center"> <b>Tabla 12.3.2: Plantilla Completa de Casos de Uso.</b> <br> </p>