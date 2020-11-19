# 3 DESCRIPCIÓN DE LA SITUACIÓN ACTUAL


Desde que se declaró el estado de alarma como consecuencia de la actual pandemia que estamos viviendo, se han debido de tomar diversas medidas, las cuales han ido cambiando constantemente, debido a la cambiante situación que se plantea con la pandemia cada día. Para poder tomar estas medidas, el gobierno junto con el grupo de expertos indicado deben conocer grandes volúmenes de información acerca de la pandemia y contrastarla.

Entre las medidas tomadas cabe destacar el confinamiento domiciliario al cual hemos estado sometidos cerca de 3 meses. Una vez que la situación mejoró se ha permitido el salir a la calle pero con un límite en el número de personas que se podían juntar. Los locales comerciales, la hosteleria, las grandes superficies han debido de tomar distintas medidas respecto al aforo y a los protocolos que se debían respetar.

Actualmente, las medidas tomadas son distintas dependiendo de las comunidades autónomas (dependen de los datos de la pandemia en dichas comunidades), y además dichas medidas cambian constantemente; luego no podemos suponer que la situación de hoy en día sea igual a la que se va a presentar mañana.

Actualmente el Ministerio de Sanidad posee una aplicación para el control y seguimiento ciudadano en términos de la pandemia mundial que nos asola causada por el COVID-19; sin embargo esta aplicación no es del agrado del ministerio por diversas razones. Para poder llevar a cabo una mejor gestión, que la proporcionada por la aplicación actual, en caso de producirse una nueva pandemia, el ministerio quiere hecerse con nuestros servicios para la creación de una nueva aplicación que sí satisfaga sus necesidades ante una posible situación similar en el futuro. 

Hoy en día todo el mundo lleva su móvil en todo momento consigo, móviles conectados a la red y que funcionan por medio de aplicaciones . Nos aprovecharemos este entorno tecnológico ya que es ideal para el seguimiento ciudadano. Puesto que las fuerzas del orden así como el sector sanitario posee también de dispositivos conectados a la red podremos comunicarnos con ellos. De esta manera se podrá comprobar el cumplimiento de las cuarentenas y las obligaciones de los ciudadanos por parte de los cuerpos de seguridad del estado, así como recibir listas, los ambulatorios, con las personas que deberán hacerse las pruebas para poder poner en conocimiento de las fuerzas del orden cualquier incumplimiento.

En la actualidad en torno al 90% de la población española dispone de un teléfono móvil, luego esto tiene las ventajas comentadas anteriormente para poder hacer el seguimiento oportuno a los ciudadanos de cara a obtener datos válidos para gestionar la pandemia. Sin embargo, el otro tanto por ciento de la población que no dispone de teléfono movil se encuentra en una situación especial que se debe tener en cuenta de cara a conocer como se va a actuar en nuestra plataforma en estos casos. Dado que dicho porcentaje de la población es muy reducido y además se corresponde con la población de menor edad y la población de edades avanzadas el rastreo de los contactos directos de estas personas se puede rastrear de forma manual con los métodos actuales, dado que estos grupos de población no tienen muchos contactos sociales distintos. A la hora de controlar el cumplimiento de la cuarentena en este tipo de usuarios, se delegará la responsabilidad en las fuerzas del orden, las cuales deberán hacer los controles oportunos, lo cual es viable al ser un número reducido de personas. 

Dado que con nuestra plataforma, Pandemio, vamos a poder obtener distintos datos de los ciudadanos, se van a manejar grandes volúmnes de información acerca de estos, lo que conlleva que los algoritmos utilizados para obtener información de estos datos o para manejear estos datos sean complejos. Dichos datos debe ser información anonimizada, tan solo podrán acceder a los datos los usuarios autorizados para ello como los agentes de la autoridad o los ambulatorios. Hoy en día, se debe tener un especial cuidado a la hora de manejar datos relacionados con las personas, y se debe cumplir la ley de protección de datos.

Debido a que la situación actual ha llevado a que se transfieran las competencias a las autonomías y cada una tiene sus propios sistemas de información, para poder realizar una implementación correcta en todas las autonomías deberemos de establecer distintas interfaces de comunicación entre ellas para poder acceder a sus sistemas de información y así acceder a los datos de los pacientes de cada autonomía.

_(Esta sección debe contener información sobre la situación actual de la organización para la que se va a desarrollar el sistema software. En concreto, debe contener información sobre los pros y contras de la situación actual, sobre los modelos de proceso de negocio actuales y sobre el entorno tecnológico actual de la organización, incluyendo la arquitectura orientada a servicios actual si existiera. Se divide en las secciones que se describen a continuación.
La información de esta sección puede que ya se encuentre total o parcialmente en documentación previa como el Pliego de Prescripciones Técnicas, la Oferta seleccionada o el Estudio de Viabilidad del Sistema, en cuyo caso se podrá reutilizar y se hará referencia a dichos documentos como fuente de la misma.)_

## 3.1 Pros y Contras de la Situación Actual

La situación actual hace que para la implementación de la aplicación que se nos solicita se nos presentan varios puntos que podrían ser de ayuda pero también cuestiones que suponen un obstacúlo a la hora de cumplir con las necesidades del cliente. 

Puesto que tenemos una aplicación realizada y probada recientemente en el mismo ámbito y con propósitos similares podremos realizar comparaciones con ella y establecer un punto de partida sólido. Tendremos en cuenta aquellos aspectos que han funcionado y aquellos que no y sus razones para poder aprender de ella y mejorar.

_(Esta sección debe contener información sobre los aspectos positivos y negativos del negocio actual de la organización para la que se va a desarrollar el sistema software. Se divide en las secciones que se describen a continuación.)_

### 3.1.1 Fortalezas de la Situación Actual

Para poder enfrentarnos al problema con un punto de partida fuerte aprovecharemos que tenemos el backup de la aplicación __Radar Covid__ de la que podemos sacar numerosas conclusiones para usarlas en nuestro favor.

Puesto que la situación de la pandemia actual es una situación critica se nos proporcionarán ciertos privilegios y facilidades proporcionandonos legalidad para ciertos asuntos que ahora mismo suponen un problema.

De toda esta situación podemos resumir las siguientes fortalezas en cuanto a nuestra situación actual:


_(Esta sección debe contener información sobre las fortalezas o aspectos positivos de la situación actual, especificadas mediante las  plantillas para fortalezas que se muestran a continuación. Se deberá prestar especial atención a aquellos aspectos que se considere que deben mantenerse en el modelo de negocio a implantar, para que se tengan en cuenta en el sistema software a desarrollar. El objetivo es mantener aquellas buenas prácticas que se considere oportuno en el nuevo sistema a desarrollar.)_


| **<id>001** | Reciente pandemia del COVID-19 |
| -- | -- |
| **[Versión]** | 1.0 (17/11/2020) |
| **Descripción** | Dado que actualmente existe la pandemia del Covid-19, hemos adquirido la suficiente experiencia de como se debe actuar ante una pandemia y cuales deben ser las medidad a tomar. Es decir, tendremos un conocimiento previo y un conjunto de técnicas que se podrán aplicar de cara a controlar la pandemia y no actuaremos desde cero. |
| **Comentarios** | En la actualidad se conocen los protocolos de actuación ante una pandemia, la sociedad conoce el como actuar y dispone de una experiencia previa de ello. Además se dispone de datos previos y estudios acerca de la eficacia de las diferenetes mediadas tomadas en la actual pandemia. |
  
<p align="center"> <b>Tabla 1.1</b>
  
| **<id>002** | Referencia Aplicación "Radar Covid" |
| -- | -- |
| **[Versión]** | 1.0  (17/11/2020) |
| **Descripción** | En la actualidad existe otra aplicación del ministerio llamada Radar Covid, la cual la base de su funcionalidad es parecida a la de nuestra plataforma, la idea de controlar los contagios surge de esta aplicación y se tratará de mejorar las deficiencias encontradas en ella. A partir de esta aplicación se dispone de una base para comenzar a desarrollar nuestra plataforma. |
| **Comentarios** | Usaremos como fortaleza de esta aplicación la idea de controlar los contactos con los positivos, pero la implementación sufrirá modificaciones, ya que se usarán los datos proporcionados por las operadoras móviles, en vez de el uso de bluetooth por los problemas encontrados en su uso.  |
  
<p align="center"> <b>Tabla 1.2</b>
    
| **<id>003** | Existencia de datos sobre la población |
| -- | -- |
| **[Versión]** | 1.0  (18/11/2020) |
| **Descripción** | Debido a la actual pandemia del COVID-19 los distintos estamentos del gobierno y sus autonomías han podido recabar información sobre la población en vistas a poder prevenir la extension del virus. |
| **Comentarios** | Con cada llamada a los teléfonos habilitados para la población para temas de COVID-19 el protocolo marcaba imprescindible recabar datos sobre la persona que realizaba la llamada, tales como la edad o el código postal. De confirmarse el positivo, y con el objetivo de realizar el rastreo se le preguntaba al usuario las personas con las que había mantenido contacto en los días previos así como su dirección y los lugares donde había estado durante un periodo largo de tiempo. Toda esa información que ya tenemos podría ser usada en un futuro para realizar estudios que nos permitieran llevar a cabo una actuación más rápida y eficiente a la hora de encotrar infectados y adelantarnos en una posible nueva pandemia para minimizar la propagación|
  
<p align="center"> <b>Tabla 1.3</b>
  
| **<id>004** | Acceso a los datos de los operadores móviles |
| -- | -- |
| **[Versión]** | 1.0 (17/11/2020) |
| **Descripción** | Gracias a que la situación de pandemia ha llevado a que se declare un estado de alerta sanitaria se dispone de una situación en la cual se pueden hacer los cambios legales necesarios, entre ellos que los datos acerca de los ciudadanos sean proporcionados por las propias operadoras con el fin de usar esta información para nuestra plataforma y no con otros fines. Dichos datos son los mas precisos que se pueden obtener, y en ellos no tiene que intervenir el usuario, sino que son obtenidos sin su "consentimiento". |
| **Comentarios** | Tomaremos como fortaleza el hecho de que al obtener los datos de las operadoras móviles, el usuario no se puede negar a proporcionar dichos datos y además, se evitan los posibles despistes de tener desconectado el bluetooth como ocurría con Radar Covid o que al utilizarse otro dispositivo, no se registren los nuevos contactos directos.|
  
<p align="center"> <b>Tabla 1.4</b>
  
| **<id>005** | Posibilidad de realizar los cambios legales necesarios |
| -- | -- |
| **[Versión]** | 1.0 (17/11/2020) |
| **Descripción** | Dado que nuestro cliente es el Ministerio de Sanidad, se está planteando crear un estado de alerta sanitaria o pandemia con el fín de que dicho estado de alerta sirva como paraguas para poder realizar los cambios legales necesarios a la hora de poder implementar de una forma correcta nuestra plataforma y poder obtener los datos necesarios para ello.|
| **Comentarios** | Se tomará como fortaleza el hecho de que si existe algún impedimento legal a la hora de poder implementar nuestra plataforma, al estar destinada al gobierno se podrán realizar los cambios legales necesarios para eliminar dichos impedimentos o reducirles. |
  
<p align="center"> <b>Tabla 1.5</b>
  
| **<id>006** | Disponibilidad de móvil de gran parte de la población |
| -- | -- |
| **[Versión]** | 1.0 (17/11/2020) |
| **Descripción** | En la actualidad cerca del 90% de la población española dispone de teléfono móvil, luego esto es una gran fortaleza dado que podremos obtener información de una gran parte de la población gracias a sus dispositivos móviles. Además se podrá utilizar a su vez como dispositivo para controlar que se cumplen con las cuarentenas obligatorias así como medio de comunicación con el ciudadano. |
| **Comentarios** | El pequeño porcentaje de la población que no dispone de teléfono movil se suele corresponder con niños o personas de edad avanzada, las cuales es más fácil de rastrear sus contagios y si cumplen la cuarentena obligatoria, para ello hará falta de la actuación de los agentes de la autoridad o personas asignadas para ello. |
  
<p align="center"> <b>Tabla 1.6</b>
  
| **<id>007** | Comunicación con las fuerzas del orden y los sanitarios |
| -- | -- |
| **[Versión]** | 1.0 (18/11/2020) |
| **Descripción** | Para poder llevar a cabo un control eficiente de las personas que deben realizarse las pruebas enviaremos a los ambulatorios los listados de personas que deben hacerse las pruebas, y estos podrán notificar a la autoridad el inclumplimiento. Por su parte las fuerzas del orden podrán comprobar el cumplimiento de las cuarentenas y las obligaciones impuestas a los ciudadanos |
| **Comentarios** | Nuestra labor será la de recabar información que proporcionaremos a los ambulatorios y a sanidad para que puedan llevar a cabo las acciones pertinentes, pero el hecho de que estemos en comunicacion directa con organismos con tanto "poder" debería influir positivamente en el éxito de nuestro proyecto |
    
<p align="center"> <b>Tabla 1.7</b>
  

### 3.1.2 Debilidades de la Situación Actual

Debido a la complejidad de la situación actual y a que la aplicación __Radar Covid__ ha ofrecido muchos puntos en contra pero pocos a favor nos encontramos en una posición donde todo aquello que queramos implementar puede ser muy buena idea sobre el papel pero causar muchas dificultades en un contezto real.

Por otro lado para poder llevar a cabo ciertas operaciones vamos a necesitar del uso de los datos de localización de los móviles y eso, por el momento supone un problema. Aún así, cuando esto esté solucionado deberemos lidiar con el cumplimiento de la ley de protección de datos.

De toda esta situación podemos resumir las siguientes debilidades en cuanto a nuestra situación actual:

_(Esta sección debe contener información sobre las debilidades o aspectos negativos de la situación actual, especificadas mediante las plantillas para debilidades que se muestran a continuación. Se deberá prestar especial atención a aquellos aspectos que se considere que no deben repetirse en el modelo de negocio a implantar, para que se eviten en el sistema software a desarrollar. El objetivo es no volver a reproducir los problemas del sistema actual en el sistema a desarrollar.)_

| **<id>001** | Problemas en el uso de Bluetooth |
| -- | -- |
| **[Versión]** | 1.0 (18/11/2020) |
| **Descripción** | La aplicación Radar Covid intentó realizar la localización de los usuarios y sus interacciones por medio del bluetooth sin embargo reultó ser inservible si este estaba apagado o siendo usado por otro accesorio.|
| **Comentarios** | Supone una debilidad el hecho de que la "primera opción" para localizar a los usuarios haya fracasado y por tanto tendremos que buscar otra opción mejor.| 
  
<p align="center"> <b>Tabla 2.1</b>
  
| **<id>002** | Opcionalidad de los usuarios para estar controlados|
| -- | -- |
| **[Versión]** | 1.0 (18/11/2020) |
| **Descripción** | La obtención de Radar Covid por parte del usuario era totalmente voluntaria, lo que supone un gran problema ya que el usuario que lo deseara podría ser "invisible" desde el punto de vista de la aplicación |
| **Comentarios** | Para poder paliar la debilidad de que los usuarios decidan no tener la aplicación nosotros contamos con los datos de las operadoras sobre los registros de localización de los usuarios con lo que el usuario estará "monitorizado" sin saberlo (ver Tabla 1.4) | 
  
<p align="center"> <b>Tabla 2.2</b>
  
 | **<id>003** | Irresponsabilidad de los usuarios en el cumplimiento de las recomendaciones|
| -- | -- |
| **[Versión]** | 1.0 (18/11/2020) |
| **Descripción** | Una vez diagnosticado un positivo y alertado a los posibles contagiados dependemos de la responsabilidad de cada uno de ellos para cumplir con las normas y las restricciones que se les apliquen. En caso de que no sea así tendremos dificultades para  llevar un control de la actividad del usuario y posibles brotes.|
| **Comentarios** | Para resolver el problema contamos con la ventaja de que podremos avisar a las fuerzas del orden para que estén al tanto de las personas que deben estar en  cuarentena y asegurar su cumplimiento (ver Tabla 1.7). También se podrá hacer el control del cumplimiento de la cuarentena, por medio de la localización del dispositivo móvil de los pacientes o por medio de llamadas telefónicas a estos. (ver tabla 1.6).| 
  
<p align="center"> <b>Tabla 2.3</b>
 
 | **<id>004** | Independecia a nivel autonómico en la gestion de los datos|
| -- | -- |
| **[Versión]** |  1.0 (18/11/2020) |
| **Descripción** | Actualmente se han transeferido las competencias en la gestión de la pandemia a las autonomias, teniendo cada una sus propios sistemas de información. |
| **Comentarios** | Para solventar esta debilidad deberemos hablar con cada autonomía para poder adaptar nuestro proyecto a trabajar con cada uno de los respectivos sistemas de información.| 
  
<p align="center"> <b>Tabla 2.4</b>

