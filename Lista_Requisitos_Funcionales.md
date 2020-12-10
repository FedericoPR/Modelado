# Requisitos funcionales

**Requisitos de información del Sistema:** (**Ángel**)
- El sistema deberá almacenar los datos relativos al ciudadanos; nombre, DNI, dirección, Telefono Movil(Numero), si dispone de telefono o no, cómo es.
- El sistema deberá almacenar la informacion sobre el resultado de las pruebas a realizar a los  ciudadanos: fecha de realización, resultado y fecha fin de cuarentena.
- El sistema deberá registrar la información relevante a las citas para realizar las pruebas a los ciudadanos: Hora, dia y ambulatorio.
- El sistema deberá almacenar los datos de la locacización de los ciudadanos proporcionados por la operadora: ciudadano, lugar, tiempo y fecha.
- El sistema deberá almacenar la información relevante al estado medico los ciudadanos registrados en el sistema.
- El sistema deberá almacenar un registro actualizable sobre si los ciudadanos están cumpliendo la curentena (Localización del móvil cada 10 mins).
- El sistema almacenará informes sobre las estadísticas generadas.

**Requisitos de Reglas de Negocio del Sistema:** (Referido a las limitaciones de mi sistema y leyes a cumplir) (**Fredy**)
- El sistema deberá cumplir la LPD a la hora de almacenar los datos relativos del ciudadano.
- El sistema deberá anonimizar los datos de los ciudadanos a aquellos que no tengan autorización.
- El sistema deberá destruir la información relativa al ciudadano una vez sea inservible.
- El sistema deberá adaptar su comunicación con lo sistemas de información de cada autonomía.

**Requisitos de Conducta:** (algo más especifico)(**Sergio**)
- El sistema deberá verificar el cumplimiento de la cuarentena por medio de la ubicación.
- El sistema deberá solicitar los datos relevantes a la localización de los ciudadanos a las operadoras.
- El sistema debera realizar un rastreo de contactos de forma automática con cada positivo registrado.
- El sistema deberá de enviar alertas vía sms con cada alteración del estado del ciudadano.
- El sistema deberá diferenciar como llevar a cabo el cumplimiento de la cuaentena en e función del tipo de movil del ciudadano tipos de movil (o si no dispone de el).
- El sistema deberá enviar estadísticas generales al gobierno de forma automática cada 3 días
