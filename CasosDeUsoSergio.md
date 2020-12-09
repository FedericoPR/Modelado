
| **CU 1.4** | Adquirir datos de los ciudadanos |
| -- | -- |
| **[Versión]** | 1.0 (04/12/2020) |
| **[Dependencias]** |  |
| **Precondicion** | Las operadoras deberán tener acceso al sistema para poder suministrar los datos de los cuidadanos o bien el administrador del sistema los recibirá de las operadoras y los incorporará al sistema  |
| **Descripción** | Este caso de uso consiste en el aporte de todos los datos de los cuidadanos por parte de la operadora telefónica. Más adelante estos datos serán imprescindibles para hacer el rastreo de los posibles contactos |
| **Postcondicion** | Los datos de los cuidadanos quedarán reflejados en el sitema de manera que puedan ser utilizados por los algoritmos para poder realizar los cruces de información y rastrear los posibles contagiados |
| **[Importancia]** | Muy Alta |
| **[Prioridad]** | Alta |
| **Estado** |  |
| **Comentarios** | Debido a la importancia de esta información para poder realizar la mayor parte de las funciones del sistema esta deberá estar lo más actualizada posbible. Por ello el encargado de administrar esta información para el sistema deberá actualizar la misma con mucha frecuencia |

| **CU 1.5** | Registrar contactos directos en el sistema |
| -- | -- |
| **[Versión]** | 1.0 (04/12/2020) |
| **[Dependencias]** |  |
| **Precondicion** | El ciudadano a registrar habrá sido identificado anteriormente por el algoritmo como posible positivo |
| **Descripción** | Una vez el algoritmo nos proporciona aquellos ciudadanos que han tenido contacto suficiente con un positivo y, por tanto, son susceptibles de ser positivos pasaremos a registrar a estos ciudadanos en el sistema. En este primer registro se pondrá al ciudadano con el estado "Pendiente de cita" para que el responsable del ambulatorio sepa que deberá concretar una cita con él para realizarse las pruebas pertinentes |
| **Postcondicion** | El ciudadano quedará registrado en el sistema como pendiente de concretar una cita lo antes posible para realizarse las puebas y se le inromará de que deberá guardar cuarentena haste ese momento|
| **[Importancia]** | Alta |
| **[Prioridad]** | Media |
| **Estado** |  |
| **Comentarios** | Una vez se guarda el cuidadano como posible positivo los responsables de llamarlo y concretar cita deberán intentar que esa cita para la realización de las pruebas no tarde para ser lo más eficientes posibles en evitar la propagación de un usuario que puede que esté contagiado|

| **CU 1.6** | Registrar cita pruebas en el sistema |
| -- | -- |
| **[Versión]** | 1.0 (04/12/2020) |
| **[Dependencias]** |  |
| **Precondicion** | El usuario debe haber sido detectado por el algoritmo y registrado en el sistema para que aparezca como pendiente de cita al filtrar para que el ambulatorio se ponga en contacto |
| **Descripción** | Tras haber detectado un posible positivo con los datos de rastreo por parte del algoritmo y haber sido registrado el usuario en el sistema, el responsable sanitario del ambulatorio al que pertenece el cuidadano se pondrá en contacto con él para concretatar la cita en la que se le realizarán las pruebas. Una vez se concrete la cita el responsable lo registrará en el sistema|
| **Postcondicion** | El usuario quedará como pendiente de realizar las pruebas y se le infromará de que permanezca en cuarentena hasta la realización de las mismas. Esta cuarentena no será controlada por las fuerzas de seguridad debido a que no se trata de un positivo confirmado por lo que se intentará dar la cita lo antes posible |
| **[Importancia]** | Alta |
| **[Prioridad]** | Media |
| **Estado** |  |
| **Comentarios** | |

| **CU 1.7** | Enviar alerta a las autoridades de incumplmiento de realizarse la prueba|
| -- | -- |
| **[Versión]** | 1.0 (04/12/2020) |
| **[Dependencias]** |  |
| **Precondicion** | La fecha de cita deberá ser 24 h inferior a la fecha actual para que se alerte a las autoridades |
| **Descripción** | Una vez se registra una cita para el ciudadano, este deberá acudir en el día y la hora previstas para la realización de la prueba. En caso de no acudir a la cita el sistema alertará al usuario de que no se ha ralizado la prueba en la cita que se registró y que dispone de 24 h para volver a llamar en vistas a explicar su situación y/o los motivos por los cuales no ha acudido así como para coincretar una nueva cita. En caso de que finalice este plazo de 24 h y el ciudadano no se haya puesto en contacto para acordar una nueva cita, es decir, el registro siga teniendo una fecha de cita que ha vencido hace más de 24 h, el sistema de manera automática enviará otro mensaje al cuidadano y tambén alertará a las fuerzas del orden de esta situación de incumplimiento por parte del ciudadano. |
| **Postcondicion** | La fecha de cita seguirá siendo una fecha pasada hasta aclarar la situación por parte de las autoridades |
| **[Importancia]** | Media |
| **[Prioridad]** | Media |
| **Estado** |  |
| **Comentarios** | Si el usuario llamara para cambiar la cita pasadas 24 horas, bien por actuación de las autoridades, o bien por descuido personal durante las 24 h de plazo, las autoridades serían informadas también|

| **CU 3.4** | Informar foco de contagio |
| -- | -- |
| **[Versión]** | 1.0 (04/12/2020) |
| **[Dependencias]** |  |
| **Precondicion** | Una vez se confirme un contagiado pos otro positivo, por medio de los datos de localizacion estableceremos cual ha sido el punto más probable donde se ha producido el contagio, en caso de haber más de uno. |
| **Descripción** | Con todos los datos de los que el sistema dispone, de contagios, lugar donde se produce el contagio, número de contagios...etc por medio de algoritmos generará una serie de estadísticas que nos permitiran averiguar cuales son los lugares donde más se contagian los ciudadanos. Cuando estos valores lleguen a ciertos parámetros previamente establecidos etiquetaremos este lugar como "foco de conagio" del cual se informará al gobierno para que tome las medidas oportunas|
| **Postcondicion** | Una vez se llegue a ciertos valores de numero de contagiados en una zona supondrá informar de esta situación al gobierno |
| **[Importancia]** | Alta |
| **[Prioridad]** | Media |
| **Estado** |  |
| **Comentarios** | |


| **\<id> CU 1.3** | Rastrear contactos directos con el postivo |  |
| --- | --- | --- |
| **[Versión]** | 1.0 (09/12/2020)|
| **[Dependencias]** | Dicho caso de uso depende del CU 1.2 (Registrar resultado de la prueba en el sistema) para alertar al sistema de que se ha detectado un positivo y de que deberá utilizar los datos de los que dispone para identificar aquellos ciudadasno que puedan haber contactado lo suficiente con el postitivo. También depende del CU 1.4 (Adquirir datos de los ciudadanos), ya que necesitará de todos los datos de localización de los ciudadanos para que el algoritmo pueda realizar los cruces e identificar los ciudadanos susceptibles de haber sido contagiados|
| **Precondición** | En el sisteme deben estar los datos de los ciudadanos suministrados por las operadoras y deberá saltar un caso positivo para que el sistema empiece a trabajar en los rastreos|
| **Descripción** |  Una vez se registra un positivo en la pruebas realizadas a algún ciudadano, este resultado es introducido en el sistema. En ese momento el algoritmo de rastreo comenzará su trabajo. Para ello tendrá en cuenta y trabajará con todos los datos previamente suministrados por las operadoras móviles, cotejará y contrastará las ubicaciones de los ciudadanos que coincidan en lugar y momento con las del postivo para establecer cuales de ellos pueden haber sido contagiados por cumplir los parámetros de contacto necesarios para contagiarse. Cuando el sistema concluye su análisis suministrará los datos de aquellos ciudadanos que puedan ser positivos y para que sean registrados en el sistema como pendientes de realizar la prueba junto con  el lugar donde es más probable que se haya producido el contagio, para tenerlo en cuenta en las estadísticas. Una vez loa ambulatorios dispongan de los datos aportados por este rastreo comenzarán a informar a los cuidadanos de su situación y a concretar citas con los mismos|
| **Secuencia Normal** | **Paso** | **Acción** |
|  | 1 | El sistema detectará que se ha introducido un nuevo positivo en el sistema y comenzará el rastreo con respecto a él CU 1.2 (Registrar resultado de la prueba en el sistema) |
|  | 2 | El algoritmo detectará aquellos cuidadanos que puedan estar infectados teniendo en cuenta los datos de las operadoras CU 1.4 (Adquirir datos de los ciudadanos) |
|  | 3 | El sistema elaborará una lista de los cuidadanos que ha detectado para que se registren en el sistema así como el punto de contagio y los ambulatorios registrarán estos datos CU 1.1(Registrar resultado de la prueba en el sistema) |
|  | 4 | Los ambulatorios se encargarán de ponerse en contacto con los posibles positivos para concretar con ellos una cita en la cual realizarse la pureba CU 1.6 (Registrar cita pruebas en el sistema) que en caso de dar positivo empezaría de nuevo el caso de uso que se está tratando (CU 1.3 "Rastrear contactos directos con el postivo") |
| **Postcondición** | El sistema registrará todos los cuidadanos que puedan haber sido contagiados para que se les realicen las pruebas y continuará con el ciclo en cada uno de los postivos encontrados de esta manera |
| **Excepciones** | **Paso** | **Acción** |
|  | 1 | El sistema identificará en el rastreo aquellos cuidadanos a los cuales se ha establecido como positivos una única vez para no caer en bucles infinitos de positivos|
| **Rendimiento** | **Paso** | **Cota de tiempo** |
| | El rastreo como tal de cuidadanos que pueden estar contagiados no debe de tardar en ser ejecutado un tiempo superior a 100 segundos, que es bastante tiempo pero es un porceso muy complejo y seguramente el más importante del poryecto por lo que es mejor que sea preciso en sacrificio de su rapidez | 1'40''|
| **Frecuencia** | El CU debe de llevarse a cabo cada vez que se registre un positivo en el sistema|
| **[Importancia]** | Muy Alta|
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** ||
