## 6. CATÁLOGO DE REQUISITOS DEL SISTEMA A DESARROLLAR

En esta sección se van a detallar la solución propuesta para poder satisfacer las necesidades que queremos cubrir con nuestro sistema. 

Para poder cumplir con los objetivos principales hemos realizado un primer agrupamiento de los mismos teniendo en cuenta la organización en subsistemas que
ya describimos en la seccción anterior. Una vez establedcidos los subsistemas o requisitos generales los desgranaremos en requisitos más especificos de manera
que podamos llevar a cabo todos los casos de uso que se planterán tambien en esta misma seccion.

_Esta sección debe contener la descripción de la solución que el ingeniero de requisitos propone al cliente para satisfacer sus necesidades de negocio.
Esta solución se define mediante los requisitos del sistema a desarrollar (requisitos de producto en terminología CMMI-DEV).
Esta sección se divide en las secciones que se describen a continuación, cada una de las cuales puede organizarse internamente como se considere oportuno
para facilitar la legibilidad del documento, siendo la organización más habitual la división en los subsistemas descritos en la sección 5, en cuyo caso la
estructura del índice para la sección sería la que puede verse en la siguiente figura._


### 6.1. Requisitos Generales del Sistema

Como ya hemos explicado, vamos a describir un primer acercamiento a lo que serán los requisitos del sistema. Para ello agruparemos los requisitos de una manera general 
siguiendo el patrón marcado en los subsistemas de la sección 5. De esta manera podemos establecer de un modo general y algomerado los siguientes requisitos generales del sistema:

1.- Rastrear el contacto entre casos positivos y Gestionar las Pruebas Médicas:
Este requisito general agrupará aquellos requisitos más concretos relacionados con el seguimiento de los ciudadanos que han dado positivo en las pruebas realizadas, y 
los relacionados con la realización de la pruebas pertinentes a aquellos cuidadanos susceptibles de haber sido contagiados por el positivo. De este modo podremos crear
una lista de las personas afectadas añadiendo toda aquella información que pueda ser de ayuda, como conseguencia de este rastreo de positivos, para poder identificar 
posibles focos de contagio.

2.- Gestionar el cumplimiento de cuarentena:
Este requisito general agrupará los requisitos relacionados con el control de los ciudadanos que han dado positivo en la prueba, asegurandose que los pacientes cumplen el 
periodo de cuarentena. Incluirán aquellos requisitos que aseguren el cumplimiento de la cuarentena pero también aquellos que nos permitan actuar en caso de verse violada.

3.- Gestionar la información recopilada y proporcionar estadísticas al gobierno:
Este subsistema agrupará los requisitos relacionados con el suministro de la información que se proporcionará al gobierno con respecto a los datos recopilados y procesados
por la plataforma.  Estos datos darán lugar a estadísticas que una vez analizadas nos posibilitará localizar los posiles focos de contagio, zonas donde más contagios hay, número 
de contagios por distrito médico...etc. De esta manera el gobierno podrá tomar las decisiones o medidas que crea convenientes.

_Esta sección debe contener la especificación de los requisitos generales del sistema, también denominados características del sistema (system features) u objetivos
del sistema, especificados mediante las plantillas para requisitos generales que se muestran a continuación. Los requisitos generales puede que ya se encuentren
especificados total o parcialmente en documentación previa como el Pliego de Prescripciones Técnicas, la Oferta seleccionada o el Estudio de Viabilidad del Sistema,
en cuyo se podrán reutilizar y se hará referencia a dichos documentos como fuente de los mismos. En el caso de que se considere necesario, los requisitos generales
se podrán descomponer jerárquicamente para facilitar su comprensión._
