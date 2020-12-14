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
- El sistema deberá adaptar su comunicación con lo sistemas de información de cada autonomía.

**Requisitos de Conducta:** (algo más especifico)(**Sergio**)
- El sistema deberá verificar el cumplimiento de la cuarentena por medio de la ubicación.
- El sistema deberá solicitar los datos relevantes a la localización de los ciudadanos a las operadoras.
- El sistema debera realizar un rastreo de contactos de forma automática con cada positivo registrado.
- El sistema deberá de enviar alertas vía sms con cada alteración del estado del ciudadano.
- El sistema deberá diferenciar como llevar a cabo el cumplimiento de la cuaentena en e función del tipo de movil del ciudadano tipos de movil (o si no dispone de el).
- El sistema deberá enviar estadísticas generales al gobierno de forma automática cada 3 días

# Requisitos no funcionales:

**Requisitos de Fiabilidad:** (**Angel**)
- El sistema deberá realizar una copia de seguridad de las bases de datos cada hora.
- El sistema deberá disponer de varios servidores. (Con el fin de evitar caidas del sistema o colapsos).
- El sistema deberá poder recuperarse aunte cualquier fallo inesperado de forma autónoma en un tiempo no superior a los 15 minutos.(Volver a las copias de seguridad anteriores).

**Requisitos de Usabilidad:**(**Sergio**)
- El sistema deberá permitir que un usuario novato no tarde mas de 15 minutos en aprender su funcionamiento.
- El sistema deberá permitir en el 75% de los casos que con un máximo de 5 clicks se pueda acceder a la información deseada.
- El sistema deberá disponer de una interfaz gráfica intuitiva.
- El sistema deberá mostrar mensajes de ayuda al realizar cualquier operación.
- El sistema deberá mostrar la información en el idioma elegido.

**Requisitos de Eficiencia:**(**Fredy**)
- El sistema deberá de rasterar los contactos entre casos positivos en un tiempo no superior a 15 minutos en el 90% de los casos.
- El sistema deberá generar informes con las estadísticas de los datos en un tiempo no superior a 30 minutos en el 80% de los casos.
- El sistema deberá mandar un aviso del incumplimiento de la cuarentena a las autoridades en un tiempo inferior a 1 minuto desde que es detectado.
- El sistema deberá tener un tiempo máximo de respuesta de 10 segundos para cualquier consulta que se realice en el.

**Requisitos de Mantenibilidad:** (**Sergio**)
- El sistema deberá de contener una base de datos cuya estructura sea lo más simplificada posible.

**Requisitos de Portabilidad:** (**Angel**)
- El sistema deberá de poder ser instalado en los equipos en un tiempo no superior a 2 horas en el 90% de los casos.
- El sistema deberá de poder ser instalado en cualquier equipo con independencia del software y hardware utilizado, es decir, debe de ser multipataforma.
- El sistema deberá de poder coexistir con los diferentes sistemas sanitarios de las comunidades autónomas.

**Requisitos de Seguridad:**(**Fredy**)
- El sistema deberá disponer de métodos de autenticación de los que dependerán las vistas a mostrar y la información a la que será accesible.
- El sistema deberá destruir los datos de los ciudadanos una vez que ya no sean útiles en un tiempo no superior a 5 días.
- El sistema deberá anonimizar los datos para todos aquellos usuarios que no dispongan de autorización.

**Otros requisitos no funcionales: