## 4. NECESIDADES DE NEGOCIO

Una vez que ya somos conscientes de cual es el dominio del problema y tenemos una visión mucho más clara y concisa de cuál es la situación actual debemos establecer aquellos puntos que vamos a necesitar cumplir para llegar a unos objetivos marcados y tangibles. 

Tenemos que tener claro en todo momento que el objetivo principal de nuestro sistema va a ser la reducción de la propagación del virus y por consiguiente la disminucion del numero de contagios. Para poder cumplir con el ojetivo principal, centraremos nuestros esfuerzos en la detección de positivos en torno a un positivo confirmado y en la confirmación del cumplimiento de la cuartentena de los contagiados.

Para poder llevar un control preciso sobre el avance y el cumplimiento de los objetivos establecidos con el cliente acotaremos estos objetivos como necesidades de negocio que podremos medir.

_Esta sección obligatoria debe contener información sobre los objetivos de negocio de clientes y usuarios, incluyendo los modelos de procesos de negocio a implantar. Esta sección se divide en las secciones que se describen a continuación.
La información de esta sección puede que ya se encuentre total o parcialmente en documentación previa como el Pliego de Prescripciones Técnicas, la Oferta seleccionada o el Estudio de Viabilidad del Sistema, en cuyo se podrá reutilizar y se hará referencia a dichos documentos como fuente de la misma._

### 4.1 Objetivos de Negocio

Una vez nuestro sistema sea funcional y esté en producción deberá llevar a cabo ciertos requerimientos para los cuales ha sido concevido. De esta manera queremos dejar plasmados los siguientes objetivos de negocio para poder demostrar en qué medida el sistema realiza su fución.

_Esta sección debe contener los objetivos de negocio que se esperan alcanzar cuando el sistema software a desarrollar esté en producción, especificados mediante las plantillas de objetivos de negocio que se muestran a continuación. En el caso de que se considere necesario, los objetivos de negocio se pueden descomponer jerárquicamente para facilitar su comprensión y representar dicha jerarquía de forma gráfica._

| **\<id>001** | Rastreo del contacto con un positivo |
| -- | -- |
| **[Versión]** | 1.0 (29/11/2020) |
| **[Dependencias]** | * \<procesos de negocio actuales o a implantar de los que depende> <br> * \<objetivo de negocio padre, si lo tiene>(padre) <br> * \<otros objetivos de negocio de los que depende> <br> * ... |
| **Descripción** | Una vez tenemos un positivo en la prueba realizada al usuario procederemos al rastreo por medio de los datos de las operadoras de todos aquellos usuarios susceptibles de estar contagiados. El objetivo ideal sería ser capaces de obtener el 100% de las personas que hayan mantenido un contacto suficiente con la persona que ha dado positivo para poder realizarles las pruebas. Como es prácticamente imposible llegar al 100% de personas que han contactado con el positivo por motivos que escapan a nuestro control ausencia de dispotivo movil en el momento del contacto, fallos o imprecisiones en el posicionamiento GPS... consideraremos aceptable poder identificar y contactar con todos aquellos que el sistema nos marque como objetivos y lo estimaremos en un 80% de los casos reales, por los inconvenientes citados anteriormente.|
| **Subobjetivos** | * <objetivos de negocio hijos(subobjetivos), si los tiene> <br> * ... |
| **[Importancia]** | \<importancia del objetivo de negocio para el cliente> |
| **[Prioridad]** | \<prioridad del objetivo de negocio para la dirección del proyecto> |
| **Comentarios** | \<comentarios adicionales> |

<p align="center"> <b>Tabla 5: Objetivos de Negocio: Rastreo del contacto con un positivo</b> <br> </p>

| **\<id>002** | Asegurar la realización de las pruebas |
| -- | -- |
| **[Versión]** | 1.0 (29/11/2020) |
| **[Dependencias]** | * \<procesos de negocio actuales o a implantar de los que depende> <br> * \<objetivo de negocio padre, si lo tiene>(padre) <br> * \<otros objetivos de negocio de los que depende> <br> * ... |
| **Descripción** | Una vez hemos contactado con todas aquellas personas que han mantenido el suficiente contacto con un positivo como para ser consideradas como posibles contagiadas tendremos que asegurarnos de que estas se realizan las pruebas pertinentes para confirmar o no si han sido contagiadas. Para ello pondremos a disposición de los ambulatorios y de las autoridades competentes los datos del usuario para que puedan informarlo y realizarle las pruebas con la mayor rapidez posible. El objetivo ideal sería que el 100% de los contactos susceptibles de ser positivos pudieran ser localizados y se les ralizaran las pruebas; sin embargo habrá situaciones que se escapen a nuestro control e incluso a de las autoridades, como por ejemplo la falta de información del usuario por parte de la operadora, la posibilidad de tener unos datos desactualizados del usuario...Por ello consideraremos aceptable llegar a realizar las pruebas al 90% de los usuarios que pueden haber sido contagiados por un caso confirmado.|
| **Subobjetivos** | * <objetivos de negocio hijos(subobjetivos), si los tiene> <br> * ... |
| **[Importancia]** | \<importancia del objetivo de negocio para el cliente> |
| **[Prioridad]** | \<prioridad del objetivo de negocio para la dirección del proyecto> |
| **Comentarios** | \<comentarios adicionales sobre el actor de negocio actual> |

<p align="center"> <b>Tabla 5: Objetivos de Negocio: Asegurar la realización de las pruebas</b> <br> </p>

| **\<id>003** | Identificar posibles focos de contagio |
| -- | -- |
| **[Versión]** | 1.0 (29/11/2020) |
| **[Dependencias]** | * \<procesos de negocio actuales o a implantar de los que depende> <br> * \<objetivo de negocio padre, si lo tiene>(padre) <br> * \<otros objetivos de negocio de los que depende> <br> * ... |
| **Descripción** | Combinando los datos de los usuarios que tenemos con los resultados de las prebas realizadas podemos establecer aquellas zonas y lugares donde se producen más contagios. Una vez obtenemos una prueba positiva realizamos el rastreo de aquellos usuarios que pueden haber sido contagiados por haber estado en contacto directo en un mismo lugar durante un tiempo determinado con el positivo. Si los usuarios localizados también dan positivo en la prueba que se les realice podremos establecer dónde se ha producivo el contagio. Con todos los datos reunidos de esta manera podemos establecer las "zonas calientes" donde se han producido más contagios para poder poner en alerta a los organismos competentes o a los usuarios de estas localizaciones. Como no podemos asegurar que el contagio se produjo al 100% en un lugar, ya que puedes contagiarte por contacto con un asintomático estableceremos como punto aceptable la determinación de los focos de contagio con un nivel de fiabilidad del 90%|
| **Subobjetivos** | * <objetivos de negocio hijos(subobjetivos), si los tiene> <br> * ... |
| **[Importancia]** | \<importancia del objetivo de negocio para el cliente> |
| **[Prioridad]** | \<prioridad del objetivo de negocio para la dirección del proyecto> |
| **Comentarios** | \<comentarios adicionales sobre el actor de negocio actual> |

<p align="center"> <b>Tabla 5: Objetivos de Negocio: Identificar posibles focos de contagio</b> <br> </p>

| **\<id>004** | Asegurar el cumplimiento de la cuarentena |
| -- | -- |
| **[Versión]** | 1.0 (29/11/2020) |
| **[Dependencias]** | * \<procesos de negocio actuales o a implantar de los que depende> <br> * \<objetivo de negocio padre, si lo tiene>(padre) <br> * \<otros objetivos de negocio de los que depende> <br> * ... |
| **Descripción** | Una vez tenemos un resultado postitivo de las pruebas pondremos a disposición de los cuerpos de seguridad del estado y de los ambulatorios los datos del usuario para poder informar al usuario de su situación de cuarentena desde ese mismo momento y para poder llevar a cabo un control exahustivo de la misma.  |
| **Subobjetivos** | * <objetivos de negocio hijos(subobjetivos), si los tiene> <br> * ... |
| **[Importancia]** | \<importancia del objetivo de negocio para el cliente> |
| **[Prioridad]** | \<prioridad del objetivo de negocio para la dirección del proyecto> |
| **Comentarios** | \<comentarios adicionales sobre el actor de negocio actual> |

<p align="center"> <b>Tabla 5: Objetivos de Negocio: Asegurar el cumplimiento de la cuarentena</b> <br> </p>

| **\<id>005** | Proporcionar información y datos al ministerio |
| -- | -- |
| **[Versión]** | 1.0 (29/11/2020) |
| **[Dependencias]** | * \<procesos de negocio actuales o a implantar de los que depende> <br> * \<objetivo de negocio padre, si lo tiene>(padre) <br> * \<otros objetivos de negocio de los que depende> <br> * ... |
| **Descripción** | Con todos los datos reunidos realizaremos un estudio y un tratamiento de los mismos. La finalidad última de este porceso es el suministro de los datos recabados y la infomración extraida de los mismos al ministerio para que pueda interpretar toda esta información y tomar las medidas y las decisiones que crea oportunas para controlar de la mejor manera la situación |
| **Subobjetivos** | * <objetivos de negocio hijos(subobjetivos), si los tiene> <br> * ... |
| **[Importancia]** | \<importancia del objetivo de negocio para el cliente> |
| **[Prioridad]** | \<prioridad del objetivo de negocio para la dirección del proyecto> |
| **Comentarios** | \<comentarios adicionales sobre el actor de negocio actual> |

<p align="center"> <b>Tabla 5: Objetivos de Negocio: Proporcionar información y datos al ministerio</b> <br> </p>
