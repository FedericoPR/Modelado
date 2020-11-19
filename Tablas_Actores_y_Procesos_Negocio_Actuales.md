## 3.2.1 Descripción de los Actores de Negocio Actuales

Los actores de negocio de nuestra aplicación o toda aquella persona interesada en está serán: ciudadanos, gobierno, autoridades y ambulatorios. Necesarios para que la información se transmita de manera segura.

| **\<id>1** | Ciudadano |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | El cuidadano es la piedra angular del proceso y por ello la mayoría de los procesos de negocio actuales dependen de el. El proceso 1, "Hacer prueba PCR", depende directamente del cuidadano ya que es objeto de dicha prueba. Por el mismo motivo también depende el proceso 2, "Registrar resultado de la prueba". El proceso 3, "Rastreo por contacto con un positivo", depende también de este actor ya que un resultado positivo en un cuidadano recae en la realización de pruebas en otros ciudadanos. Por último el proceso control de la cuarentena y seguimiento del estado del paciente, proceso 4, depende del cuidadano por razones obvias.|
| **Descripción** | Este actor de negocio actual es el actor principal en torno al que gira todo el sistema. Representa a cada uno de los ciudadanos. De este actor se obtiene la informacion de su localización por medio de la tecnología bluetooth de su móvil para que si se produce un positivo poder alertar a aquellas personas que hayan tenido contacto. La llamada de un ciudadano por padecer síntomas y la realización de una PCR es lo que dispara los diferentes procesos de negocio, ya que si se produce un positivo este debe guardar una cuarentena sobre la que se realiza un seguimiento además de iniciarse un rastreo de los posibles cuidadanos que también puedan haber sido contagiados. La información sobre los resultados de las pruebas y sobre el seguimiento del cuidadano positivo se pone en conocimiento de los rastreadores que llevan a cabo las acciones pertinentes|
| **Comentarios** | De la información obtenida por medio de los ciudadanos positivos, como la residencia, los puntos de visita frecuentes o las personas con las que ha mantenido contacto se sacan conclusiones por medio de su análisis que puedan dar lugar a toma de decisiones. |

<p align="center"> <b>Tabla 3.1: Actores de negocio.</b>

| **\<id>2** | Gobierno |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | De este actor depende el proceso de negocio 5, "Toma de decisiones", ya que es el encargado de tomar las medidas o imponer las restriccones en función del análisis de la información disponible. |
| **Descripción** | Este actor de negocio actual representa al gobierno, en concreto al ministro de sanidad, al que se le suministrarán todos los datos y estadísticas que se han obtenido por medio del procesamiento de los datos capturados de los ciudadanos y procesados. Dicho actor se encargará como entidad de tomar las decisiones oportunas en función de los datos suministrados por la plataforma, en base a diferentes criterios.
| **Comentarios** | Es un actor que se encuentra "aislado" del proceso de deteccion y seguimiento de positivos pero que será muy importante debido a su capacidad de toma de decisiones. Este actor puede imponer medidas nuevas, protocolos diferentes y alterar de manera importante todos los procesos tal y como se llevan a cabo hasta ahora. Es por ello que aunque se encuentre fuera del flujo normal es importantisimo incluirlo por su capacidad de cambiar el mismo. |

<p align="center"> <b>Tabla 3.2: Actores de negocio.</b> 


# 3.2.2 Descripción de Procesos de Negocio Actuales

Aquí se especificarán los procesos que debe llevar a cabo nuestra aplicación que llevarán un diagrama donde se detallarán los pasos a seguir. Según finalicen las entrevistas se 
irán añadiento y modificando los procesos. Inicialmente podemos pensar en estos como los procesos principales del programa.

| **\<id>3** | Rastreo por contacto con positivo |
| -- | -- |
| **[Versión]** | 1.0(19/11/2020) |
| **[Dependencias]** | Este porceso de negocio depende totalmente del proceso 2, "Registrar resultado de la prueba PCR", ya que unicamente entra en juego con un resultado positivo de la prueba realizada al ciudadano. |
| **Descripción** | A día de hoy en la llamada que se realiza con el usuario susceptible de ser positivo se le solicitan a este los nombres de todas aquellas personas con las que ha mantenido contacto directo a lo largo de las úlitmas horas, normalmente las 48 horas previas a la manifestación de síntomas. En  caso de confirmarse el positivo del usuario los sanitarios y/o las autoridades proceden a contactar con aquellos cuidadanos que el positivo suministró en un primer momento para poder realizarles las pruebas pertinentes a cada uno de ellos y volver a comenzar con el proceso|
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Actores]** | * Ambulatorio <br> * Cuidadano <br> * Autoridades |
| **Comentarios** | Actualmente tenemos que confiar en que el usuario nos proporcione todos los contactos que ha tenido en las horas previas. En este sentido tenemos el handicap de que el usuario puede no recordarlos todos y/o no querer proporcionarlos todos por conveniencia|

<p align="center"> <b>Tabla 4.3: Procesos de Negocio actuales.</b> <br> <i>Los atributos entre corchetes son opcionales</i> </p>


| **\<id>4** | Llevar seguimiento del paciente y control de su cuarentena |
| -- | -- |
| **[Versión]** | 1.1(19/11/2020) |
| **[Dependencias]** | Este porceso de negocio depende totalmente del proceso 2, "Registrar resultado de la prueba PCR", ya que unicamente entra en juego con un resultado positivo de la prueba realizada al ciudadano. |
| **Descripción** | Actualmente una vez se detecta un positivo, este queda automaticamente puesto en cuarentena de 10 a 15 días dependiendo del caso. Para poder llevar a cabo un seguimiento de esta cuarentena los sanitarios y/o las autoridades realizan llamadas con frecuencia al paciente. Con esta llamada se pretede controlar que el usuario está cumpliendo las restricciones impuestas así como llevar a cabo un seguimiento sobre su estado de salud|
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Actores]** | * Ambulatorio <br> * Cuidadano <br> * Autoridades |
| **Comentarios** | Este proceso de negocio finalizaría una vez termine esta cuarentena, dando por hecho que, pasado el tiempo estimado, el paciente estará sano y no puede contagiar|

<p align="center"> <b>Tabla 4.4: Procesos de Negocio actuales.</b> <br> <i>Los atributos entre corchetes son opcionales</i> </p>
