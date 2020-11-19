# PANDEMIO

## 1. INTRODUCCIÓN
Ante los resultados decepcionantes obtenidos con la aplicación **Radar Covid** para llevar a cabo el rastreo de los contagios entre los ciudadanos durante la pandemia, el Ministro de Sanidad ha propuesto desarrollar una plataforma que permita rastrear los casos Covid, así como gestionar los datos de los ciudadanos que sean positivos.

<<<<<<< HEAD
<<<<<<< HEAD
Con esta nueva plataforma que se propone desarrollar, se desea mitigar aquellos problemas que se han encontrado en la ya existente aplicación **Radar Covid**. Entre los cuales el comité de expertos resalta que son debidos a que la instalación y el uso de la app NO eran obligatorios, por lo que pocos usuarios la instalaron. Además, dicha aplicación al basarse en el uso de bluetooth, la aplicación era inservible si el bluetooth estaba apagado o bien estaba ocupado.

Se propone que la nueva plataforma a desarrollar pueda llevar a cabo un seguimiento de aquellos ciudadanos que deben cumplir la cuarentena y no la cumplían, asi como aquellos que no acudían a hacerse las pruebas médicas oportunas. Donde resulta importante que se cumpla la ley de datos y los datos de los ciudadanos solo sean usados por las personas autorizadas y sean anonimizados cuando sea posible.
=======
Con esta nueva plataforma que se propone desarrollar, se desea mitigar aquellos problemas que se han encontrado en la ya existente aplicación **Radar Covid**. Entre los cuales el comité de expertos resalta que son debidos a que la instalación y el uso de la aplicación NO eran obligatorios, por lo que pocos usuarios la instalaron y además dicha aplicación al basarse en el uso de bluetooth, la aplicación era inservible si el bluetooth estaba apagado o bien estaba ocupado.

Además, se propone que la nueva plataforma a desarrollar pueda llevar a cabo un seguimiento de aquellos ciudadanos que deben cumplir la cuarentena y no la cumplían, así como aquellos que no acudían a hacerse las pruebas médicas oportunas. Donde resulta importante que se cumpla la ley de datos y los datos de los ciudadanos solo sean usados por las personas autorizadas y sean anonimizados cuando sea posible.
>>>>>>> 7e1458613f795b44406b67ba50a1db5d7bf90743
=======
Con esta nueva plataforma que se propone desarrollar, se desea mitigar aquellos problemas que se han encontrado en la ya existente aplicación **Radar Covid**. Entre los cuales el comité de expertos resalta que son debidos a que la instalación y el uso de la aplicación NO eran obligatorios, por lo que pocos usuarios la instalaron y además dicha aplicación al basarse en el uso de bluetooth, la aplicación era inservible si el bluetooth estaba apagado o bien estaba ocupado.

Además, se propone que la nueva plataforma a desarrollar pueda llevar a cabo un seguimiento de aquellos ciudadanos que deben cumplir la cuarentena y no la cumplían, así como aquellos que no acudían a hacerse las pruebas médicas oportunas. Donde resulta importante que se cumpla la ley de datos y los datos de los ciudadanos solo sean usados por las personas autorizadas y sean anonimizados cuando sea posible.
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef

### 1.1 Alcance
Con el desarrollo de la plataforma PANDEMIO, se busca conseguir un sistema de control e información acerca de los contagios que se dan en una pandemia, en este caso de Covid-19, pero también nos servirá para otras pandemias que se pudieran presentar en un futuro.

Pandemio proporcionará distintos datos acerca de los contagios de los ciudadanos al ministerio de Sanidad, para que dichos datos sean procesados y se tomen las medidas oportunas por parte del juicio de expertos correspondiente. También, se proporcionarán los datos necesarios acerca de los contagios a los ambulatorios, así como a las autoridades correspondientes para que puedan llevar a cabo un control de que los casos positivos cumplen la cuarentena obligatoria cuando sea necesario.
El alcance del proyecto se centra en tres grandes características, el rastreo de los contactos con los casos positivos, gestionar la realización de las pruebas médicas y gestionar el cumplimiento de la cuarentena. Dentro de cada una de estas características se incluirá diferente funcionalidad, a continuación, se muestra un diagrama de característica que plasma cual es el alcance del proyecto de una forma más precisa.
![picture 1](images/e5d1862358a7e70d3ee10eb80bf1c2e63aa3983a3a58056b05b740be66bb8fb3.png)

### 1.2 Objetivos
Entre los objetivos que se desean alcanzar al desarrollar dicha plataforma se encuentran:

- Llevar a cabo un rastreo de los casos positivos entre los ciudadanos, así como conocer las personas que hayan estado en contacto con un positivo (durante un tiempo superior a 15 minutos)
- LLevar a cabo un control del correcto cumplimiento de la cuarentena por aquellos ciudadanos que la deban cumplir, notificando a la autoridad cuando se deja de cumplir la cuarentena.
<<<<<<< HEAD
<<<<<<< HEAD
- LLevar a cabo un control de aquellos ciudadanos que deben presentarse a las pruebas médicas oportunas, así como el resultado de estas.
=======
- Llevar a cabo un control de aquellos ciudadanos que deben presentarse a las pruebas médicas oportunas, así como el resultado de estas.
>>>>>>> 7e1458613f795b44406b67ba50a1db5d7bf90743
=======
- Llevar a cabo un control de aquellos ciudadanos que deben presentarse a las pruebas médicas oportunas, así como el resultado de estas.
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef
- Proporcionar información de los distintos casos positivos que se detectan al ministerio de Sanidad, se debe informar del número de casos positivos que se encuentran en una determinada zona, ya sea por barrios, pueblos, etc. Para que los expertos epidemiólogos puedan tomar las medidas oportunas a partir de estos datos.
- Rastrear donde se han podido ocasionar los contagios entre los casos positivos, para que dicha información sea proporcionada al ministerio de sanidad y pueda tomar las medidas oportunas sobre permitir ciertas actividades o no.

## 2. INFORMACIÓN DEL DOMINIO DEL PROBLEMA
El 17 de noviembre de 2019 se detectó en China el primer caso de Covid-19, a partir de esta fecha y durante todo el año 2020 la situación mundial ha cambiado después de que el 11 de Marzo de 2020 la Organización Mundial de la Salud (**OMS**) declarara la enfermedad Covid-19 como pandemia.

Debido a esta pandemia, se han debido de tomar ciertas medidas, tales como el confinamiento domiciliario durante 99 días, la limitación de aforos en los comercios y los establecimientos, el toque de queda o el cierre de aquellos comercios que no se consideren esenciales. Debido a la cambiante e incierta situación que se está viviendo durante todos estos meses, dichas medidas están sufriendo constante modificaciones e incluso se añaden nuevas medidas, para tomar estas decisiones es necesario conocer las estadísticas y los datos acerca de la pandemia.

Uno de los aspectos más importantes que se deben de tener en cuenta para poder hacer frente a esta pandemia es el rastreo de todos aquellos casos positivos en la población, así como asegurar que los ciudadanos que sean positivos o hayan estado en contacto directo con positivos cumplan la cuarentena durante los días que indiquen los médicos.

Otro aspecto importante a tener en cuenta a la hora de rastrear los casos positivos es que aquellos ciudadanos que hayan estado en contacto con positivos o aquellas personas que tengan síntomas compatibles con Covid-19 acudan a los centros de salud a realizarse las pruebas médicas oportunas.

Para asegurarse que todas estas medidas anteriormente comentadas se cumplan por parte de los ciudadanos se dispone del apoyo de las fuerzas del orden (policía local, nacional, guardia civil y ejército).

### 2.1 Introducción al dominio del problema
A la hora de actuar ante un nuevo caso positivo en Covid-19, se debe seguir un protocolo estricto. El cuál consiste en que una vez que se conoce el resultado positivo de la prueba PCR oportuna, el paciente positivo debe permanecer en cuarentena durante 15 días, en los cuales no podrá salir de casa o incluso de su habitación en caso de que conviva con más personas que no sean positivas.

<<<<<<< HEAD
<<<<<<< HEAD
Después, se llevará a cabo un seguimiento de todas aquellas personas que hayan estado en contacto (durante un tiempo superior a 15 minutos) con el paciente positivo en las 48 horas anteriores a la realización de la prueba PCR, a las cuales se les considerará contacto directo. Los contactos directos deben permanecer en cuarentena hasta que se conozca el resultado de la prueba PCR, si esta es negativa en algunos casos se debe mantener la cuarentena unos días más (depende del tipo de contacto, tiempo, si ha sido con mascarilla o sin ella,etc) en caso de que lo indique el responsable sanitario. Si la prueba es positiva, se repetirá el mismo proceso con los contactos directos del nuevo caso positivo.
=======
Después, se llevará a cabo un seguimiento de todas aquellas personas que hayan estado en contacto (durante un tiempo superior a 15 minutos) con el paciente positivo en las 48 horas anteriores a la realización de la prueba PCR, a las cuales se les considerará contacto directo. Los contactos directos deben permanecer en cuarentena hasta que se conozca el resultado de la prueba PCR, si esta es negativa en algunos casos se debe mantener la cuarentena unos días más (depende del tipo de contacto, tiempo, si ha sido con mascarilla o sin ella, etc.) en caso de que lo indique el responsable sanitario. Si la prueba es positiva, se repetirá el mismo proceso con los contactos directos del nuevo caso positivo.
>>>>>>> 7e1458613f795b44406b67ba50a1db5d7bf90743
=======
Después, se llevará a cabo un seguimiento de todas aquellas personas que hayan estado en contacto (durante un tiempo superior a 15 minutos) con el paciente positivo en las 48 horas anteriores a la realización de la prueba PCR, a las cuales se les considerará contacto directo. Los contactos directos deben permanecer en cuarentena hasta que se conozca el resultado de la prueba PCR, si esta es negativa en algunos casos se debe mantener la cuarentena unos días más (depende del tipo de contacto, tiempo, si ha sido con mascarilla o sin ella, etc.) en caso de que lo indique el responsable sanitario. Si la prueba es positiva, se repetirá el mismo proceso con los contactos directos del nuevo caso positivo.
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef

### 2.2 Glosario de términos
- **Caso positivo:** Aquella persona que tras la realización de la prueba oportuna ha indicado que tiene la enfermedad por la cual se hace la prueba.
- **Confinamiento:** Acción que se lleva cabo para mantener a una persona positiva dentro de unos límites (en este caso su vivienda), con el fin de que no contagie al resto de la población.
- **Contacto directo:** Aquella persona que ha estado en contacto con un caso confirmado de Covid-19 desde las 48 horas antes del inicio de síntomas o del diagnóstico. Entre estas, son más probables de ser positivos aquellas que hayan estado en el mismo lugar que un caso positivo, a una distancia menor de 2 metros durante un tiempo superior de 15 minutos.
- **Covid-19:** Enfermedad infecciosa causada por el coronavirus SARS-COV-2.
- **Cuarentena:** Ponerse en cuarentena significa separarse de los demás porque ha estado expuesto a alguien con COVID‑19 aunque usted mismo no tenga síntomas. Durante la cuarentena, debe vigilar su estado para detectar síntomas. El objetivo de la cuarentena es prevenir la transmisión.
- **Pandemia:** Enfermedad epidémica que se extiende a muchos países o que ataca a casi todos los individuos de una localidad o región.
- **Prueba PCR:** Tipo de prueba de diagnóstico, que permite detectar un caso positivo de Covid-19.
- **Toque de queda:**  se refiere a la prohibición o restricción, establecida por instituciones gubernamentales, de circular libremente por las calles de una ciudad o permanecer en lugares públicos, permaneciendo los habitantes únicamente en sus hogares salvo excepciones de necesidad o urgencia.

## 3. DESCRIPCIÓN DE LA SITUACIÓN ACTUAL
Desde que se declaró el estado de alarma como consecuencia de la actual pandemia que estamos viviendo, se han debido de tomar diversas medidas, las cuales han ido cambiando constantemente, debido a la cambiante situación que se plantea con la pandemia cada día. Para poder tomar estas medidas, el gobierno junto con el grupo de expertos indicado debe conocer grandes volúmenes de información acerca de la pandemia y contrastarla.

Entre las medidas tomadas cabe destacar el confinamiento domiciliario al cual hemos estado sometidos cerca de 3 meses. Una vez que la situación mejoró se ha permitido el salir a la calle, pero con un límite en el número de personas que se podían juntar. Los locales comerciales, la hostelería, las grandes superficies han debido de tomar distintas medidas respecto al aforo y a los protocolos que se debían respetar.

Actualmente, las medidas tomadas son distintas dependiendo de las comunidades autónomas (dependen de los datos de la pandemia en dichas comunidades), y además dichas medidas cambian constantemente; luego no podemos suponer que la situación de hoy en día sea igual a la que se va a presentar mañana.

Actualmente el Ministerio de Sanidad posee una aplicación para el control y seguimiento ciudadano en términos de la pandemia mundial que nos asola causada por el COVID-19; sin embargo, esta aplicación no es del agrado del ministerio por diversas razones. Para poder llevar a cabo una mejor gestión, que la proporcionada por la aplicación actual, en caso de producirse una nueva pandemia, el ministerio quiere hacerse con nuestros servicios para la creación de una nueva aplicación que sí satisfaga sus necesidades ante una posible situación similar en el futuro. 

Hoy en día todo el mundo lleva su móvil en todo momento consigo, móviles conectados a la red y que funcionan por medio de aplicaciones. Nos aprovecharemos este entorno tecnológico ya que es ideal para el seguimiento ciudadano. Puesto que las fuerzas del orden, así como el sector sanitario posee también de dispositivos conectados a la red podremos comunicarnos con ellos. De esta manera se podrá comprobar el cumplimiento de las cuarentenas y las obligaciones de los ciudadanos por parte de los cuerpos de seguridad del estado, así como recibir listas, los ambulatorios, con las personas que deberán hacerse las pruebas para poder poner en conocimiento de las fuerzas del orden cualquier incumplimiento.

En la actualidad en torno al 90% de la población española dispone de un teléfono móvil, luego esto tiene las ventajas comentadas anteriormente para poder hacer el seguimiento oportuno a los ciudadanos de cara a obtener datos válidos para gestionar la pandemia. Sin embargo, el otro tanto por ciento de la población que no dispone de teléfono móvil se encuentra en una situación especial que se debe tener en cuenta de cara a conocer cómo se va a actuar en nuestra plataforma en estos casos. Dado que dicho porcentaje de la población es muy reducido y además se corresponde con la población de menor edad y la población de edades avanzadas el rastreo de los contactos directos de estas personas se puede rastrear de forma manual con los métodos actuales, dado que estos grupos de población no tienen muchos contactos sociales distintos. A la hora de controlar el cumplimiento de la cuarentena en este tipo de usuarios, se delegará la responsabilidad en las fuerzas del orden, las cuales deberán hacer los controles oportunos, lo cual es viable al ser un número reducido de personas. 

Dado que, con nuestra plataforma, Pandemio, vamos a poder obtener distintos datos de los ciudadanos, se van a manejar grandes volúmenes de información acerca de estos, lo que conlleva que los algoritmos utilizados para obtener información de estos datos o para manejar estos datos sean complejos. Dichos datos debe ser información anonimizada, tan solo podrán acceder a los datos los usuarios autorizados para ello como los agentes de la autoridad o los ambulatorios. Hoy en día, se debe tener un especial cuidado a la hora de manejar datos relacionados con las personas, y se debe cumplir la ley de protección de datos.

Debido a que la situación actual ha llevado a que se transfieran las competencias a las autonomías y cada una tiene sus propios sistemas de información, para poder realizar una implementación correcta en todas las autonomías deberemos de establecer distintas interfaces de comunicación entre ellas para poder acceder a sus sistemas de información y así acceder a los datos de los pacientes de cada autonomía.

### 3.1 Pros y Contras de la Situación Actual
La situación actual hace que para la implementación de la aplicación que se nos solicita se nos presentan varios puntos que podrían ser de ayuda, pero también cuestiones que suponen un obstáculo a la hora de cumplir con las necesidades del cliente. 

Puesto que tenemos una aplicación realizada y probada recientemente en el mismo ámbito y con propósitos similares podremos realizar comparaciones con ella y establecer un punto de partida sólido. Tendremos en cuenta aquellos aspectos que han funcionado y aquellos que no y sus razones para poder aprender de ella y mejorar.

#### 3.1.1 Fortalezas de la Situación Actual
Para poder enfrentarnos al problema con un punto de partida fuerte aprovecharemos que tenemos el backup o copia de seguridad de la aplicación __Radar Covid__ de la que podemos sacar numerosas conclusiones para usarlas en nuestro favor.

<<<<<<< HEAD
<<<<<<< HEAD
Puesto que la situación de la pandemia actual es una situación crítica se nos proporcionarán ciertos privilegios y facilidades proporcionandonos legalidad para ciertos asuntos que ahora mismo suponen un problema.
=======
Puesto que la situación de la pandemia actual es una situación crítica se nos proporcionarán ciertos privilegios y facilidades proporcionándonos legalidad para ciertos asuntos que ahora mismo suponen un problema.
>>>>>>> 7e1458613f795b44406b67ba50a1db5d7bf90743
=======
Puesto que la situación de la pandemia actual es una situación crítica se nos proporcionarán ciertos privilegios y facilidades proporcionándonos legalidad para ciertos asuntos que ahora mismo suponen un problema.
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef

De toda esta situación podemos resumir las siguientes fortalezas en cuanto a nuestra situación actual:

| **\<id>001** | Reciente pandemia del COVID-19 |
| -- | -- |
| **[Versión]** | 1.0 (17/11/2020) |
<<<<<<< HEAD
<<<<<<< HEAD
| **Descripción** | Dado que actualmente existe la pandemia del Covid-19, hemos adquirido la suficiente experiencia de como se debe actuar ante una pandemia y cuáles deben ser las medidas a tomar. Es decir, tendremos un conocimiento previo y un conjunto de técnicas que se podrán aplicar de cara a controlar la pandemia y no actuaremos desde cero. |
| **Comentarios** | En la actualidad se conocen los protocolos de actuación ante una pandemia, la sociedad conoce el como actuar y dispone de una experiencia previa de ello. Además se dispone de datos previos y estudios acerca de la eficacia de las diferenetes mediadas tomadas en la actual pandemia. |
=======
| **Descripción** | Dado que actualmente existe la pandemia del Covid-19, hemos adquirido la suficiente experiencia de cómo se debe actuar ante una pandemia y cúales deben ser las medidad a tomar. Es decir, tendremos un conocimiento previo y un conjunto de técnicas que se podrán aplicar de cara a controlar la pandemia y no actuaremos desde cero. |
| **Comentarios** | En la actualidad se conocen los protocolos de actuación ante una pandemia, la sociedad conoce el cómo actuar y dispone de una experiencia previa de ello. Además, se dispone de datos previos y estudios acerca de la eficacia de las diferentes mediadas tomadas en la actual pandemia. |
>>>>>>> 7e1458613f795b44406b67ba50a1db5d7bf90743
=======
| **Descripción** | Dado que actualmente existe la pandemia del Covid-19, hemos adquirido la suficiente experiencia de cómo se debe actuar ante una pandemia y cúales deben ser las medidad a tomar. Es decir, tendremos un conocimiento previo y un conjunto de técnicas que se podrán aplicar de cara a controlar la pandemia y no actuaremos desde cero. |
| **Comentarios** | En la actualidad se conocen los protocolos de actuación ante una pandemia, la sociedad conoce el cómo actuar y dispone de una experiencia previa de ello. Además, se dispone de datos previos y estudios acerca de la eficacia de las diferentes mediadas tomadas en la actual pandemia. |
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef
  
<p align="center"> <b>Tabla 1.1: Fortalezas de la situación actual.</b> </p>
  
| **\<id>002** | Referencia Aplicación "Radar Covid" |
| -- | -- |
| **[Versión]** | 1.0 (17/11/2020) |
| **Descripción** | En la actualidad existe otra aplicación del ministerio llamada Radar Covid, la cual la base de su funcionalidad es parecida a la de nuestra plataforma, la idea de controlar los contagios surge de esta aplicación y se tratará de mejorar las deficiencias encontradas en ella. A partir de esta aplicación se dispone de una base para comenzar a desarrollar nuestra plataforma. |
| **Comentarios** | Usaremos como fortaleza de esta aplicación la idea de controlar los contactos con los positivos, pero la implementación sufrirá modificaciones, ya que se usarán los datos proporcionados por las operadoras móviles, en vez de el uso de bluetooth por los problemas encontrados en su uso. |
  
<p align="center"> <b>Tabla 1.2: Fortalezas de la situación actual.</b> </p>
    
| **\<id>003** | Existencia de datos sobre la población |
| -- | -- |
| **[Versión]** | 1.0 (18/11/2020) |
| **Descripción** | Debido a la actual pandemia del COVID-19 los distintos estamentos del gobierno y sus autonomías han podido recabar información sobre la población en vistas a poder prevenir la extensión del virus. |
| **Comentarios** | Con cada llamada a los teléfonos habilitados para la población para temas de COVID-19 el protocolo marcaba imprescindible recabar datos sobre la persona que realizaba la llamada, tales como la edad o el código postal. De confirmarse el positivo, y con el objetivo de realizar el rastreo se le preguntaba al usuario las personas con las que había mantenido contacto en los días previos, así como su dirección y los lugares donde había estado durante un periodo largo de tiempo. Toda esa información que ya tenemos podría ser usada en un futuro para realizar estudios que nos permitieran llevar a cabo una actuación más rápida y eficiente a la hora de encontrar infectados y adelantarnos en una posible nueva pandemia para minimizar la propagación. |
  
<p align="center"> <b>Tabla 1.3: Fortalezas de la situación actual.</b> </p>
  
| **\<id>004** | Acceso a los datos de los operadores móviles |
| -- | -- |
| **[Versión]** | 1.0 (17/11/2020) |
| **Descripción** | Gracias a que la situación de pandemia ha llevado a que se declare un estado de alerta sanitaria se dispone de una situación en la cual se pueden hacer los cambios legales necesarios, entre ellos que los datos acerca de los ciudadanos sean proporcionados por las propias operadoras con el fin de usar esta información para nuestra plataforma y no con otros fines. Dichos datos son los más precisos que se pueden obtener, y en ellos no tiene que intervenir el usuario, sino que son obtenidos sin su "consentimiento". |
| **Comentarios** | Tomaremos como fortaleza el hecho de que al obtener los datos de las operadoras móviles, el usuario no se puede negar a proporcionar dichos datos y además, se evitan los posibles despistes de tener desconectado el bluetooth como ocurría con Radar Covid o que al utilizarse otro dispositivo, no se registren los nuevos contactos directos. |
  
<p align="center"> <b>Tabla 1.4: Fortalezas de la situación actual.</b> </p>
  
| **\<id>005** | Posibilidad de realizar los cambios legales necesarios |
| -- | -- |
| **[Versión]** | 1.0 (17/11/2020) |
| **Descripción** | Dado que nuestro cliente es el Ministerio de Sanidad, se está planteando crear un estado de alerta sanitaria o pandemia con el fin de que dicho estado de alerta sirva como paraguas para poder realizar los cambios legales necesarios a la hora de poder implementar de una forma correcta nuestra plataforma y poder obtener los datos necesarios para ello. |
| **Comentarios** | Se tomará como fortaleza el hecho de que, si existe algún impedimento legal a la hora de poder implementar nuestra plataforma, al estar destinada al gobierno se podrán realizar los cambios legales necesarios para eliminar dichos impedimentos o reducirles. |
  
<p align="center"> <b>Tabla 1.5: Fortalezas de la situación actual.</b> </p>
  
| **\<id>006** | Disponibilidad de móvil de gran parte de la población |
| -- | -- |
| **[Versión]** | 1.0 (17/11/2020) |
| **Descripción** | En la actualidad cerca del 90% de la población española dispone de teléfono móvil, luego esto es una gran fortaleza dado que podremos obtener información de una gran parte de la población gracias a sus dispositivos móviles. Además, se podrá utilizar a su vez como dispositivo para controlar que se cumplen con las cuarentenas obligatorias así como medio de comunicación con el ciudadano. |
<<<<<<< HEAD
<<<<<<< HEAD
| **Comentarios** | El pequeño porcentaje de la población que no dispone de teléfono movil se suele corresponder con niños o personas de edad avanzada, las cuales es más fácil de rastrear sus contagios y si cumplen la cuarentena obligatoria, para ello hará falta de la actuación de los agentes de la autoridad o personas asignadas para ello. |
=======
| **Comentarios** | El pequeño porcentaje de la población que no dispone de teléfono móvil se suele corresponder con niños o personas de edad avanzada, las cuales es más fácil de rastrear sus contagios y si cumplen la cuarentena obligatoria, para ello hará falta de la actuación de los agentes de la autoridad o personas asignadas para ello. |
>>>>>>> 7e1458613f795b44406b67ba50a1db5d7bf90743
=======
| **Comentarios** | El pequeño porcentaje de la población que no dispone de teléfono móvil se suele corresponder con niños o personas de edad avanzada, las cuales es más fácil de rastrear sus contagios y si cumplen la cuarentena obligatoria, para ello hará falta de la actuación de los agentes de la autoridad o personas asignadas para ello. |
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef
  
<p align="center"> <b>Tabla 1.6: Fortalezas de la situación actual.</b> </p>
  
| **\<id>007** | Comunicación con las fuerzas del orden y los sanitarios |
| -- | -- |
| **[Versión]** | 1.0 (18/11/2020) |
<<<<<<< HEAD
<<<<<<< HEAD
| **Descripción** | Para poder llevar a cabo un control eficiente de las personas que deben realizarse las pruebas enviaremos a los ambulatorios los listados de personas que deben hacerse las pruebas, y estos podrán notificar a la autoridad el inclumplimiento. Por su parte las fuerzas del orden podrán comprobar el cumplimiento de las cuarentenas y las obligaciones impuestas a los ciudadanos |
| **Comentarios** | Nuestra labor será la de recabar información que proporcionaremos a los ambulatorios y al gobierno para que puedan llevar a cabo las acciones pertinentes, pero el hecho de que estemos en comunicacion directa con organismos con tanto "poder" debería influir positivamente en el éxito de nuestro proyecto |
=======
| **Descripción** | Para poder llevar a cabo un control eficiente de las personas que deben realizarse las pruebas enviaremos a los ambulatorios los listados de personas que deben hacerse las pruebas, y estos podrán notificar a la autoridad el incumplimiento. Por su parte las fuerzas del orden podrán comprobar el cumplimiento de las cuarentenas y las obligaciones impuestas a los ciudadanos. |
| **Comentarios** | Nuestra labor será la de recabar información que proporcionaremos a los ambulatorios y a sanidad para que puedan llevar a cabo las acciones pertinentes, pero el hecho de que estemos en comunicación directa con organismos con tanto "poder" debería influir positivamente en el éxito de nuestro proyecto. |
>>>>>>> 7e1458613f795b44406b67ba50a1db5d7bf90743
=======
| **Descripción** | Para poder llevar a cabo un control eficiente de las personas que deben realizarse las pruebas enviaremos a los ambulatorios los listados de personas que deben hacerse las pruebas, y estos podrán notificar a la autoridad el incumplimiento. Por su parte las fuerzas del orden podrán comprobar el cumplimiento de las cuarentenas y las obligaciones impuestas a los ciudadanos. |
| **Comentarios** | Nuestra labor será la de recabar información que proporcionaremos a los ambulatorios y a sanidad para que puedan llevar a cabo las acciones pertinentes, pero el hecho de que estemos en comunicación directa con organismos con tanto "poder" debería influir positivamente en el éxito de nuestro proyecto. |
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef
  
<p align="center"> <b>Tabla 1.7: Fortalezas de la situación actual.</b> </p>

#### 3.1.2 Debilidades de la situación Actual
Debido a la complejidad de la situación actual y a que la aplicación __Radar Covid__ ha ofrecido muchos puntos en contra pero pocos a favor nos encontramos en una posición donde todo aquello que queramos implementar puede ser muy buena idea sobre el papel pero causar muchas dificultades en un contexto real.

<<<<<<< HEAD
<<<<<<< HEAD
Por otro lado, para poder llevar a cabo ciertas operaciones vamos a necesitar del uso de los datos de localización de los móviles y eso, por el momento supone un problema. Aún así, cuando esto esté solucionado deberemos lidiar con el cumplimiento de la ley de protección de datos.
=======
Por otro lado, para poder llevar a cabo ciertas operaciones vamos a necesitar del uso de los datos de localización de los móviles y eso, por el momento supone un problema. Aun así, cuando esto esté solucionado deberemos lidiar con el cumplimiento de la ley de protección de datos.
>>>>>>> 7e1458613f795b44406b67ba50a1db5d7bf90743
=======
Por otro lado, para poder llevar a cabo ciertas operaciones vamos a necesitar del uso de los datos de localización de los móviles y eso, por el momento supone un problema. Aun así, cuando esto esté solucionado deberemos lidiar con el cumplimiento de la ley de protección de datos.
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef

De toda esta situación podemos resumir las siguientes debilidades en cuanto a nuestra situación actual:

| **\<id>001** | Problemas en el uso de Bluetooth |
| -- | -- |
| **[Versión]** | 1.0 (18/11/2020) |
<<<<<<< HEAD
<<<<<<< HEAD
| **Descripción** | La aplicación Radar Covid intentó realizar la localización de los usuarios y sus interacciones por medio del bluetooth sin embargo resultó ser inservible si este estaba apagado o siendo usado por otro accesorio.|
| **Comentarios** | Supone una debilidad el hecho de que la "primera opción" para localizar a los usuarios haya fracasado y por tanto tendremos que buscar otra opción mejor.| 
=======
| **Descripción** | La aplicación Radar Covid intentó realizar la localización de los usuarios y sus interacciones por medio del bluetooth sin embargo resultó ser inservible si este estaba apagado o siendo usado por otro accesorio. |
| **Comentarios** | Supone una debilidad el hecho de que la "primera opción" para localizar a los usuarios haya fracasado y por tanto tendremos que buscar otra opción mejor. | 
>>>>>>> 7e1458613f795b44406b67ba50a1db5d7bf90743

<p align="center"> <b>Tabla 2.1: Debilidades de la situación actual.</b> </p>
  
<<<<<<< HEAD
| **\<id>002** | Opcionalidad de los usuarios para estar controlados|
=======
| **<id>002** | Opcionalidad de los usuarios para estar controlados |
>>>>>>> 7e1458613f795b44406b67ba50a1db5d7bf90743
=======
| **Descripción** | La aplicación Radar Covid intentó realizar la localización de los usuarios y sus interacciones por medio del bluetooth sin embargo resultó ser inservible si este estaba apagado o siendo usado por otro accesorio. |
| **Comentarios** | Supone una debilidad el hecho de que la "primera opción" para localizar a los usuarios haya fracasado y por tanto tendremos que buscar otra opción mejor. | 

<p align="center"> <b>Tabla 2.1: Debilidades de la situación actual.</b> </p>
  
| **<id>002** | Opcionalidad de los usuarios para estar controlados |
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef
| -- | -- |
| **[Versión]** | 1.0 (18/11/2020) |
| **Descripción** | La obtención de Radar Covid por parte del usuario era totalmente voluntaria, lo que supone un gran problema ya que el usuario que lo deseara podría ser "invisible" desde el punto de vista de la aplicación. |
| **Comentarios** | Para poder paliar la debilidad de que los usuarios decidan no tener la aplicación nosotros contamos con los datos de las operadoras sobre los registros de localización de los usuarios con lo que el usuario estará "monitorizado" sin saberlo (ver Tabla 1.4). | 
  
<p align="center"> <b>Tabla 2.2: Debilidades de la situación actual.</b> </p>
  
<<<<<<< HEAD
<<<<<<< HEAD
| **\<id>003** | Irresponsabilidad de los usuarios en el cumplimiento de las recomendaciones|
=======
| **<id>003** | Irresponsabilidad de los usuarios en el cumplimiento de las recomendaciones |
>>>>>>> 7e1458613f795b44406b67ba50a1db5d7bf90743
=======
| **<id>003** | Irresponsabilidad de los usuarios en el cumplimiento de las recomendaciones |
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef
| -- | -- |
| **[Versión]** | 1.0 (18/11/2020) |
| **Descripción** | Una vez diagnosticado un positivo y alertado a los posibles contagiados dependemos de la responsabilidad de cada uno de ellos para cumplir con las normas y las restricciones que se les apliquen. En caso de que no sea así tendremos dificultades para llevar un control de la actividad del usuario y posibles brotes. |
| **Comentarios** | Para resolver el problema contamos con la ventaja de que podremos avisar a las fuerzas del orden para que estén al tanto de las personas que deben estar en cuarentena y asegurar su cumplimiento (ver Tabla 1.7). También se podrá hacer el control del cumplimiento de la cuarentena, por medio de la localización del dispositivo móvil de los pacientes o por medio de llamadas telefónicas a estos. (ver tabla 1.6). | 
  
<p align="center"> <b>Tabla 2.3: Debilidades de la situación actual.</b> </p>
 
| **\<id>004** | Independencia a nivel autonómico en la gestión de los datos |
| -- | -- |
| **[Versión]** |  1.0 (18/11/2020) |
| **Descripción** | Actualmente se han transferido las competencias en la gestión de la pandemia a las autonomías, teniendo cada una sus propios sistemas de información. |
| **Comentarios** | Para solventar esta debilidad deberemos hablar con cada autonomía para poder adaptar nuestro proyecto a trabajar con cada uno de los respectivos sistemas de información. | 
  
<p align="center"> <b>Tabla 2.4: Debilidades de la situación actual.</b> </p>

<<<<<<< HEAD
<<<<<<< HEAD
### 3.2 Modelos de Procesos de Negocios Acutales
En este apartado representaremos y describiremos todos aquellos procesos que se llevarán acabo para gestionar los contagios que se producen en la pandemia, asi como los procesos que se emplearán para controlar el cumplimiento de la cuarentena obligatoria por parte de los ciudadanos positivos. También se tendrán en cuenta todos aquellos procesos en los que se gestionen las distintas pruebas médicas que se deben realizar los ciudadanos, así como informales a estos de los resultados.Por otro lado, se especificará como debe ser la comunicación con el resto de actores que intervienen en la plataforma como los agentes de la autoridad o el gobierno al que se le proporcionarán todos los datos obtenidos con la plataforma para que puedan tomarse las medidas oportunas por parte de los expertos correspondientes.
=======
### 3.2 Modelos de Procesos de Negocios Actuales
En este apartado representaremos y describiremos todos aquellos procesos que se llevarán a cabo para gestionar los contagios que se producen en la pandemia, así como los procesos que se emplearán para controlar el cumplimiento de la cuarentena obligatoria por parte de los ciudadanos positivos. También se tendrán en cuenta todos aquellos procesos en los que se gestionen las distintas pruebas médicas que se deben realizar los ciudadanos, asi como informales a estos de los resultados. Por otro lado, se especificará como debe ser la comunicación con el resto de los actores que intervienen en la plataforma como los agentes de la autoridad o el gobierno al que se le proporcionarán todos los datos obtenidos con la plataforma para que puedan tomarse las medidas oportunas por parte de los expertos correspondientes.
>>>>>>> 7e1458613f795b44406b67ba50a1db5d7bf90743
=======
### 3.2 Modelos de Procesos de Negocios Actuales
En este apartado representaremos y describiremos todos aquellos procesos que se llevarán a cabo para gestionar los contagios que se producen en la pandemia, así como los procesos que se emplearán para controlar el cumplimiento de la cuarentena obligatoria por parte de los ciudadanos positivos. También se tendrán en cuenta todos aquellos procesos en los que se gestionen las distintas pruebas médicas que se deben realizar los ciudadanos, asi como informales a estos de los resultados. Por otro lado, se especificará como debe ser la comunicación con el resto de los actores que intervienen en la plataforma como los agentes de la autoridad o el gobierno al que se le proporcionarán todos los datos obtenidos con la plataforma para que puedan tomarse las medidas oportunas por parte de los expertos correspondientes.
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef

#### 3.2.1 Descripción de los Actores de Negocio Actuales
Los actores de negocio actuales son todas aquellas personas o entidades que están involucradas en la gestión de la pandemia actual y en los procesos de negocio llevados a cabo. Dichos actores se corresponden con: ciudadanos, gobierno, autoridades y ambulatorios. Necesarios para que la información se transmita de manera segura.

| **\<id>001** | Ciudadano |
| -- | -- |
<<<<<<< HEAD
| **[Versión]** | 1.0(17/11/2020) |
<<<<<<< HEAD
| **[Dependencias]** | El cuidadano es la piedra angular del proceso y por ello la mayoría de los procesos de negocio actuales dependen de él. El proceso 1, "Hacer prueba PCR", depende directamente del cuidadano ya que es objeto de dicha prueba. Por el mismo motivo también depende el proceso 2, "Registrar resultado de la prueba". El proceso 3, "Rastreo por contacto con un positivo", depende también de este actor ya que un resultado positivo en un cuidadano recae en la realización de pruebas en otros ciudadanos. Por último el proceso control de la cuarentena y seguimiento del estado del paciente, proceso 4, depende del cuidadano por razones obvias.|
| **Descripción** | Este actor de negocio actual es el actor principal en torno al que gira todo el sistema. Representa a cada uno de los ciudadanos. De este actor se obtiene la informacion de su localización por medio de la tecnología bluetooth de su móvil para que si se produce un positivo poder alertar a aquellas personas que hayan tenido contacto. La llamada de un ciudadano por padecer síntomas y la realización de una PCR es lo que dispara los diferentes procesos de negocio, ya que si se produce un positivo este debe guardar una cuarentena sobre la que se realiza un seguimiento además de iniciarse un rastreo de los posibles cuidadanos que también puedan haber sido contagiados. La información sobre los resultados de las pruebas y sobre el seguimiento del cuidadano positivo se pone en conocimiento de los rastreadores que llevan a cabo las acciones pertinentes.|
=======
| **[Dependencias]** | El ciudadano es la piedra angular del proceso y por ello la mayoría de los procesos de negocio actuales dependen de él. El proceso 1, "Hacer prueba PCR", depende directamente del ciudadano ya que es objeto de dicha prueba. Por el mismo motivo también depende el proceso 2, "Registrar resultado de la prueba". El proceso 3, "Rastreo por contacto con un positivo", depende también de este actor ya que un resultado positivo en un ciudadano recae en la realización de pruebas en otros ciudadanos. Por último el proceso control de la cuarentena y seguimiento del estado del paciente, proceso 4, depende del ciudadano por razones obvias. |
| **Descripción** | Este actor de negocio actual es el actor principal en torno al que gira todo el sistema. Representa a cada uno de los ciudadanos. De este actor se obtiene la información de su localización por medio de la tecnología bluetooth de su móvil para que si se produce un positivo poder alertar a aquellas personas que hayan tenido contacto. La llamada de un ciudadano por padecer síntomas y la realización de una PCR es lo que dispara los diferentes procesos de negocio, ya que si se produce un positivo este debe guardar una cuarentena sobre la que se realiza un seguimiento además de iniciarse un rastreo de los posibles ciudadanos que también puedan haber sido contagiados. La información sobre los resultados de las pruebas y sobre el seguimiento del ciudadano positivo se pone en conocimiento de los rastreadores que llevan a cabo las acciones pertinentes. |
>>>>>>> 7e1458613f795b44406b67ba50a1db5d7bf90743
=======
| **[Versión]** | 1.0 (17/11/2020) |
| **[Dependencias]** | El ciudadano es la piedra angular del proceso y por ello la mayoría de los procesos de negocio actuales dependen de él. El proceso 1, "Hacer prueba PCR", depende directamente del ciudadano ya que es objeto de dicha prueba. Por el mismo motivo también depende el proceso 2, "Registrar resultado de la prueba". El proceso 3, "Rastreo por contacto con un positivo", depende también de este actor ya que un resultado positivo en un ciudadano recae en la realización de pruebas en otros ciudadanos. Por último el proceso control de la cuarentena y seguimiento del estado del paciente, proceso 4, depende del ciudadano por razones obvias. |
| **Descripción** | Este actor de negocio actual es el actor principal en torno al que gira todo el sistema. Representa a cada uno de los ciudadanos. De este actor se obtiene la información de su localización por medio de la tecnología bluetooth de su móvil para que si se produce un positivo poder alertar a aquellas personas que hayan tenido contacto. La llamada de un ciudadano por padecer síntomas y la realización de una PCR es lo que dispara los diferentes procesos de negocio, ya que si se produce un positivo este debe guardar una cuarentena sobre la que se realiza un seguimiento además de iniciarse un rastreo de los posibles ciudadanos que también puedan haber sido contagiados. La información sobre los resultados de las pruebas y sobre el seguimiento del ciudadano positivo se pone en conocimiento de los rastreadores que llevan a cabo las acciones pertinentes. |
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef
| **Comentarios** | De la información obtenida por medio de los ciudadanos positivos, como la residencia, los puntos de visita frecuentes o las personas con las que ha mantenido contacto se sacan conclusiones por medio de su análisis que puedan dar lugar a toma de decisiones. |

<p align="center"> <b>Tabla 3.1: Actores de negocio.</b> </p>

| **\<id>002** | Gobierno |
| -- | -- |
<<<<<<< HEAD
| **[Versión]** | 1.0(17/11/2020) |
=======
| **[Versión]** | 1.0 (17/11/2020) |
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef
| **[Dependencias]** | De este actor depende el proceso de negocio 5, "Toma de decisiones", ya que es el encargado de tomar las medidas o imponer las restricciones en función del análisis de la información disponible. |
| **Descripción** | Este actor de negocio actual representa al gobierno, en concreto al ministro de sanidad, al que se le suministrarán todos los datos y estadísticas que se han obtenido por medio del procesamiento de los datos capturados de los ciudadanos y procesados. Dicho actor se encargará como entidad de tomar las decisiones oportunas en función de los datos suministrados por la plataforma, en base a diferentes criterios. |
| **Comentarios** | Es un actor que se encuentra "aislado" del proceso de detección y seguimiento de positivos pero que será muy importante debido a su capacidad de toma de decisiones. Este actor puede imponer medidas nuevas, protocolos diferentes y alterar de manera importante todos los procesos tal y como se llevan a cabo hasta ahora. Es por ello que, aunque se encuentre fuera del flujo normal es importantísimo incluirlo por su capacidad de cambiar el mismo. |

<p align="center"> <b>Tabla 3.2: Actores de negocio.</b> </p>

| **\<id>003** | Autoridades |
| -- | -- |
<<<<<<< HEAD
| **[Versión]** | 1.0(17/11/2020) |
=======
| **[Versión]** | 1.0 (17/11/2020) |
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef
| **[Dependencias]** | Dicho actor participa en los procesos de negocio 3 Rastreo por contacto con positivo y en el proceso 4 llevar seguimiento del paciente y control de su cuarentena. |
| **Descripción** | Este actor de negocio actual representa a las fuerzas del orden (policía local, nacional, guardia civil y el ejército) que se encargan de rastrear cuales han sido los contactos directos con los positivos y proveer dicha información a los ambulatorios para que sean los encargados de llamar a dichos contactos directos para que se les realicen las pruebas médicas oportunas. También son los encargados de controlar el cumplimiento de las cuarentenas obligatorias por parte de los ciudadanos que deban de cumplirlas, para ello se encargan de hacer llamadas telefónicas o videollamadas con los pacientes positivos para comprobar que se encuentran en casa cumpliendo la cuarentena. |
| **Comentarios** | A este actor en determinadas ocasiones se les llama rastreadores, y llevaran a cabo la misión de rastrear el cómo se producen los contagios entre los positivos, asi como obtener cuales son los brotes de dichos contagios, para ello tan solo disponen de la información proporcionada por los pacientes positivos. |

<p align="center"> <b>Tabla 3.3: Actores de negocio.</b> </p>

| **\<id>004** | Ambulatorio |
| -- | -- |
<<<<<<< HEAD
| **[Versión]** | 1.0(17/11/2020) |
=======
| **[Versión]** | 1.0 (17/11/2020) |
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef
| **[Dependencias]** | Este actor entra en juego en la mayoría de los procesos de negocio, dado que es el conocedor de cómo se debe gestionar la pandemia y se encarga de mediar en cómo se debe actuar en los distintos casos. Los procesos de negocio en los que participa son 1 Hacer prueba PCR, 2 Registrar resultado de la prueba PCR, 3 rastreo por contacto con positivo, 4 llevar seguimiento del paciente y control de su cuarentena y 5 interpretación de los datos. |
| **Descripción** | Este actor de negocio actual representa al centro de salud, asi como los responsables médicos, se encargan de determinar si se les debe de realizar las pruebas a los pacientes ante la aparición de síntomas o por contacto directo, también se encargan de concretar las citas para la realización de las pruebas médicas con los pacientes, así como informarles de los resultados obtenidos en dichas pruebas y en caso de ser positivos solicitan los datos de los contactos directos. <br> Por otra parte, se encargan de registrar los resultados de dichas pruebas en la base de datos del centro de salud, para que posteriormente pueda ser proporcionada esta información al gobierno. También se encargan de realizar un seguimiento de la evolución del estado del paciente durante la cuarentena por medio de las llamadas telefónicas. |
| **Comentarios** | Dicho actor en determinadas ocasiones se les llama responsable Covid y es el encargado de realizar todas las acciones anteriormente comentadas respecto a la gestión de los casos covid en cada uno de los ambulatorios. |

<p align="center"> <b>Tabla 3.4: Actores de negocio.</b> <br> </p>

#### 3.2.2 Descripción de Procesos de Negocio Actuales
En este apartado se comentarán cúales son los procesos de negocio que se llevan a cabo en la actualidad para gestionar la pandemia. Dichos procesos son en los que se basará nuestra plataforma para agilizarlos y poder ser llevadas a cabo de una forma más automatizada. De forma general, se comentará cual es el flujo de procesos que se han de llevar a cabo cuando se detectan los síntomas compatibles con la enfermedad. Dichos procesos son los siguientes:

| **\<id>001** | Hacer prueba PCR |
| -- | -- |
<<<<<<< HEAD
| **[Versión]** | 1.0(17/11/2020) |
<<<<<<< HEAD
| **[Dependencias]** | En algunos casos depende del proceso de negocio 3, Rastreo de contacto con el positivo, sin embargo en otros casos no hay ninguna dependencia cuando se registra un caso aislado. |
| **Descripción** | En la actualidad, cuando un ciudadano presenta síntomas compatibles con la enfermedad, debe de llamar al centro de salud al que esté asignado e indicará cuales son los síntomas que presenta. El responsable Covid de cada centro de salud, será el encargado de tomar la decisión de si se le debe realizar las pruebas oportunas, en la mayoría de los casos se realizan. El centro de salud, concretará una cita médica con el paciente para realizarle las pruebas oportunas. <br> El paciente acudirá al centro médico el día de la cita y se le realizarán las pruebas necesarias, en la mayoría de los casos son una pueba PCR o una prueba de sangre, según el criterio del responsable médico. Después de esto, el paciente debe de dirigirse a su residencia y debe permanecer en cuarentena hasta conocer el resultado de las pruebas realizadas, que en general, no tardarán mas de 24-48 horas.|
=======
| **[Dependencias]** | En algunos casos depende del proceso de negocio 3, Rastreo de contacto con el positivo, sin embargo, en otros casos no hay ninguna dependencia cuando se registra un caso aislado. |
| **Descripción** | En la actualidad, cuando un ciudadano presenta síntomas compatibles con la enfermedad, debe de llamar al centro de salud al que esté asignado e indicará cuales son los síntomas que presenta. El responsable Covid de cada centro de salud, será el encargado de tomar la decisión de si se le debe realizar las pruebas oportunas, en la mayoría de los casos se realizan. El centro de salud concretará una cita médica con el paciente para realizarle las pruebas oportunas. <br> El paciente acudirá al centro médico el día de la cita y se le realizarán las pruebas necesarias, en la mayoría de los casos son una prueba PCR o una prueba de sangre, según el criterio del responsable médico. Después de esto, el paciente debe de dirigirse a su residencia y debe permanecer en cuarentena hasta el resultado de las pruebas realizadas, que en general, no tardarán más de 24-48 horas. |
>>>>>>> 7e1458613f795b44406b67ba50a1db5d7bf90743
=======
| **[Versión]** | 1.0 (17/11/2020) |
| **[Dependencias]** | En algunos casos depende del proceso de negocio 3, Rastreo de contacto con el positivo, sin embargo, en otros casos no hay ninguna dependencia cuando se registra un caso aislado. |
| **Descripción** | En la actualidad, cuando un ciudadano presenta síntomas compatibles con la enfermedad, debe de llamar al centro de salud al que esté asignado e indicará cuales son los síntomas que presenta. El responsable Covid de cada centro de salud, será el encargado de tomar la decisión de si se le debe realizar las pruebas oportunas, en la mayoría de los casos se realizan. El centro de salud concretará una cita médica con el paciente para realizarle las pruebas oportunas. <br> El paciente acudirá al centro médico el día de la cita y se le realizarán las pruebas necesarias, en la mayoría de los casos son una prueba PCR o una prueba de sangre, según el criterio del responsable médico. Después de esto, el paciente debe de dirigirse a su residencia y debe permanecer en cuarentena hasta el resultado de las pruebas realizadas, que en general, no tardarán más de 24-48 horas. |
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef
| **[Importancia]** | Alta |
| **[Actores]** | * Ciudadano <br> * Ambulatorio |
| **Comentarios** | El medio de comunicación en todo momento son las llamadas telefónicas.|

<p align="center"> <b>Tabla 4.1: Procesos de Negocio actuales.</b> <br> </p>

| **\<id>002** | Registrar resultado prueba PCR |
| -- | -- |
<<<<<<< HEAD
| **[Versión]** | 1.0(17/11/2020) |
<<<<<<< HEAD
| **[Dependencias]** | Este proceso de negocio depende del proceso 1 hacerse prueba PCR, dado que si no se ha realizado previamente una prueba PCR el paciente, no se puede tener una base en la que basarse para actuar de una forma u otra. |
| **Descripción** | Una vez que el paciente se ha realizado las pruebas oportunas, y se encuentra confinado en su casa, el ambulatorio le llamará para informarle del resultado de las pruebas lo antes posible y en cuanto se conozca el resultado de estas. Además, el ambulatorio se encargará de registrar en su base de datos el resultado de dicha prueba, para que así esta información sea procesada por parte de los responsables sanitarios y se puedan obtener las estadísticas oportunas. <br> Dependiendo del resultado de dicha prueba, se tomarán distintas medidas, si el resultado es positivo, el paciente deberá permanecer aislado y no podrá salir de casa, si convive con mas personas, dichas personas serán detectadas como contacto directo (ver proceso de negocio 3 Rastreo de contacto con positivo) y se les realizarán las pruebas oportunas, si son negativas o hasta que se conozca el resultado de dichas pruebas deberá permanecer aislado en su habitación y no podrá salir de esta a no ser que sea necesario (y con mascarilla siempre). Si el resultado es negativo pero al paciente se le considera contacto directo con un positivo confirmado, deberá permanecer en cuarentena durante 10 días. Si el paciente es negativo,y no es un contacto directo con un caso positivo confirmado, podrá hacer vida normal a no ser que los síntomas persistan que se le repetirá las pruebas por si es un caso de falso negativo.|
| **[Importancia]** | Alta |
=======
=======
| **[Versión]** | 1.0 (17/11/2020) |
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef
| **[Dependencias]** | Este proceso de negocio depende del proceso 1 hacerse prueba PCR, dado que, si no se ha realizado previamente una prueba PCR el paciente, no se puede tener una base en la que basarse para actuar de una forma u otra. |
| **Descripción** | Una vez que el paciente se ha realizado las pruebas oportunas, y se encuentra confinado en su casa, el ambulatorio le llamará para informarle del resultado de las pruebas lo antes posible y en cuanto se conozca el resultado de estas. Además, el ambulatorio se encargará de registrar en su base de datos el resultado de dicha prueba, para que así esta información sea procesada por parte de los responsables sanitarios y se puedan obtener las estadísticas oportunas. <br> Dependiendo del resultado de dicha prueba, se tomarán distintas medidas, si el resultado es positivo, el paciente deberá permanecer aislado y no podrá salir de casa, si convive con más personas, dichas personas serán detectadas como contacto directo (ver proceso de negocio 3 Rastreo de contacto con positivo) y se les realizarán las pruebas oportunas, si son negativas o hasta que se conozca el resultado de dichas pruebas deberá permanecer aislado en su habitación y no podrá salir de esta a no ser que sea necesario (y con mascarilla siempre). Si el resultado es negativo, pero al paciente se le considera contacto directo con un positivo confirmado, deberá permanecer en cuarentena durante 10 días. Si el paciente es negativo, y no es un contacto directo con un caso positivo confirmado, podrá hacer vida normal a no ser que los síntomas persistan que se le repetirá las pruebas por si es un caso de falso negativo. |
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
>>>>>>> 7e1458613f795b44406b67ba50a1db5d7bf90743
| **[Actores]** | * Ambulatorio> <br> * Ciudadano |
| **Comentarios** | La comunicación se realiza por medio de llamadas telefónicas. Se tienen en cuenta numerosos factores para decidir cúal es la forma de actuar en cada caso. |

<p align="center"> <b>Tabla 4.2: Procesos de Negocio actuales.</b> <br>  </p>

| **\<id>003** | Rastreo por contacto con positivo |
| -- | -- |
<<<<<<< HEAD
| **[Versión]** | 1.0(19/11/2020) |
<<<<<<< HEAD
| **[Dependencias]** | Este porceso de negocio depende totalmente del proceso 2, "Registrar resultado de la prueba PCR", ya que unicamente entra en juego con un resultado positivo de la prueba realizada al ciudadano. |
| **Descripción** | A día de hoy en la llamada que se realiza con el usuario susceptible de ser positivo se le solicitan a este los nombres de todas aquellas personas con las que ha mantenido contacto directo a lo largo de las úlitmas horas, normalmente las 48 horas previas a la manifestación de síntomas. En  caso de confirmarse el positivo del usuario los sanitarios y/o las autoridades proceden a contactar con aquellos cuidadanos que el positivo suministró en un primer momento para poder realizarles las pruebas pertinentes a cada uno de ellos y volver a comenzar con el proceso.|
| **[Importancia]** | Alta|
| **[Actores]** | * Ambulatorio <br> * Cuidadano <br> * Autoridades |
| **Comentarios** | Actualmente tenemos que confiar en que el usuario nos proporcione todos los contactos que ha tenido en las horas previas. En este sentido tenemos el handicap de que el usuario puede no recordarlos todos y/o no querer proporcionarlos todos por conveniencia.|
=======
=======
| **[Versión]** | 1.0 (19/11/2020) |
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef
| **[Dependencias]** | Este proceso de negocio depende totalmente del proceso 2, "Registrar resultado de la prueba PCR", ya que únicamente entra en juego con un resultado positivo de la prueba realizada al ciudadano. |
| **Descripción** | Hoy en día en la llamada que se realiza con el usuario susceptible de ser positivo se le solicitan a este los nombres de todas aquellas personas con las que ha mantenido contacto directo a lo largo de las últimas horas, normalmente las 48 horas previas a la manifestación de síntomas. En caso de confirmarse el positivo del usuario los sanitarios y/o las autoridades proceden a contactar con aquellos ciudadanos que el positivo suministró en un primer momento para poder realizarles las pruebas pertinentes a cada uno de ellos y volver a comenzar con el proceso. |
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Actores]** | * Ambulatorio <br> * Ciudadano <br> * Autoridades |
| **Comentarios** | Actualmente tenemos que confiar en que el usuario nos proporcione todos los contactos que ha tenido en las horas previas. En este sentido tenemos el hándicap de que el usuario puede no recordarlos todos y/o no querer proporcionarlos todos por conveniencia. |
<<<<<<< HEAD
>>>>>>> 7e1458613f795b44406b67ba50a1db5d7bf90743
=======
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef

<p align="center"> <b>Tabla 4.3: Procesos de Negocio actuales.</b> <br> </p>


| **\<id>004** | Llevar seguimiento del paciente y control de su cuarentena |
| -- | -- |
<<<<<<< HEAD
| **[Versión]** | 1.1(19/11/2020) |
<<<<<<< HEAD
| **[Dependencias]** | Este porceso de negocio depende totalmente del proceso 2, "Registrar resultado de la prueba PCR", ya que unicamente entra en juego con un resultado positivo de la prueba realizada al ciudadano. |
| **Descripción** | Actualmente una vez se detecta un positivo, este queda automaticamente puesto en cuarentena de 10 a 15 días dependiendo del caso. Para poder llevar a cabo un seguimiento de esta cuarentena los sanitarios y/o las autoridades realizan llamadas con frecuencia al paciente. Con esta llamada se pretede controlar que el usuario está cumpliendo las restricciones impuestas así como llevar a cabo un seguimiento sobre su estado de salud|
| **[Importancia]** | Media |
| **[Actores]** | * Ambulatorio <br> * Cuidadano <br> * Autoridades |
| **Comentarios** | Este proceso de negocio finalizaría una vez termine esta cuarentena, dando por hecho que, pasado el tiempo estimado, el paciente estará sano y no puede contagiar|
=======
=======
| **[Versión]** | 1.1 (19/11/2020) |
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef
| **[Dependencias]** | Este proceso de negocio depende totalmente del proceso 2, "Registrar resultado de la prueba PCR", ya que unicamente entra en juego con un resultado positivo de la prueba realizada al ciudadano. |
| **Descripción** | Actualmente una vez se detecta un positivo, este queda automáticamente puesto en cuarentena de 10 a 15 días dependiendo del caso. Para poder llevar a cabo un seguimiento de esta cuarentena los sanitarios y/o las autoridades realizan llamadas con frecuencia al paciente. Con esta llamada se pretende controlar que el usuario está cumpliendo las restricciones impuestas así como llevar a cabo un seguimiento sobre su estado de salud. |
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Actores]** | * Ambulatorio <br> * Ciudadano <br> * Autoridades |
| **Comentarios** | Este proceso de negocio finalizaría una vez termine esta cuarentena, dando por hecho que, pasado el tiempo estimado, el paciente estará sano y no puede contagiar. |
<<<<<<< HEAD
>>>>>>> 7e1458613f795b44406b67ba50a1db5d7bf90743
=======
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef

<p align="center"> <b>Tabla 4.4: Procesos de Negocio actuales.</b> <br>  </p>


| **\<id>005** | Interpretación de los datos |
| -- | -- |
<<<<<<< HEAD
| **[Versión]** | 1.0(17/11/2020) |
=======
| **[Versión]** | 1.0 (17/11/2020) |
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef
| **[Dependencias]** | Dicho proceso de negocio depende sobre todo del proceso 2 registrar casos positivos (para conocer los positivos que hay en cada centro de salud) y del proceso 3 Rastreo por contacto con positivo (para conocer de donde provienen dichos contagios). |
| **Descripción** | Una vez que los casos positivos han sido registrados en las bases de datos de los ambulatorios, estos pueden proporcionar dicha información al gobierno, para que estos tomen las medidas oportunas en función de estos datos proporcionados y las estadísticas obtenidas. |
| **[Importancia]** | Alta |
| **[Actores]** | * Gobierno <br> * Ambulatorios |
| **Comentarios** | El gobierno debe de pedir los datos sanitarios a los ambulatorios "en crudo" y por medio de los expertos del gobierno se realizarán las estadísticas oportunas con la escasa información que se dispone de cada caso, para posteriormente tomar decisiones. Pero los ambulatorios no disponen de dicha información de forma directa. |

<p align="center"> <b>Tabla 4.5: Procesos de Negocio actuales.</b> <br> </p>

### 3.3 Entorno Tecnológico Actual
<<<<<<< HEAD
<<<<<<< HEAD
Pandemio surge como necesidad de mejorar diferentes aspectos negativos encontrados en la ya existente aplicación Radar Covid, aparte de introducir nueva funcionalidad para poder gestionar los datos acerca de la pandemia. Además a parte de esta aplicación en la actualidad se encuentran otras con una funcionalidad parecida, como se comentrá en el apartado 3.3.2, entorno software actual.
=======
Pandemio surge como necesidad de mejorar diferentes aspectos negativos encontrados en la ya existente aplicación Radar Covid, aparte de introducir nueva funcionalidad para poder gestionar los datos acerca de la pandemia. Además, a parte de esta aplicación en la actualidad se encuentran otras con una funcionalidad parecida, como se ha comentado en el apartado 3.0.
>>>>>>> 7e1458613f795b44406b67ba50a1db5d7bf90743
=======
Pandemio surge como necesidad de mejorar diferentes aspectos negativos encontrados en la ya existente aplicación Radar Covid, aparte de introducir nueva funcionalidad para poder gestionar los datos acerca de la pandemia. Además, a parte de esta aplicación en la actualidad se encuentran otras con una funcionalidad parecida, como se ha comentado en el apartado 3.0.
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef

Dado que, en la actualidad, la sociedad está muy concienciada con las nuevas tecnologías y cada vez está más acostumbrada al uso de la tecnología en su vida diaria, hace que sea interesante aprovechar este entorno tecnológico en el que vivimos para poder obtener datos e información acerca de la pandemia.

#### 3.3.1 Descripción del Entorno de Hardware Actual
Hoy en día, cerca del 90% de la población española dispone de un teléfono móvil y en la mayoría de los casos se tratan de smartphones. Aprovechando de que la mayoría de la población dispone de tal dispositivo y lo lleva siempre consigo, podemos beneficiarnos de toda la información que se está compartiendo por la red mientras estamos conectados o disponemos de cobertura o señal GPS.

Por otra parte, hoy en día disponemos de unas buenas infraestructuras de redes de comunicación en la que se pueden sustentar todo este intercambio de información constante.

Dado que Pandemio va a gestionar también información y datos médicos relativos a los pacientes que se deben realizar las pruebas oportunas en los ambulatorios en los que estén asignados, se necesita disponer de tal información la cual se encuentra en las bases de datos y servidores del sistema sanitario de cada comunidad autónoma. Por lo que resulta conveniente que se pueda acceder a tal información de dichas bases de datos por medio de nuestra plataforma Pandemio.

#### 3.3.2 Descripción del Entorno Software Actual
A día de hoy y como consecuencia de la relevancia a nivel mundial y de la alteración de la normalidad que ha supuesto la pandemia del COVID-19 se han implementado numerosas aplicaciones en torno a la resolución de este problema o simplemente para poder obtener un mejor conocimiento sobre sus efectos en la población de cara a tomar medidas que nos puedan ayudar a revertir poco a poco esta situación. Observando el estado del arte en este campo podemos orientar mejor nuestro trabajo. Tomaremos como referencia algunas aplicaciones, además de _Radar Covid_ en este ámbito que creemos que nos pueden ayudar en nuestro proyecto:

__CoronaMadrid:__ La aplicación permite a sus usuarios poder detectar, informarse y contactar con las autoridades en cualquier fase de la concepción de la enfermedad COVID-19. CoronaMadrid tiene la misión de ayudar a los ciudadanos a poder detectar si están siendo afectados por la enfermedad y obtener las mejores recomendaciones dependiendo de su estado. En caso de estado grave las autoridades serán conocedoras de la situación y podrán comunicarse directamente con el afectado.

De _CoronaMadrid_ nos resulta interesante la capacidad del usuario para informarse y poner en conocimiento de las autoridades su estado.

__COVID-19.eus:__ Es una aplicación colaborativa en el ámbito de la comunidad autónoma vasca. La aplicación permite hacer un autodiagnóstico del contagio de COVID-19. En caso de ser positivo, el usuario se considerará _POSIBLE contagio_ (según terminología de la OMS) y avisará a todo el círculo de personas, de tal forma que se considerarán en riesgo. Junto a esta información el sistema registrará ese dato, de tal forma que se puede seguir un rastro de contagios con esta funcionalidad de círculos. Junto con esta información, se pide el Código Postal, y en caso de infección comunitaria, se podrían también detectar focos de contagio.

Con respecto a _COVID-19.eus_ creemos que puede ser útil la manera de prevenir la extensión de los contagios por medio del aviso al círculo de personas cercanas a un positivo y la relativa capacidad de detectar focos de contagio.

__STOP COVID19 CAT:__ Es una aplicación móvil de salud con un doble objetivo: Dar respuesta a las necesidades de información de la ciudadanía en relación al Covid 19, a través de un cuestionario que les indica si tienen posibilidad de tener Covid. Recoger datos de la población para poder crear estadísticas.

De _STOP COVID19 CAT_ nos parece buena idea el uso de los datos de la población para llevar a cabo estadísticas de las cuales obtener conclusiones a utilizar.

<<<<<<< HEAD
<<<<<<< HEAD
De Radar Covid, ya se ha comentado en secciones previas de este documento, como surge la necesidad de desarrollar esta nueva plataforma Pandemio, ante los errores detectados en la anterior aplicación del ministerio. Los cuales son el uso de bluetooth y que su uso no es obligatorio por parte de los usuarios. Sin embargo, resulta interesante la idea de como rastrear los contagios entre los ciudadanos, por lo que usaremos esta idea como base en nuestra plataforma Pandemio, pero realizando las modificaciones oportunas en su implementación para mitigar los problemas de implementación encontrados en Radar Covid.
=======
De Radar Covid, ya se ha comentado en secciones previas de este documento, como surge la necesidad de desarrollar esta nueva plataforma Pandemio, ante los errores detectados en la anterior aplicación del ministerio. Los cuales son el uso de bluetooth y que su uso no es obligatorio por parte de los usuarios. Sin embargo, resulta interesante la idea de cómo rastrear los contagios entre los ciudadanos, por lo que usaremos esta idea como base en nuestra plataforma Pandemio, pero realizando las modificaciones de oportunas en su implementación para mitigar los problemas de implementación encontrados en Radar Covid.
>>>>>>> 7e1458613f795b44406b67ba50a1db5d7bf90743
=======
De Radar Covid, ya se ha comentado en secciones previas de este documento, como surge la necesidad de desarrollar esta nueva plataforma Pandemio, ante los errores detectados en la anterior aplicación del ministerio. Los cuales son el uso de bluetooth y que su uso no es obligatorio por parte de los usuarios. Sin embargo, resulta interesante la idea de cómo rastrear los contagios entre los ciudadanos, por lo que usaremos esta idea como base en nuestra plataforma Pandemio, pero realizando las modificaciones de oportunas en su implementación para mitigar los problemas de implementación encontrados en Radar Covid.
>>>>>>> 7f7310ef154dc7968726921b7d57cd833f8eadef

