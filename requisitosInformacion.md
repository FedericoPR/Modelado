| **RF 01** | Datos de los ciudadanos |
| -- | -- |
| **[Versión]** | 1.0 (10/12/2020) |
| **[Dependencias]** | El requisito depende del CU 1.1 Registrar ciudadano en el sistema y del CU 1.5 Registrar contactos directos en el sistema.|
| **Descripción** | El sistema deberá almacenar los datos relativos a los  ciudadanos registrados en el sistema. En concreto: |
| **Datos especificos** | El nombre del ciudadano, el DNI, la dirección, el número de teléfono móvil, si dispone de teléfono móvil o no y en caso de tenerlo si dispone de sensor de huella dactilar. |
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | Los datos relativos a los ciudadanos son introducidos en el sistema una vez que se le registra al ciudadano por parte de los ambulatorios cuando se realizan las pruebas médicas o cuando se le considera un posible contacto directo con un positivo (almacenando parte de la información que será completada cuando se le realicen las pruebas médicas.) |

<p align="center"> <b>Tabla 13.1: Requisitos de Información.</b> <br> </p>

| **RF 02** | Resultado de las pruebas médicas |
| -- | -- |
| **[Versión]** | 1.0 (10/12/2020) |
| **[Dependencias]** | El requisito depende del CU 1.2 Registrar resultado de la prueba en el sistema. También depende del requisito general gestión de la realización de las pruebas médicas.|
| **Descripción** | El sistema deberá almacenar los datos relativos al resultado de las pruebas realizadas a los ciudadanos. En concreto:|
| **Datos especificos** | La fecha de realización de la prueba médica, el ciudadano al que se le ha realizado, el resultado de dicha prueba y si es necesario que el ciudadano realice cuarentena la fecha de fin de esta.|
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | Los datos relativos a las pruebas médicas serán introducidos en el sistema por parte del responsable médico de los ambulatorios una vez se conozca el resultado de la prueba médica realizada al ciudadano. |


<p align="center"> <b>Tabla 13.2: Requisitos de Información.</b> <br> </p>

| **RF 03** | Citas médicas |
| -- | -- |
| **[Versión]** | 1.0 (10/12/2020) |
| **[Dependencias]** | El requisito depende del CU 1.6 Registrar cita pruebas en el sistema y del CU 1.7 Enviar alerta a las autoridades de incumplmiento de realizarse la prueba.También depende del requisito general gestión de la realización de las pruebas médicas.|
| **Descripción** | El sistema deberá almacenar los datos relativos a las citas para realizar las pruebas médicas a los ciudadanos. En concreto:|
| **Datos especificos** | La hora de la cita, el día de la cita y el ambulatorio en el que se le realizará la prueba médica.|
| **[Importancia]** | Media |
| **[Prioridad]** | Media |
| **[Estado]** | Pendiente |
| **Comentarios** | Los datos relativos a las citas serán introducidos en el sistema por parte del responsable médico de los ambulatorios una vez se realice una llamada telefónica con el ciudadano para concretar la cita. Dichas citas se tendrán en cuenta dado que se realizarán comprobaciones periodicamente de que los ciudadanos han acudido a realizarse las pruebas médicas el día citado y en caso de no acudir, se enviará una alerta a las autoridades. |


<p align="center"> <b>Tabla 13.3: Requisitos de Información.</b> <br> </p>

| **RF 04** | Datos de localización de los ciudadanos. |
| -- | -- |
| **[Versión]** | 1.0 (10/12/2020) |
| **[Dependencias]** | El requisito depende del CU 1.3 Rastrear contactos directos con el postivo y del CU 1.4 Adquirir datos de los ciudadanos.También depende del requisito general rastrear los contactos entre casos positivos.|
| **Descripción** | El sistema deberá almacenar los datos relativos a la localización de los ciudadanos.En concreto:|
| **Datos especificos** | El ciudadano, el lugar en el que ha estado, el tiempo que ha estado en ese lugar y la fecha en la que estuvo en ese lugar.|
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | Los datos relativos a la localización de los ciudadanos serán proporcionados por las operadoras telefónicas de los ciudadanos, y tendrán una estrcutura clara fijada por dichas operadoras. Estos datos de localización de los ciudadanos serán actualizados periodicamente por las operadoras con el fin de que los rastreos de los contactos directos con los positivos que se realizan con dichos datos sean lo mas reales posibles. (La forma de manejar estos datos es responsabilidad del algoritmo de rastreo de contactos positivos.) |


<p align="center"> <b>Tabla 13.4: Requisitos de Información.</b> <br> </p>

| **RF 05** | Estado médico de los ciudadanos. |
| -- | -- |
| **[Versión]** | 1.0 (10/12/2020) |
| **[Dependencias]** | El requisito depende del CU 0.1 Listar ciudadanos por estado.|
| **Descripción** | El sistema deberá almacenar la información relevante al estado medico los ciudadanos registrados en el sistema. En concreto:|
| **Datos especificos** | El estado médico del ciudadano, que puede ser: contacto directo, a la espera de prueba, a la espera de resultado, en cuarentena (positivo), finaliza cuarentena.|
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | Los datos relativos al estado médico de los ciudadanos registrados en el sistema irá siendo actualizado en función de los eventos que ocurran en el sistema y dicha información será utilizada para poder listar aquellos ciudadanos que tengan un estado concreto con el fin de tomar distintas acciones en función de dicho estado. |


<p align="center"> <b>Tabla 13.5: Requisitos de Información.</b> <br> </p>

| **RF 06** | Localización del móvil de los ciudadanos. |
| -- | -- |
| **[Versión]** | 1.0 (10/12/2020) |
| **[Dependencias]** | El requisito depende del CU 2.1 Control automático por el sistema del cumplimiento cuarentena.(Ciudadanos con móvil) y del CU 2.3 Enviar alerta autoridades incumplimiento cuarentena.También depende del requisito general gestionar el cumplimiento de la cuarentena.|
| **Descripción** |El sistema deberá almacenar un registro actualizable sobre si los ciudadanos están cumpliendo la curentena.En concreto: (Localización del móvil cada 10 mins).|
| **Datos especificos** | La localización del móvil de aquellos ciudadanos que deben cumplir cuarentena (coordenadas) así como el ciudadano.|
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | Los datos relativos a la localización del móvil del ciudadano serán proporcionados al sistema por las operadores telefónicas de los ciudadanos, y serán almacenados en el sistema como un registro de coordenadas de la localización del móvil, de esta forma el sistema podrá controlar que el ciudadano está cumpliendo la cuarentena.|

<p align="center"> <b>Tabla 13.6: Requisitos de Información.</b> <br> </p>

| **RF 07* | Informe de las estadísticas generadas |
| -- | -- |
| **[Versión]** | 1.0 (10/12/2020) |
| **[Dependencias]** | El requisito depende del CU 3.2 Generar estadísticas y del CU 3.3 Informar estadísticas.También depende del requisito general gestionar la información recopilada y proporcionar estadísticas al gobierno.|
| **Descripción** |El sistema debrá almacenar informes sobre las estadísticas generadas. En concreto:|
| **Datos especificos** | Los informes generados por el sistema, que contendrán datos en un formato legible acompañados de distintos gráficos representativos de dichas estadísticas, además de la fecha en la que se ha generado el informe.|
| **[Importancia]** | Alta |
| **[Prioridad]** | Alta |
| **[Estado]** | Pendiente |
| **Comentarios** | Los datos relativos a los informes son generados de forma automática por el propio sistema y se deberá mantener un histórico de dichos informes, para que el gobierno pueda acceder a dicha información en cualquier momento.|

<p align="center"> <b>Tabla 13.7: Requisitos de Información.</b> <br> </p>

A continucación se mostrará un modelo gráfico que facilite la comprensión de los requisitos de información que debe de cumplir el sistema a desarrollar, para ello se adjunta un diagrama de entidad relación.

![picture 1](images/709d19016093475e858288348c505f388f6212b090e58cdda6c8af6b730b98f7.png)  
