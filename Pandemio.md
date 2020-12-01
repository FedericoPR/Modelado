# PANDEMIO

## 1. INTRODUCCIÓN
Ante los resultados decepcionantes obtenidos con la aplicación **Radar Covid** para llevar a cabo el rastreo de los contagios entre los ciudadanos durante la pandemia, el Ministro de Sanidad ha propuesto desarrollar una plataforma que permita rastrear los casos Covid, así como gestionar los datos de los ciudadanos que sean positivos.

Con esta nueva plataforma que se propone desarrollar, se desea mitigar aquellos problemas que se han encontrado en la ya existente aplicación **Radar Covid**. Entre los cuales el comité de expertos resalta que son debidos a que la instalación y el uso de la aplicación NO eran obligatorios, por lo que pocos usuarios la instalaron y además dicha aplicación al basarse en el uso de bluetooth, la aplicación era inservible si el bluetooth estaba apagado o bien estaba ocupado.

Además, se propone que la nueva plataforma a desarrollar pueda llevar a cabo un seguimiento de aquellos ciudadanos que deben cumplir la cuarentena y no la cumplían, así como aquellos que no acudían a hacerse las pruebas médicas oportunas. Donde resulta importante que se cumpla la ley de datos y los datos de los ciudadanos solo sean usados por las personas autorizadas y sean anonimizados cuando sea posible.

Uno de los aspectos importantes que motiva el desarollo de la plataforma PANDEMIO, es que en la actual pandemia que nos encontramos hay personas que son positivos y que no presentan síntomas, los llamados casos asintomáticos. Dichos casos, son personas que contagian la enfermedad, pero es muy difícil detectar que son contagiadoras, dado que no presentan ningún síntoma que pueda hacer sospechar que están infectados. Por lo cual, se persigue que con la plataforma PANDEMIO, se pueda llevar un control mas preciso de los contactos para poder conocer si alguno de los contactos directos con los positivos puede ser un caso aintomático.

### 1.1 Alcance
Con el desarrollo de la plataforma PANDEMIO, se busca conseguir un sistema de control e información acerca de los contagios que se dan en una pandemia, en este caso de Covid-19, pero también nos servirá para otras pandemias que se pudieran presentar en un futuro.

Pandemio proporcionará distintos datos acerca de los contagios de los ciudadanos al ministerio de Sanidad, para que dichos datos sean procesados y se tomen las medidas oportunas por parte del juicio de expertos correspondiente. También, se proporcionarán los datos necesarios acerca de los contagios a los ambulatorios, así como a las autoridades correspondientes para que puedan llevar a cabo un control de que los casos positivos cumplen la cuarentena obligatoria cuando sea necesario.
El alcance del proyecto se centra en tres grandes características, el rastreo de los contactos con los casos positivos, gestionar la realización de las pruebas médicas y gestionar el cumplimiento de la cuarentena. Dentro de cada una de estas características se incluirá diferente funcionalidad, a continuación, se muestra un diagrama de característica que plasma cual es el alcance del proyecto de una forma más precisa.

![picture 1](images/0002456fa2638cf889623d3a73b555753c8edcd47c789245ce2fe16a3b0e85e8.png)  

### 1.2 Objetivos
Entre los objetivos que se desean alcanzar al desarrollar dicha plataforma se encuentran:

- Llevar a cabo un rastreo de los casos positivos entre los ciudadanos, así como conocer las personas que hayan estado en contacto con un positivo (durante un tiempo superior a 15 minutos)
- LLevar a cabo un control del correcto cumplimiento de la cuarentena por aquellos ciudadanos que la deban cumplir, notificando a la autoridad cuando se deja de cumplir la cuarentena.
- LLevar a cabo un control de aquellos ciudadanos que deben presentarse a las pruebas médicas oportunas, así como el resultado de estas.
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

Después, se llevará a cabo un seguimiento de todas aquellas personas que hayan estado en contacto (durante un tiempo superior a 15 minutos) con el paciente positivo en las 48 horas anteriores a la realización de la prueba PCR, a las cuales se les considerará contacto directo. Los contactos directos deben permanecer en cuarentena hasta que se conozca el resultado de la prueba PCR, si esta es negativa en algunos casos se debe mantener la cuarentena unos días más (depende del tipo de contacto, tiempo, si ha sido con mascarilla o sin ella, etc.) en caso de que lo indique el responsable sanitario. Si la prueba es positiva, se repetirá el mismo proceso con los contactos directos del nuevo caso positivo.

### 2.2 Glosario de términos
- **Asintomático:** Aquella persona que padece una enfermedad pero no presenta síntomas de ella.
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

Puesto que la situación de la pandemia actual es una situación crítica se nos proporcionarán ciertos privilegios y facilidades proporcionándonos legalidad para ciertos asuntos que ahora mismo suponen un problema.

De toda esta situación podemos resumir las siguientes fortalezas en cuanto a nuestra situación actual:

| **\<id>001** | Reciente pandemia del COVID-19 |
| -- | -- |
| **[Versión]** | 1.0 (17/11/2020) |
| **Descripción** | Dado que actualmente existe la pandemia del Covid-19, hemos adquirido la suficiente experiencia de cómo se debe actuar ante una pandemia y cúales deben ser las medidad a tomar. Es decir, tendremos un conocimiento previo y un conjunto de técnicas que se podrán aplicar de cara a controlar la pandemia y no actuaremos desde cero. |
| **Comentarios** | En la actualidad se conocen los protocolos de actuación ante una pandemia, la sociedad conoce el cómo actuar y dispone de una experiencia previa de ello. Además, se dispone de datos previos y estudios acerca de la eficacia de las diferentes mediadas tomadas en la actual pandemia. |
  
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
| **Comentarios** | El pequeño porcentaje de la población que no dispone de teléfono móvil se suele corresponder con niños o personas de edad avanzada, las cuales es más fácil de rastrear sus contagios y si cumplen la cuarentena obligatoria, para ello hará falta de la actuación de los agentes de la autoridad o personas asignadas para ello. |
  
<p align="center"> <b>Tabla 1.6: Fortalezas de la situación actual.</b> </p>
  
| **\<id>007** | Comunicación con las fuerzas del orden y los sanitarios |
| -- | -- |
| **[Versión]** | 1.0 (18/11/2020) |
| **Descripción** | Para poder llevar a cabo un control eficiente de las personas que deben realizarse las pruebas enviaremos a los ambulatorios los listados de personas que deben hacerse las pruebas, y estos podrán notificar a la autoridad el incumplimiento. Por su parte las fuerzas del orden podrán comprobar el cumplimiento de las cuarentenas y las obligaciones impuestas a los ciudadanos. |
| **Comentarios** | Nuestra labor será la de recabar información que proporcionaremos a los ambulatorios y a sanidad para que puedan llevar a cabo las acciones pertinentes, pero el hecho de que estemos en comunicación directa con organismos con tanto "poder" debería influir positivamente en el éxito de nuestro proyecto. |
  
<p align="center"> <b>Tabla 1.7: Fortalezas de la situación actual.</b> </p>

#### 3.1.2 Debilidades de la situación Actual
Debido a la complejidad de la situación actual y a que la aplicación __Radar Covid__ ha ofrecido muchos puntos en contra pero pocos a favor nos encontramos en una posición donde todo aquello que queramos implementar puede ser muy buena idea sobre el papel pero causar muchas dificultades en un contexto real.

Por otro lado, para poder llevar a cabo ciertas operaciones vamos a necesitar del uso de los datos de localización de los móviles y eso, por el momento supone un problema. Aun así, cuando esto esté solucionado deberemos lidiar con el cumplimiento de la ley de protección de datos.

De toda esta situación podemos resumir las siguientes debilidades en cuanto a nuestra situación actual:

| **\<id>001** | Problemas en el uso de Bluetooth |
| -- | -- |
| **[Versión]** | 1.0 (18/11/2020) |
| **Descripción** | La aplicación Radar Covid intentó realizar la localización de los usuarios y sus interacciones por medio del bluetooth sin embargo resultó ser inservible si este estaba apagado o siendo usado por otro accesorio.|
| **Comentarios** | Supone una debilidad el hecho de que la "primera opción" para localizar a los usuarios haya fracasado y por tanto tendremos que buscar otra opción mejor.| 
<p align="center"> <b>Tabla 2.1: Debilidades de la situación actual.</b> </p>
  
| **\<id>002** | Opcionalidad de los usuarios para estar controlados |
| -- | -- |
| **[Versión]** | 1.0 (18/11/2020) |
| **Descripción** | La obtención de Radar Covid por parte del usuario era totalmente voluntaria, lo que supone un gran problema ya que el usuario que lo deseara podría ser "invisible" desde el punto de vista de la aplicación. |
| **Comentarios** | Para poder paliar la debilidad de que los usuarios decidan no tener la aplicación nosotros contamos con los datos de las operadoras sobre los registros de localización de los usuarios con lo que el usuario estará "monitorizado" sin saberlo (ver Tabla 1.4). | 
  
<p align="center"> <b>Tabla 2.2: Debilidades de la situación actual.</b> </p>
  
| **\<id>003** | Irresponsabilidad de los usuarios en el cumplimiento de las recomendaciones |
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

| **\<id>005** | Gran volumen de datos a gestionar y algaritmos complejos|
| -- | -- |
| **[Versión]** |  1.0 (26/11/2020) |
| **Descripción** | Debido a los númerosos datos que se deben de gestionar de los usuarios, tales como el historial de localizaciones, el resultado de sus pruebas médicas o los datos personales de este, se deben de manejar grandes volúmenes de información por lo que se necesitará disponer de grandes computadoras, grandes servidores o bases de datos, por lo que la implementación de esta plataforma no está al alcance de cualquiera, se necesita el uso de estos grandes computadores.<br> Además, dado esta gran cantidad de datos, se deberá disponer de algoritmos bastante complejos para poder obtener distinta información acerca de ellos y estos deben de ser eficientes.  |
| **Comentarios** | Para solventar esta debilidad deberemos de disponer o contratar los servicios de grandes computadoras como mare nostrum. | 
  
<p align="center"> <b>Tabla 2.5: Debilidades de la situación actual.</b> </p>

| **\<id>006** | Personas asintomaticas |
| -- | -- |
| **[Versión]** |  1.0 (26/11/2020) |
| **Descripción** | En la actualidad, la enfermedad de la pandemia, hace que haya personas asintomáticas, es decir personas infectadas pero que no presentan síntomas, dichas personas pueden contagiar al resto de ciudadanos y no se sabe que están contagiando al resto. Lo cual, esto ayuda a que se propague el virus entre la población y se pueda desbordar la pandemia y los infectados. |
| **Comentarios** | Para solventar esta debilidad deberemos de rastrear cuales han sido los contactos directos con los positivos para así poder realizarles las pruebas médicas oportunas.| 
  
<p align="center"> <b>Tabla 2.6: Debilidades de la situación actual.</b> </p>

### 3.2 Modelos de Procesos de Negocios Actuales
En este apartado representaremos y describiremos todos aquellos procesos que se llevarán a cabo para gestionar los contagios que se producen en la pandemia, así como los procesos que se emplearán para controlar el cumplimiento de la cuarentena obligatoria por parte de los ciudadanos positivos. También se tendrán en cuenta todos aquellos procesos en los que se gestionen las distintas pruebas médicas que se deben realizar los ciudadanos, asi como informales a estos de los resultados. Por otro lado, se especificará como debe ser la comunicación con el resto de los actores que intervienen en la plataforma como los agentes de la autoridad o el gobierno al que se le proporcionarán todos los datos obtenidos con la plataforma para que puedan tomarse las medidas oportunas por parte de los expertos correspondientes.

#### 3.2.1 Descripción de los Actores de Negocio Actuales
Los actores de negocio actuales son todas aquellas personas o entidades que están involucradas en la gestión de la pandemia actual y en los procesos de negocio llevados a cabo. Dichos actores se corresponden con: ciudadanos, gobierno, autoridades y ambulatorios. Necesarios para que la información se transmita de manera segura.

| **\<id>001** | Ciudadano |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | El ciudadano es la piedra angular del proceso y por ello la mayoría de los procesos de negocio actuales dependen de él. El proceso 1, "Hacer prueba PCR", depende directamente del ciudadano ya que es objeto de dicha prueba. Por el mismo motivo también depende el proceso 2, "Registrar resultado de la prueba". El proceso 3, "Rastreo por contacto con un positivo", depende también de este actor ya que un resultado positivo en un ciudadano recae en la realización de pruebas en otros ciudadanos. Por último el proceso control de la cuarentena y seguimiento del estado del paciente, proceso 4, depende del ciudadano por razones obvias. |
| **Descripción** | Este actor de negocio actual es el actor principal en torno al que gira todo el sistema. Representa a cada uno de los ciudadanos. De este actor se obtiene la información de su localización por medio de la tecnología bluetooth de su móvil para que si se produce un positivo poder alertar a aquellas personas que hayan tenido contacto. La llamada de un ciudadano por padecer síntomas y la realización de una PCR es lo que dispara los diferentes procesos de negocio, ya que si se produce un positivo este debe guardar una cuarentena sobre la que se realiza un seguimiento además de iniciarse un rastreo de los posibles ciudadanos que también puedan haber sido contagiados. La información sobre los resultados de las pruebas y sobre el seguimiento del ciudadano positivo se pone en conocimiento de los rastreadores que llevan a cabo las acciones pertinentes. |
| **Comentarios** | De la información obtenida por medio de los ciudadanos positivos, como la residencia, los puntos de visita frecuentes o las personas con las que ha mantenido contacto se sacan conclusiones por medio de su análisis que puedan dar lugar a toma de decisiones. |

<p align="center"> <b>Tabla 3.1: Actores de negocio.</b> </p>

| **\<id>002** | Gobierno |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | De este actor depende el proceso de negocio 5, "Toma de decisiones", ya que es el encargado de tomar las medidas o imponer las restricciones en función del análisis de la información disponible. |
| **Descripción** | Este actor de negocio actual representa al gobierno, en concreto al ministro de sanidad, al que se le suministrarán todos los datos y estadísticas que se han obtenido por medio del procesamiento de los datos capturados de los ciudadanos y procesados. Dicho actor se encargará como entidad de tomar las decisiones oportunas en función de los datos suministrados por la plataforma, en base a diferentes criterios. |
| **Comentarios** | Es un actor que se encuentra "aislado" del proceso de detección y seguimiento de positivos pero que será muy importante debido a su capacidad de toma de decisiones. Este actor puede imponer medidas nuevas, protocolos diferentes y alterar de manera importante todos los procesos tal y como se llevan a cabo hasta ahora. Es por ello que, aunque se encuentre fuera del flujo normal es importantísimo incluirlo por su capacidad de cambiar el mismo. |

<p align="center"> <b>Tabla 3.2: Actores de negocio.</b> </p>

| **\<id>003** | Autoridades |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | Dicho actor participa en los procesos de negocio 3 Rastreo por contacto con positivo y en el proceso 4 llevar seguimiento del paciente y control de su cuarentena. |
| **Descripción** | Este actor de negocio actual representa a las fuerzas del orden (policía local, nacional, guardia civil y el ejército) que se encargan de rastrear cuales han sido los contactos directos con los positivos y proveer dicha información a los ambulatorios para que sean los encargados de llamar a dichos contactos directos para que se les realicen las pruebas médicas oportunas. También son los encargados de controlar el cumplimiento de las cuarentenas obligatorias por parte de los ciudadanos que deban de cumplirlas, para ello se encargan de hacer llamadas telefónicas o videollamadas con los pacientes positivos para comprobar que se encuentran en casa cumpliendo la cuarentena. |
| **Comentarios** | A este actor en determinadas ocasiones se les llama rastreadores, y llevaran a cabo la misión de rastrear el cómo se producen los contagios entre los positivos, asi como obtener cuales son los brotes de dichos contagios, para ello tan solo disponen de la información proporcionada por los pacientes positivos. |
<p align="center"> <b>Tabla 3.3: Actores de negocio.</b> </p>

| **\<id>004** | Ambulatorio |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | Este actor entra en juego en la mayoría de los procesos de negocio, dado que es el conocedor de cómo se debe gestionar la pandemia y se encarga de mediar en cómo se debe actuar en los distintos casos. Los procesos de negocio en los que participa son 1 Hacer prueba PCR, 2 Registrar resultado de la prueba PCR, 3 rastreo por contacto con positivo, 4 llevar seguimiento del paciente y control de su cuarentena y 5 interpretación de los datos. |
| **Descripción** | Este actor de negocio actual representa al centro de salud, asi como los responsables médicos, se encargan de determinar si se les debe de realizar las pruebas a los pacientes ante la aparición de síntomas o por contacto directo, también se encargan de concretar las citas para la realización de las pruebas médicas con los pacientes, así como informarles de los resultados obtenidos en dichas pruebas y en caso de ser positivos solicitan los datos de los contactos directos. <br> Por otra parte, se encargan de registrar los resultados de dichas pruebas en la base de datos del centro de salud, para que posteriormente pueda ser proporcionada esta información al gobierno. También se encargan de realizar un seguimiento de la evolución del estado del paciente durante la cuarentena por medio de las llamadas telefónicas. |
| **Comentarios** | Dicho actor en determinadas ocasiones se les llama responsable Covid y es el encargado de realizar todas las acciones anteriormente comentadas respecto a la gestión de los casos covid en cada uno de los ambulatorios. |

<p align="center"> <b>Tabla 3.4: Actores de negocio.</b> <br> </p>

#### 3.2.2 Descripción de Procesos de Negocio Actuales
En este apartado se comentarán cúales son los procesos de negocio que se llevan a cabo en la actualidad para gestionar la pandemia. Dichos procesos son en los que se basará nuestra plataforma para agilizarlos y poder ser llevadas a cabo de una forma más automatizada. De forma general, se comentará cual es el flujo de procesos que se han de llevar a cabo cuando se detectan los síntomas compatibles con la enfermedad. Dichos procesos son los siguientes:

| **\<id>001** | Hacer prueba PCR |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | En algunos casos depende del proceso de negocio 3, Rastreo de contacto con el positivo, sin embargo, en otros casos no hay ninguna dependencia cuando se registra un caso aislado. |
| **Descripción** | En la actualidad, cuando un ciudadano presenta síntomas compatibles con la enfermedad, debe de llamar al centro de salud al que esté asignado e indicará cuales son los síntomas que presenta. El responsable Covid de cada centro de salud, será el encargado de tomar la decisión de si se le debe realizar las pruebas oportunas, en la mayoría de los casos se realizan. El centro de salud concretará una cita médica con el paciente para realizarle las pruebas oportunas. <br> El paciente acudirá al centro médico el día de la cita y se le realizarán las pruebas necesarias, en la mayoría de los casos son una prueba PCR o una prueba de sangre, según el criterio del responsable médico. Después de esto, el paciente debe de dirigirse a su residencia y debe permanecer en cuarentena hasta el resultado de las pruebas realizadas, que en general, no tardarán más de 24-48 horas. |
| **[Importancia]** | Alta |
| **[Actores]** | * Ciudadano <br> * Ambulatorio |
| **Comentarios** | El medio de comunicación en todo momento son las llamadas telefónicas.|

<p align="center"> <b>Tabla 4.1: Procesos de Negocio actuales.</b> <br> </p>

| **\<id>002** | Registrar resultado prueba PCR |
| -- | -- |
| **[Versión]** | 1.0 (17/11/2020) |
| **[Dependencias]** | Este proceso de negocio depende del proceso 1 hacerse prueba PCR, dado que si no se ha realizado previamente una prueba PCR el paciente, no se puede tener una base en la que basarse para actuar de una forma u otra. |
| **Descripción** | Una vez que el paciente se ha realizado las pruebas oportunas, y se encuentra confinado en su casa, el ambulatorio le llamará para informarle del resultado de las pruebas lo antes posible y en cuanto se conozca el resultado de estas. Además, el ambulatorio se encargará de registrar en su base de datos el resultado de dicha prueba, para que así esta información sea procesada por parte de los responsables sanitarios y se puedan obtener las estadísticas oportunas. <br> Dependiendo del resultado de dicha prueba, se tomarán distintas medidas, si el resultado es positivo, el paciente deberá permanecer aislado y no podrá salir de casa, si convive con mas personas, dichas personas serán detectadas como contacto directo (ver proceso de negocio 3 Rastreo de contacto con positivo) y se les realizarán las pruebas oportunas, si son negativas o hasta que se conozca el resultado de dichas pruebas deberá permanecer aislado en su habitación y no podrá salir de esta a no ser que sea necesario (y con mascarilla siempre). Si el resultado es negativo pero al paciente se le considera contacto directo con un positivo confirmado, deberá permanecer en cuarentena durante 10 días. Si el paciente es negativo,y no es un contacto directo con un caso positivo confirmado, podrá hacer vida normal a no ser que los síntomas persistan que se le repetirá las pruebas por si es un caso de falso negativo.|
| **[Importancia]** | Alta |
| **[Actores]** | * Ambulatorio> <br> * Ciudadano |
| **Comentarios** | La comunicación se realiza por medio de llamadas telefónicas. Se tienen en cuenta numerosos factores para decidir cúal es la forma de actuar en cada caso. |

<p align="center"> <b>Tabla 4.2: Procesos de Negocio actuales.</b> <br>  </p>

| **\<id>003** | Rastreo por contacto con positivo |
| -- | -- |
| **[Versión]** | 1.0 (19/11/2020) |
| **[Dependencias]** | Este porceso de negocio depende totalmente del proceso 2, "Registrar resultado de la prueba PCR", ya que unicamente entra en juego con un resultado positivo de la prueba realizada al ciudadano. |
| **Descripción** | A día de hoy en la llamada que se realiza con el usuario susceptible de ser positivo se le solicitan a este los nombres de todas aquellas personas con las que ha mantenido contacto directo a lo largo de las úlitmas horas, normalmente las 48 horas previas a la manifestación de síntomas. En  caso de confirmarse el positivo del usuario los sanitarios y/o las autoridades proceden a contactar con aquellos cuidadanos que el positivo suministró en un primer momento para poder realizarles las pruebas pertinentes a cada uno de ellos y volver a comenzar con el proceso.|
| **[Importancia]** | Alta|
| **[Actores]** | * Ambulatorio <br> * Cuidadano <br> * Autoridades |
| **Comentarios** | Actualmente tenemos que confiar en que el usuario nos proporcione todos los contactos que ha tenido en las horas previas. En este sentido tenemos el handicap de que el usuario puede no recordarlos todos y/o no querer proporcionarlos todos por conveniencia.|

<p align="center"> <b>Tabla 4.3: Procesos de Negocio actuales.</b> <br> </p>


| **\<id>004** | Llevar seguimiento del paciente y control de su cuarentena |
| -- | -- |
| **[Versión]** | 1.1 (19/11/2020) |
| **[Dependencias]** | Este porceso de negocio depende totalmente del proceso 2, "Registrar resultado de la prueba PCR", ya que unicamente entra en juego con un resultado positivo de la prueba realizada al ciudadano. |
| **Descripción** | Actualmente una vez se detecta un positivo, este queda automaticamente puesto en cuarentena de 10 a 15 días dependiendo del caso. Para poder llevar a cabo un seguimiento de esta cuarentena los sanitarios y/o las autoridades realizan llamadas con frecuencia al paciente. Con esta llamada se pretede controlar que el usuario está cumpliendo las restricciones impuestas así como llevar a cabo un seguimiento sobre su estado de salud|
| **[Importancia]** | Media |
| **[Actores]** | * Ambulatorio <br> * Cuidadano <br> * Autoridades |
| **Comentarios** | Este proceso de negocio finalizaría una vez termine esta cuarentena, dando por hecho que, pasado el tiempo estimado, el paciente estará sano y no puede contagiar|

<p align="center"> <b>Tabla 4.4: Procesos de Negocio actuales.</b> <br>  </p>


| **\<id>005** | Interpretación de los datos |
| -- | -- |
| **[Versión]** | 1.0(17/11/2020) |
| **[Dependencias]** | Dicho proceso de negocio depende sobre todo del proceso 2 registrar casos positivos (para conocer los positivos que hay en cada centro de salud) y del proceso 3 Rastreo por contacto con positivo (para conocer de donde provienen dichos contagios). |
| **Descripción** | Una vez que los casos positivos han sido registrados en las bases de datos de los ambulatorios, estos pueden proporcionar dicha información al gobierno, para que estos tomen las medidas oportunas en función de estos datos proporcionados y las estadísticas obtenidas. |
| **[Importancia]** | Alta |
| **[Actores]** | * Gobierno <br> * Ambulatorios |
| **Comentarios** | El gobierno debe de pedir los datos sanitarios a los ambulatorios "en crudo" y por medio de los expertos del gobierno se realizarán las estadísticas oportunas con la escasa información que se dispone de cada caso, para posteriormente tomar decisiones. Pero los ambulatorios no disponen de dicha información de forma directa. |

<p align="center"> <b>Tabla 4.5: Procesos de Negocio actuales.</b> <br> </p>

### 3.3 Entorno Tecnológico Actual

Pandemio surge como necesidad de mejorar diferentes aspectos negativos encontrados en la ya existente aplicación Radar Covid, aparte de introducir nueva funcionalidad para poder gestionar los datos acerca de la pandemia. Además, a parte de esta aplicación en la actualidad se encuentran otras con una funcionalidad parecida, como se ha comentado en el apartado 3.0.

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

De Radar Covid, ya se ha comentado en secciones previas de este documento, como surge la necesidad de desarrollar esta nueva plataforma Pandemio, ante los errores detectados en la anterior aplicación del ministerio. Los cuales son el uso de bluetooth y que su uso no es obligatorio por parte de los usuarios. Sin embargo, resulta interesante la idea de cómo rastrear los contagios entre los ciudadanos, por lo que usaremos esta idea como base en nuestra plataforma Pandemio, pero realizando las modificaciones de oportunas en su implementación para mitigar los problemas de implementación encontrados en Radar Covid.

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

### 4.2 Modelos de Procesos de Negocio a Implantar

En este apartado representaremos y describiremos todos aquellos procesos que se llevarán acabo en nuestra plataforma PANDEMIO para gestionar los contagios que se producen en la pandemia, asi como los procesos que se emplearán para controlar el cumplimiento de la cuarentena obligatoria por parte de los ciudadanos positivos. También se tendrán en cuenta todos aquellos procesos en los que se gestionen las distintas pruebas médicas que se deben realizar los ciudadanos, asi como informales a estos de los resultados.Por otro lado, se especificará como debe ser la comunicación con el resto de actores que intervienen en la plataforma como los agentes de la autoridad o el gobierno al que se le proporcionarán todos los datos obtenidos con la plataforma para que puedan tomarse las medidas oportunas por parte de los expertos correspondientes.

#### 4.2.1 Descripción de los Actores de Negocio a Implantar
Los actores de negocio de nuestra plataforma PANDEMIO, son todas aquellas personas, entidades u organizaciones que están involucrados en los procesos de negocio a implantar, en este caso los actores de negocio de nuestra plataforma son los siguientes: ciudadanos, gobierno, autoridades y ambulatorios.

| **\<id>001** | Ciudadano |
| -- | -- |
| **[Versión]** | 1.0(28/11/2020) |
| **[Dependencias]** | Dicho actor participa en los procesos de negocio a implantar:<br>* 001 Rastrear contactos con los casos positivos. <br> * 002 Gestionar la realización de las pruebas médicas. <br> * 003 Gestionar el cumplimiento de la cuarentena.|
| **Descripción** | Este actor de negocio actual es el actor principal de la plataforma y representa a cada uno de los ciudadanos, de dicho actor se van a obtener todos los datos que se gestionarán por medio de la plataforma. De ellos por medio de sus dispositivos móviles, se va a poder acceder a cual ha sido su localización, las personas con las que ha estado en contacto, el tiempo que ha permanecido en un determinado lugar, etc. Toda esta información será procesada por la plataforma pandemio para poder obtener la información "depurada" y poderla suministrar a los distintos actores interesados como el gobierno, las autoridades o los ambulatorios.|
| **Comentarios** | De dicho actor se van a obtener sus datos por medio de los datos suministrados por las compañias telefónicas. |

<p align="center"> <b>Tabla 6.1: Actores de negocio a implantar.</b>

| **\<id>002** | Gobierno |
| -- | -- |
| **[Versión]** | 1.0(28/11/2020) |
| **[Dependencias]** | Dicho actor participa en los procesos de negocio a implantar:<br>* 004 Suministrar información y estadísticas al gobierno.  |
| **Descripción** | Este actor de negocio actual representa al gobierno, en concreto al ministerio de sanidad y el comité de expertos, al que se le suministrarán todos los datos y estadísticas que se han obtenido por medio del procesamiento de los datos capturados de los ciudadanos y procesados por parte de nuestra plataforma pandemio. Dicho actor se encargará como entidad de tomar las decisiones oportunas en función de los datos suministrados por la plataforma, en base a diferentes criterios.
| **Comentarios** | El objetivo de nuestra plataforma es proporcionar los datos lo mejor procesados y "depurados" a este actor para que puedan tomar decisiones. |

<p align="center"> <b>Tabla 6.2: Actores de negocio a implantar.</b> 

| **\<id>003** | Autoridades |
| -- | -- |
| **[Versión]** | 1.0(28/11/2020) |
| **[Dependencias]** | Dicho actor participa en los procesos de negocio a implantar:<br>* 002 Gestionar la realización de las pruebas médicas. <br> * 003 Gestionar el cumplimiento de la cuarentena. |
| **Descripción** | Este actor de negocio actual representa a las fuerzas del orden (policía local, nacional, guardia civil y el ejército) que deberán de ser informados del cumplimiento de la cuarentena y poder verificar que se está cumpliendo esta. Dicho actor podrá acceder a la información de los ciudadanos que estén en cuarentena para poder controlar que se cumplen dichas cuarentenas así como intervenir en el caso de que dejen de cumplirse o no se realicen las pruebas médicas oportunas.|
| **Comentarios** | Las autoridades dispondrán de dispositivos por medio de los cuales se les podrá notificar cuando un ciudadano no se ha presentado a hacerse las pruebas médicas, para que actuen en consecuencia. Por otra parte, también se les informará cuando deben de realizar los controles periódicos de que se cumple la cuarentena entre aquellos ciudadanos que deben cumplirla, será con la minoría de la población que no disponde de teléfono móvil o con aquellos que sí disponen de teléfono móvil pero que no es posible verificar que se encuentran en casa o es imposible contactar con ellos.|

<p align="center"> <b>Tabla 6.3: Actores de negocio a implantar.</b> </p>

| **\<id>004** | Ambulatorio |
| -- | -- |
| **[Versión]** | 1.0(28/11/2020) |
| **[Dependencias]** |Dicho actor participa en los procesos de negocio a implantar:<br> * 002 Gestionar la realización de las pruebas médicas. |
| **Descripción** | Este actor de negocio actual representa al centro de salud que dispondrá de listados donde se informarán del estado de los ciudadanos, así como de las distintas pruebas médicas que se les debe de realizar a cada uno de ellos. También se encargarán de notificar a los ciudadanos las citas en las que se les realizarán las pruebas, asi como las medidas que deben de tomar en caso de dar positivo y cual es la duración de la cuarentena que deben de cumplir.|
| **Comentarios** | Este actor podrá acceder a los datos de los ciudadanos (a sus datos médicos), también será el encargado de registrar el resultado de las pruebas realizadas a los ciudadanos en la plataforma pandemio, para que finalmente se pueda contabilizar dicho positivo y poder hacer un seguimiento de los contactos de dicho positivo, así como proporcionar los datos al gobierno. |

<p align="center"> <b>Tabla 6.4: Actores de negocio a implantar.</b> <br> </p>

#### 4.2.2 Descripción de Procesos de Negocio a Implantar

En esta sección se especificarán cuales serán los procesos de negocio que se implementarán en nuestra plataforma PANDEMIO. Dichos procesos representarán a grandes rasgos la operativa de nuestra plataforma y el funcionamiento general de ella. De esta forma, definiremos como deberán de interactuar los actores definidos en el apartado anterior una vez que el sistema esté en producción. Los procesos de negocio a implementar serán los siguientes.

| **\<id>001** | Rastrear contactos con los casos positivos |
| -- | -- |
| **[Versión]** | 1.0(29/11/2020) |
| **[Dependencias]** | Para que se lleve a cabo este proceso de negocio, se podrán presentar dos situaciones distintas. La primera es que un ciudadano aislado acuda al ambulatorio porque presenta síntomas compatibles con el virus y de positivo en las pruebas. La segunda, es que tras realizarse el proceso de negocio 002 el rastreo de los contactos con los casos positivos alguno de ellos de positivo en las pruebas. En definitiva, este proceso de negocio se dispara cuando hay algún ciudadano que de positivo en las pruebas. |
| **Descripción** | En este proceso de negocio, se llevará a cabo un rastreo de los contactos que haya podido tener un caso positivo confirmado con otros ciudadanos, para ello se podrá realizar este seguimiento por medio de los datos de la localización que nos proporcionen las operadoras telefónicas de los ciudadanos. Nuestra plataforma será capaz de trazar dicha información obteniendo las personas que hayan estado en el mismo lugar que el positivo durante un tiempo superior de 15 minutos, para que a dichas personas posteriormente se les realicen las pruebas médicas oportunas (proceso de negocio 002 Gestionar la realización de las pruebas médicas). También, la plataforma podrá obtener información de cuales han sido los focos de contagios entre los casos que estén relacionados. |
| **[Importancia]** | Alta |
| **[Actores]** | * Ciudadano <br>  |
| **Comentarios** | Para llevar a cavo este proceso de rastreo es necesario conocer los datos de la localización de los ciudadanos suministrados por las operadoras telefónicas de estos. El proceso de rastreo requiere de algoritmos complejos. |

<p align="center"> <b>Tabla 7.1: Procesos de Negocio a implantar.</b> <br> </p>

| **\<id>002** | Gestionar la realización de las pruebas médicas |
| -- | -- |
| **[Versión]** | 1.0(29/11/2020) |
| **[Dependencias]** | Dicho proceso de negocio depende del proceso de negocio 001 Rastrear los contactos con los casos positivos, para poder obtener el listado de las personas a las que se les debe de realizar las pruebas médicas. |
| **Descripción** | Una vez que se ha llevado a cabo el proceso de negocio 001 Rastrear contactos con los casos positivos, la plataforma PANDEMIO suministrará un listado con todos aquellos ciudadanos que sean sospechosos de tener el virus al estar en contacto con un caso positivo confirmado. Una vez que el ambulatorio conozca dicho listado, se encargará de concertar una cita con el ciudadano para que se le realicen las pruebas médicas oportunas y registrarán en la plataforma dicha cita. La plataforma enviará un SMS al ciudadano informandole de que debe de realizarse las pruebas médicas y cuando se le ha concertado la cita para ello.<br> En caso de que algún ciudadano no acuda a la cita médica, el ambulatorio lo registrará en la plataforma y esta se pondrá en contacto con las autoridades para informarle de qué ciudadano no acudió a hacerse las pruebas médicas para que actuen en consecuencia.<br> Una vez que se conozca el resultado de las pruebas médicas, los ambulatorios registrarán el resultado en la plataforma y esta informará a los ciudadanos de los resultados por medio de SMS, además de que el ambulatorio contacte con ellos vía telefónica para informarles de cuales deben de ser las medidas a adoptar, cuarentenas, etc. Si el resultado de la prueba es positivo, se volverá al proceso de negocio 001 Rastrear contactos con los casos positivos y se repetirá el proceso. También entrará en acción el proceso de negocio 003 Gestionar el cumplimiento de la cuarentena|
| **[Importancia]** | Alta |
| **[Actores]** | * Ambulatorio> <br>* Ciudadano <br>* Autoridades |
| **Comentarios** | Cuando un ciudadano no acuda a la realización de las pruebas médicas las autoridades se encargarán de localizarle para que se realicen.|

<p align="center"> <b>Tabla 7.2: Procesos de Negocio a implantar.</b> <br> </p>

| **\<id>003** | Gestionar el cumplimiento de la cuarentena |
| -- | -- |
| **[Versión]** | 1.0(29/11/2020) |
| **[Dependencias]** | Dicho proceso de negocio depende del proceso de negocio 002 Gestionar la realización de las pruebas médicas, dado que el control del cumplimiento de las cuarentenas solo se llevará a cabo en aquellos ciudadanos que hayan dado positivo en las pruebas que se les han realizado o en los ciudadanos que se indique que deben de mantener cuarentena.|
| **Descripción** | Una vez que en la plataforma se conozca cuales son los ciudadanos que deben de cumplir la cuarentena, se llevará a cabo un control de que esta se cumple. Para ello, la plataforma se encargará de localizar a los ciudadanos que deben de cumplir la cuarentena por medio de su telefono móvil, pidiendo que ponga su huella dactilar y localizando el teléfono móvil o por medio de llamadas telefónicas cuando los dispositivos no dispongan de huella dactilar. Cuando se detecte que un ciudadano no cumple la cuarentena por medio de cualquiera de las técnicas anteriores, el sistema informará a las autoridades de su incumplimiento y actuarán en consecuencia. Cuando el sistema detecte que un usuario que debe permanecer en cuarenta está incumpliendola, el sistema se lo notificará por medio de un SMS. |
| **[Importancia]** | Alta |
| **[Actores]** | * Ciudadano <br> * Autoridades |
| **Comentarios** | Si el ciudadano que debe de cumplir cuarentena pertenece al pequeño porcentaje de la población que no dispone de teléfono móvil se informará a las autoridades para que lleven a cabo los controles de cumplimiento de la cuarentena de forma presencial en su domicilio. |

<p align="center"> <b>Tabla 7.3: Procesos de Negocio a implantar.</b> <br> </p>

| **\<id>004** | Suministrar información y estadísticas al gobierno |
| -- | -- |
| **[Versión]** | 1.0(29/11/2020) |
| **[Dependencias]** | Dicho proceso de negocio depende de los procesos de negocio 001 Rastrera contactos con los casos positivos y 002 Gestionar la realización de las pruebas médicas, para que se disponga de la información de los casos positivos y cuales han sido los contactos entre ellos.|
| **Descripción** | Este proceso de negocio es el proceso de negocio sobre el que se basa nuestra plataforma PANDEMIO, a partir del rastreo llevado a cabo en el proceso de negocio 001, la plataforma dipondrá de la información relativa a los casos positivos, los contactos entre los casos positivos, las zonas en las que se han producido y los focos de contagios. El sistema elaborará estadísticas con todos estos datos y serán proporcionados al gobierno, para que dicha información sea interpretada por el comité de expertos y se tomen las medidas oportunas |
| **[Importancia]** | Muy Alta|
| **[Actores]** | * Gobierno |
| **Comentarios** | La información recopilada por la plataforma será proporcionada constantemente al gobierno, asi como cada nuevo caso positivo registrado en la plataforma.|

<p align="center"> <b>Tabla 7.4: Procesos de Negocio a implementar.</b> <br></p>


A continuación se muestra un diagrama de actividad que modela el funcionamiento general del sistema, indicando cuales son los procesos de negocio que se han de llevar a acabo.

![picture 3](images/f0458b44825e71f402de6c44e5a9728c6928ce3145875d9c90e4090b9269f83b.jpg)  

## 5. DESCRIPCIÓN DE LOS SUBSISTEMAS DEL SISTEMA A DESARROLLAR
Para la mejor compresión de la plataforma PANDEMIO que se deseea implementar, dividiremos dicha plataforma en distintos módulos que agruparán las funcionalidades necesarias. Estos subsistemas estarán descritos con mayor detalle en las siguientes tablas. Nos basamos en el diagrama de características del apartado de alcance (1.1).


| **\<id>001** | Rastreo de contacto entre casos positivos y Gestion de Pruebas Médicas|
| -- | -- |
| **[Versión]** | 1.0 (29/11/2020) |
| **[Dependencias]** |Dicho subsistema depende de los objetivos de negocio:<br> * 002 Rastreo del contacto con un positivo.<br> * 003 Asegurar la realización de las pruebas.<br> * 004 Identificar posibles focos de contagio.<br>Contendrá los procesos de negocio a implementar:<br> * 001 Rastrear contactos con los casos positivos. <br> * 002 Gestionar la realización de las pruebas médicas.  |
| **Descripción** | Este subsistema agrupa los requisitos relacionados con el seguimiento de aquellos que han dado positivo en las pruebas, para así crear una lista de las personas afectada y todo aquello que tenga que ver con el rastreo de casos positivos para poder identificar posibles focos de contagio.  |
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Prioridad]** | * Alta |
| **Comentarios** |  |

<p align="center"> <b>Tabla 8.1: Subsistemas a desarrollar.</b> <br> </p>

| **\<id>002** | Gestión del cumplimiento de cuarentena |
| -- | -- |
| **[Versión]** | 1.0 (29/11/2020) |
| **[Dependencias]** | Dicho subsistema depende de los objetivos de negocio:<br> * 005 Asegurar el cumplimiento de la cuarentena.<br> Contendrá los procesos de negocio a implementar:<br> * 003 Gestionar el cumplimiento de la cuarentena.|
| **Descripción** | Este subsistema agrupa los requisitos relacionados con el control de aquellos ciudadanos que han dado positivo en la prueba y asegurandose que los pacientes cumplen el periodo de cuarentena. En caso de incumplimiento se notificara a las autoridades. |
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Prioridad]** | * Alta |
| **Comentarios** | |

<p align="center"> <b>Tabla 8.2: Subsistemas a desarrollar.</b> <br> </p>

| **\<id>003** | Gestión de información y estadísticas al gobierno |
| -- | -- |
| **[Versión]** | 1.0 (29/11/2020) |
| **[Dependencias]** | Dicho subsistema depende de los objetivos de negocio:<br> * 006 Proporcionar información y datos al ministerio .<br> Contendrá los procesos de negocio a implementar:<br> * 004 Suministrar información y estadísticas al gobierno.|
| **Descripción** | Este subsistema agrupa los requisitos relacionados con el suministro de información que se proporcionará al gobierno por parte de los datos recopilados y procesados por la plataforma PANDEMIO.  Estos datos generarán las distintas estadísticas que permitirán localizar los focos de contagio, zonas de más contagios, número de contagios por distrito médico,etc para que así el gobierno pueda tomar las decisiones oportunas. |
| **[Importancia]** | \<importancia del proceso de negocio para el cliente> |
| **[Prioridad]** | * Media |
| **Comentarios** | |

<p align="center"> <b>Tabla 8.3: Subsistemas a desarrollar.</b> <br> </p>

Para que quede claro la descomposición en subsistemas, a continuación se muestra un diagrama de componentes con los subsistemas considerados.

![picture 1](images/fb9286ac15bd71d1f044f3cee392a03ba4dd4dd3f6a1c17516e10f1c3f9427b3.jpg)  


