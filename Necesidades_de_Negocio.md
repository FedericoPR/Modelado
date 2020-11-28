## 4. NECESIDADES DE NEGOCIO
Esta sección obligatoria debe contener información sobre los objetivos de negocio de clientes y usuarios, incluyendo los modelos de procesos de negocio a implantar. Esta sección se divide en las secciones que se describen a continuación.
La información de esta sección puede que ya se encuentre total o parcialmente en documentación previa como el Pliego de Prescripciones Técnicas, la Oferta seleccionada o el Estudio de Viabilidad del Sistema, en cuyo se podrá reutilizar y se hará referencia a dichos documentos como fuente de la misma.

### 4.1 Objetivos de Negocio
Esta sección debe contener los objetivos de negocio que se esperan alcanzar cuando el sistema software a desarrollar esté en producción, especificados mediante las plantillas de objetivos de negocio que se muestran a continuación. En el caso de que se considere necesario, los objetivos de negocio se pueden descomponer jerárquicamente para facilitar su comprensión y representar dicha jerarquía de forma gráfica.

| **\<id>999** | \<nombre descriptivo> |
| -- | -- |
| **[Versión]** | <nº versión>(<fecha versión>) |
| **[Dependencias]** | * \<procesos de negocio actuales o a implantar de los que depende> <br> * \<objetivo de negocio padre, si lo tiene>(padre) <br> * \<otros objetivos de negocio de los que depende> <br> * ... |
| **Descripción** | <descripción del objetivo de negocio en términos del problema> |
| **Subobjetivos** | * <objetivos de negocio hijos(subobjetivos), si los tiene> <br> * ... |
| **[Importancia]** | \<importancia del objetivo de negocio para el cliente> |
| **[Prioridad]** | \<prioridad del objetivo de negocio para la dirección del proyecto> |
| **Comentarios** | \<comentarios adicionales sobre el actor de negocio actual> |

<p align="center"> <b>Tabla 5: Objetivos de Negocio.</b> <br> </p>

### 4.2 Modelos de Procesos de Negocio a Implantar
Esta sección debe contener los modelos de procesos de negocio a implantar, que normalmente son los modelos de procesos de negocio actuales con ciertas mejoras. Si las diferencias con los modelos de procesos actuales son pequeñas, se puede optar por describir únicamente dichas diferencias siempre que se hayan incluido los modelos de procesos actuales en la sección 3.2.
Esta sección podrá omitirse si se han incluido los modelos de procesos de negocio actuales en la sección 3.2 y no se van a introducir cambios significativos en dichos modelos. En cualquier otra situación, esta sección debe considerarse como obligatoria, ya que los modelos de procesos de negocio son la base para un buen desarrollo de sistemas de información, especialmente si se quieren aplicar arquitecturas orientadas a servicios.

#### 4.2.1 Descripción de los Actores de Negocio a Implantar
Esta sección debe contener información sobre los actores de negocio (organizaciones, roles o responsabilidades) de los modelos de procesos de negocio a implantar, especificados mediante las plantillas para actores del negocio a implantar que se muestran a continuación.

| **\<id>999** | \<nombre descriptivo> |
| -- | -- |
| **[Versión]** | <nº versión>(<fecha versión>) |
| **[Dependencias]** | * \<actores de negocio actual relacionados> <br> * ... |
| **Descripción** | Este actor de negocio actual representa a <descripción de la organización, rol o responsabilidad a la que representa el actor de negocio actual> |
| **Comentarios** | \<comentarios adicionales sobre el actor de negocio a implantar> |

<p align="center"> <b>Tabla 6: Actores de negocio a implantar.</b> <br> </p>

#### 4.2.2 Descripción de Procesos de Negocio a Implantar
Esta sección debe contener información sobre los procesos de negocio a implantar, tal y como se espera que se realicen en la organización del cliente una vez que el sistema software a desarrollar esté en producción. Para cada proceso de negocio se incluirá una descripción textual usando las plantillas para procesos de negocio a implantar que se muestran a continuación, y un diagrama en la notación que se considere oportuna, por ejemplo diagramas BPMN (Business Process Model and Notation) o diagramas de actividad UML (Unified Modeling Language).

| **\<id>999** | \<nombre descriptivo> |
| -- | -- |
| **[Versión]** | <nº versión>(<fecha versión>) |
| **[Dependencias]** | * \<procesos de negocio actuales que modifica o sustituye> <br> * ... |
| **Descripción** | <descripción del proceso de negocio a implantar en términos del dominio del problema> |
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Actores]** | * \<actor que participa en el proceso de negocio> <br> * ... |
| **Comentarios** | \<comentarios adicionales sobre el proceso de negocio a implantar> |

<p align="center"> <b>Tabla 7: Procesos de Negocio a implantar.</b> <br> </p>
