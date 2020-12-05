#### 6.2.3 Especificación de Casos de Uso del Sistema

| **\<id> CU 0.1** | Listar ciudadanos por estado |
| -- | -- |
| **[Versión]** | 1.0 (04/12/2020) |
| **[Dependencias]** | Este caso de uso depende del CU 1.1 (Registrar ciudadano en el sistema) ya que necesita que recopilar la información de los ciudadanos ya registrados en el sistema que filtrará según su estado. Este caso de uso interactua con los actores ambulatorio y fuerzas del orden dado que estos podrán acceder a las listas creadas por el sistema. |
| **Precondición** | El sistema debe tener ciudadanos ya registrados con sus respectivos datos |
| **Descripción** | El sistema deberá recopilar la información de los ciudadanos en forma de listas que iran filtradas por el estado de los ciudadanos. Es de vital importancia pues será la base para gestionar los procesos y decisiones que deberán tomar los actores relacionados con la salida de este caso de uso ya que el conocimiento del estado de los ciudadanos nos dará perspectiva a la hora de tomar acción. |
| **Postcondición** | Se habran creado una lista de todos los ciudadanos registrados según su estado, esta información será accesible tanto para los ambulatorios como para las fuerzas del orden. |
| **[Importancia]** | Muy alta |
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | Debemos tener siempre encuenta la enorme catidad de datos que maneja este caso de uso como explicamos en las debilidades. Ya que una mala gestión del flujo de datos afectaría a la efectividad y no tendriamos en estas listas un fiel reflejo de la situación actual lo que derivaría en no poder tomar la decisión óptima. |

<p align="center"> <b>Tabla 11.1: Plantilla simplificada de Casos de Uso.</b> <br> </p>

| **\<id> CU 0.2** | Informar al ciudadano |
| -- | -- |
| **[Versión]** | 1.0 (04/12/2020) |
| **[Dependencias]** | Este caso de uso depende del CU 1.2 (Registrar resultado de la prueba en el sistema) ya que si el ciudadano da positivo, el sistema notificará este para que sepa que pasos debe realizar, si se debe realizar alguna otra prueba o  iniciar el CU 2.1 o bien el CU 2.2 para llevar acabo el control del cumplimiento del periodo de cuarentena. |
| **Precondición** | El ciudadano tiene que estar registrado en el sistema ya que se debe obtener su numero de télefono para así contactar con la mayor rapidez posible.|
| **Descripción** | El sistema debera notificar al ciudadano de que precauciones debe tomar y que pasos a seguir si debe cumplir el periodo de cuarentena o realizar alguna prueba médica. Cuanta más completa sea la información mejor reaccionará el ciudadano y será menos propenso a cometer cualquier error que pueda poner en riesgo a sí mismo y a los que le rodean.|
| **Postcondición** | El ciudadano tendrá instrucciones claras de como debe proceder en caso de tener que realizarse una prueba médica o de cumplir el periodo de cuarentena establecido. |
| **[Importancia]** | Muy alta |
| **[Prioridad]** | alta |
| **[Estado]** | Pendiente |
| **Comentarios** | Aunque no necesitemos de la intervención del ciudadano en el sistema es muy importante que esté bien informado dado que todo gira en torno a su bienestar y salud. |

<p align="center"> <b>Tabla 11.2: Plantilla simplificada de Casos de Uso.</b> <br> </p>

| **\<id> CU 1.1** | Registrar ciudadano en el sistema |
| -- | -- |
| **[Versión]** | 1.0 (04/12/2020) |
| **[Dependencias]** | Este caso de uso depende del CU 1.6 (Registrar cita pruebas en el sistema) ya que un ciudadano sospechoso de tener el virus debe realizarse una prueba por lo que se debe guardar información sobre él en caso de que diera un resultado positivo. Lo que iniciaria el CU 0.1 (Listar ciudadanos por estado) con los datos que proporciona este caso de uso con la información del ciudadano y estado. En este caso de uso interactutuará con el actor ambulatorio que tendrá permiso para introducir la información necesaria del ciudadano al sistema. |
| **Precondición** | El usuario debe presentar sintomas de la enfermedad para así considerarlo caso sospechoso y empezar el seguimiento de su situación. |
| **Descripción** | Este caso de uso supone el inicio del proceso de seguimiento de un ciudadano del cual se sospecha que tenga la enfermedad, para tener disponibe su información y poder contactar rapidaente con dicho ciudadano en caso de dar positivo, asi como poder almacenarlo en nuestros listados de ciudadanos por estado. La información del ciudadano tras su resgistro se considerá vital para el funcionamiento del sistema en cuanto a generar estadisticas estadisticas y dar su acceso a aquellosactores autorizados ..  |
| **Postcondición** | Habrá un nuevo ciudadano registrado en el sistema con sus correspondientes datos. |
| **[Importancia]** | Muy Alta> |
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | La información del ciudadano registrado es únicamente accesible a los actores autorizados de cara a proteger su privacidad y que agentes externos no se puedan aprovechar de dichos datos |

<p align="center"> <b>Tabla 11.3: Plantilla simplificada de Casos de Uso.</b> <br> </p>

| **\<id> CU 1.2** | Registrar resultado de la prueba en el sistema |  |
| --- | --- | --- |
| **[Versión]** | 1.0 (05/12/2020) |
| **[Dependencias]** | Este caso de uso depende del CU 1.3 (Rastrear contactos directos con el postivo) que será necesario para poder llevar a cabo el CU 1.6 (Registrar cita pruebas en el sistema), de dichas citas se realizarán las pruebas pertinentes al ciudadano.  Este caso de uso  será el inicio del CU  3.1 (Registrar cita pruebas en el sistema) en caso de que las pruebas den positivo. Así como del CU 0.2 (Informar al ciudadano) notificandole a este el resultado de la prueba.|
| **Precondición** | La prueba ha sido realizada al ciudadano en la cita acordada. |
| **Descripción** | El sistema deberá almacenar los resultados de las pruebas realizadas a los ciudadanos, lo que ejecutará los procesos necesarios para saber si debemos iniciar un seguimiento del paciente en caso de tener la enfermedad. Basicamente informa a los distintos procesos de nuestro sistema el estado del ciudadano de cara  |
| **Secuencia Normal** | **Paso** | **Acción** |
|  | 1 |  El responsable del ambulatorio solicitará los resultados del ciudadano al que se le ha realizado la prueba  |
|  | 2 | El sistema devuelve los resultados de dicha prueba. |
|  | 3 | Si el resultado es positivo en coronavirus |
|  | 4 | Se inicia el CU 1.1 (Registrar ciudadano en el sistema) |
|  | 5 | Se inicia el CU 0.2 (Informar al ciudadano) |
|  | 6 | {El caso de uso termina con éxito} |
| **Postcondición** | El resultado de la prueba realizada se almacenará en el sistema. |
| **Excepciones** | **Paso** | **Acción** |
|  | 1 | Si el resultado de la prueba es negativo |
|  | 2 | El ambulatorio registrara al ciudadano como caso no positivo en las listas de estado del sistema.  |
|  | 3 | Se inicia el CU 0.2 (Informar al ciudadano) pero en este caso se le dira que no tiene coronavirus y que no debe cumplir la cuarentena. |
|  | 4 | El caso de uso termina |
| **Rendimiento** | **Paso** | **Cota de tiempo** |
| | q | k\<unidad de tiempo> no se| 
| **Frecuencia** | \<nº veces / unidad de tiempo> no se|
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** |  |
<p align="center"> <b>Tabla 12: Plantilla Completa de Casos de Uso.</b> <br> </p>


