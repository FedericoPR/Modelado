# 3.2.2 Descripción de Procesos de Negocio Actuales

Aquí se especificarán los procesos que debe llevar a cabo nuestra aplicación que llevarán un diagrama donde se detallarán los pasos a seguir. Según finalicen las entrevistas se 
irán añadiento y modificando los procesos. Inicialmente podemos pensar en estos como los procesos principales del programa.

| **\<id>3** | Rastreo por contacto con positivo |
| -- | -- |
| **[Versión]** | 1.0(19/11/2020) |
| **[Dependencias]** | Este porceso de negocio depende totalmente del proceso 2, "Registrar resultado de la prueba PCR", ya que unicamente entra en juego con un resultado positivo de la prueba realizada al ciudadano. |
| **Descripción** | A día de hoy en la llamada que se realiza con el usuario susceptible de ser positivo se le solicitan a este los nombres de todas aquellas personas con las que ha mantenido contacto directo a lo largo de las úlitmas horas, normalmente las 48 horas previas a la manifestación de síntomas. En  caso de confirmarse el positivo del usuario se procede a contactar con aquellos que el positivo suministró en un primer momento para poder realizar las pruebas pertinentes a cada uno de ellos y volver a comenzar con el proceso|
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Actores]** | * Ambulatorio <br> * Cuidadano |
| **Comentarios** | Actualmente tenemos que confiar en que el usuario nos proporcione todos los contactos que ha tenido en las horas previas. En este sentido tenemos el handicap de que el usuario puede no recordarlos todos y/o no querer proporcionarlos todos por conveniencia|

<p align="center"> <b>Tabla 4.3: Procesos de Negocio actuales.</b> <br> <i>Los atributos entre corchetes son opcionales</i> </p>


| **\<id>4** | Llevar seguimiento del paciente y control de su cuarentena |
| -- | -- |
| **[Versión]** | 1.1(19/11/2020) |
| **[Dependencias]** | Este porceso de negocio depende totalmente del proceso 2, "Registrar resultado de la prueba PCR", ya que unicamente entra en juego con un resultado positivo de la prueba realizada al ciudadano. |
| **Descripción** | Actualmente una vez se detecta un positivo, este queda automaticamente puesto en cuarentena de 10 a 15 días dependiendo del caso. Para poder llevar a cabo un seguimiento de esta cuarentena las autoridades sanitarias realizan llamadas con frecuencia al paciente. Con esta llamada se pretede controlar que el usuario está cumpliendo las restricciones impuestas así como llevar a cabo un seguimiento sobre su estado de salud|
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Actores]** | * Ambulatorio <br> * Cuidadano |
| **Comentarios** | Este proceso de negocio finalizaría una vez termine esta cuarentena, dando por hecho que, pasado el tiempo estimado, el paciente estará sano y no puede contagiar|

<p align="center"> <b>Tabla 4.4: Procesos de Negocio actuales.</b> <br> <i>Los atributos entre corchetes son opcionales</i> </p>
