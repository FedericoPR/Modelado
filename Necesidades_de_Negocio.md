## 4. NECESIDADES DE NEGOCIO

Una vez que ya somos conscientes de cual es el dominio del problema y tenemos una visión mucho más clara y concisa de cuál es la situación actual debemos establecer aquellos puntos que vamos a necesitar cumplir para llegar a unos objetivos marcados y tangibles. 

Tenemos que tener claro en todo momento que el objetivo principal de nuestro sistema va a ser la reducción de la propagación del virus y por consiguiente la disminución del numero de contagios. Para poder cumplir con el objetivo principal, centraremos nuestros esfuerzos en la detección de positivos en torno a un positivo confirmado y en la confirmación del cumplimiento de la cuarentena de los contagiados.

Para poder llevar un control preciso sobre el avance y el cumplimiento de los objetivos establecidos con el cliente acotaremos estos objetivos como necesidades de negocio que podremos medir.


### 4.1 Objetivos de Negocio

Una vez nuestro sistema sea funcional y esté en producción deberá llevar a cabo ciertos requerimientos para los cuales ha sido concebido. De esta manera queremos dejar plasmados los siguientes objetivos de negocio para poder demostrar en qué medida el sistema realiza su función.

| **\<id>001** | Reducir la propagación del virus y el número de contagios en la pandemia actual o en futuras pandemias. |
| -- | -- |
| **[Versión]** | 1.0 (29/11/2020) |
| **[Dependencias]** | Objetivo de negocio padre, de el dependen el resto de objetivos de negocio. |
| **Descripción** | El objetivo principal de la plataforma a desarrollar es que el número de contagios de la pandemia disminuya y así poder hacer frente a la actual pandemia, así como disponer de una plataforma funcional por si en un futuro se presenta una situación parecida. De esta forma, podremos actuar y poner en marcha esta plataforma disminuyendo los efectos negativos que se puedan presentar. Para poder implementar esta plataforma, se deberán cumplir con ciertos subobjetivos de negocio que dependen totalmente de este objetivo principal, los cuales se indican en el apartado de subobjetivos y dependencias.|
| **Subobjetivos** | Para poder cumplir con este objetivo principal, se deberán cumplir con ciertos subobjetivos u objetivos hijos, los cuales son: <br>* 002 Rastreo del contacto con un positivo. <br> * 003 Asegurar la realización de las pruebas. <br>* 004 Identificar posibles focos de contagio. <br> * 005 Asegurar el cumplimiento de la cuarentena. <br> * 006 Proporcionar información y datos al ministerio.|
| **[Importancia]** | Muy Alta|
| **[Prioridad]** | Alta|
| **Comentarios** | Es el objetivo principal del proyecto, el objetivo padre del que dependen el resto de los objetivos que nos encontramos en el proyecto. |

<p align="center"> <b>Tabla 5.1: Objetivos de Negocio: Rastreo del contacto con un positivo</b> <br> </p>


| **\<id>002** | Rastreo del contacto con un positivo |
| -- | -- |
| **[Versión]** | 1.0 (29/11/2020) |
| **[Dependencias]** | Es hijo y por tanto depende del proceso de negocio 001 Reducir la propagación del virus y el número de contagios en la pandemia actual o en futuras pandemias. Depende del proceso de negocio a implementar 001 Rastrear contactos con los casos positivos.|
| **Descripción** | Una vez tenemos un positivo en la prueba realizada al usuario procederemos al rastreo por medio de los datos de las operadoras de todos aquellos usuarios susceptibles de estar contagiados. El objetivo ideal sería ser capaces de obtener el 100% de las personas que hayan mantenido un contacto suficiente con la persona que ha dado positivo para poder realizarles las pruebas. Como es prácticamente imposible llegar al 100% de personas que han contactado con el positivo por motivos que escapan a nuestro control ausencia de dispotivo movil en el momento del contacto, fallos o imprecisiones en el posicionamiento GPS... consideraremos aceptable poder identificar y contactar con todos aquellos que el sistema nos marque como objetivos y lo estimaremos en un 80% de los casos reales, por los inconvenientes citados anteriormente.|
| **Subobjetivos** | Como objetivo hijo tiene el objetivo 004 Identificar posibles focos de contagio.|
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **Comentarios** |  |

<p align="center"> <b>Tabla 5.2: Objetivos de Negocio: Rastreo del contacto con un positivo</b> <br> </p>

| **\<id>003** | Asegurar la realización de las pruebas |
| -- | -- |
| **[Versión]** | 1.0 (29/11/2020) |
| **[Dependencias]** | Es hijo y por tanto depende del proceso de negocio 001 Reducir la propagación del virus y el número de contagios en la pandemia actual o en futuras pandemias. Depende del proceso de negocio a implementar 002 Gestionar la realización de las pruebas médicas. |
| **Descripción** | Una vez hemos contactado con todas aquellas personas que han mantenido el suficiente contacto con un positivo como para ser consideradas como posibles contagiadas tendremos que asegurarnos de que estas se realizan las pruebas pertinentes para confirmar o no si han sido contagiadas. Para ello pondremos a disposición de los ambulatorios y de las autoridades competentes los datos del usuario para que puedan informarlo y realizarle las pruebas con la mayor rapidez posible. El objetivo ideal sería que el 100% de los contactos susceptibles de ser positivos pudieran ser localizados y se les ralizaran las pruebas; sin embargo habrá situaciones que se escapen a nuestro control e incluso a de las autoridades, como por ejemplo la falta de información del usuario por parte de la operadora, la posibilidad de tener unos datos desactualizados del usuario...Por ello consideraremos aceptable llegar a realizar las pruebas al 90% de los usuarios que pueden haber sido contagiados por un caso confirmado.|
| **Subobjetivos** |  |
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **Comentarios** |  |

<p align="center"> <b>Tabla 5.3: Objetivos de Negocio: Asegurar la realización de las pruebas</b> <br> </p>

| **\<id>004** | Identificar posibles focos de contagio |
| -- | -- |
| **[Versión]** | 1.0 (29/11/2020) |
| **[Dependencias]** | Es hijo y por tanto depende del proceso de negocio 001 Reducir la propagación del virus y el número de contagios en la pandemia actual o en futuras pandemias, también es un subobjetivo del objetivo 002 Rastreo del contacto con un positivo . Depende del proceso de negocio a implementar 001 Rastrear contactos con los casos positivos. |
| **Descripción** | Combinando los datos de los usuarios que tenemos con los resultados de las pruebas realizadas podemos establecer aquellas zonas y lugares donde se producen más contagios. Una vez obtenemos una prueba positiva realizamos el rastreo de aquellos usuarios que pueden haber sido contagiados por haber estado en contacto directo en un mismo lugar durante un tiempo determinado con el positivo. Si los usuarios localizados también dan positivo en la prueba que se les realice podremos establecer dónde se ha producivo el contagio. Con todos los datos reunidos de esta manera podemos establecer las "zonas calientes" donde se han producido más contagios para poder poner en alerta a los organismos competentes o a los usuarios de estas localizaciones. Como no podemos asegurar que el contagio se produjo al 100% en un lugar, ya que puedes contagiarte por contacto con un asintomático estableceremos como punto aceptable la determinación de los focos de contagio con un nivel de fiabilidad del 90%.|
| **Subobjetivos** |  |
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **Comentarios** | |

<p align="center"> <b>Tabla 5.4: Objetivos de Negocio: Identificar posibles focos de contagio</b> <br> </p>

| **\<id>005** | Asegurar el cumplimiento de la cuarentena |
| -- | -- |
| **[Versión]** | 1.0 (29/11/2020) |
| **[Dependencias]** | Es hijo y por tanto depende del proceso de negocio 001 Reducir la propagación del virus y el número de contagios en la pandemia actual o en futuras pandemias. Depende del proceso de negocio a implementar 003 Gestionar el cumplimiento de la cuarentena. |
| **Descripción** | Una vez tenemos un resultado postitivo de las pruebas pondremos a disposición de los cuerpos de seguridad del estado y de los ambulatorios los datos del usuario para poder informar al usuario de su situación de cuarentena desde ese mismo momento y para poder llevar a cabo un control exahustivo de la misma. Puesto que tenemos los datos de localización por medio del movil de los usuarios y podemos suministrarselos a las autoridades para que se aseguren de que el usuario permanezca en su domicilio durante la cuarentena podemos obtener un 100% de cumplimiento de las mismas.El inconveniente de este método es que los usuarios podrán evadir el cumplimiento de la cuarentena mientras el móvil permaneza en el domicilio. Para ello las autoridades realizarán llamadas o inspecciones domiciliares asegurarse de que el usuario esté en casa. Aún así sera imposible asegurar el 100% de las cuarentenas enteras por lo que establecemos como un objetivo aceptable que se logren cumplir el 90% de las mismas.|
| **Subobjetivos** |  |
| **[Importancia]** | Alta|
| **[Prioridad]** | Alta |
| **Comentarios** |  |

<p align="center"> <b>Tabla 5.5: Objetivos de Negocio: Asegurar el cumplimiento de la cuarentena</b> <br> </p>

| **\<id>006** | Proporcionar información y datos al ministerio |
| -- | -- |
| **[Versión]** | 1.0 (29/11/2020) |
| **[Dependencias]** | Es hijo y por tanto depende del proceso de negocio 001 Reducir la propagación del virus y el número de contagios en la pandemia actual o en futuras pandemias. Depende del proceso de negocio a implementar 004 Suministrar información y estadísticas al gobierno. |
| **Descripción** | Con todos los datos reunidos realizaremos un estudio y un tratamiento de los mismos. La finalidad última de este porceso es el suministro de los datos recabados y la información extraida de los mismos al ministerio para que pueda interpretar toda esta información y tomar las medidas y las decisiones que crea oportunas para controlar de la mejor manera la situación. |
| **Subobjetivos** |  |
| **[Importancia]** | Muy alta|
| **[Prioridad]** | Alta |
| **Comentarios** | Se necesita disponer de dicha información para poder tomar decisiones en base a los datos recopilados.|

<p align="center"> <b>Tabla 5.6: Objetivos de Negocio: Proporcionar información y datos al ministerio</b> <br> </p>
