### 6.5 Restricciones Técnicas del Sistema.
En este apartado se comentarán las restricciones técnicas del sistema detectadas, para ello no se dispone de suficiente información acerca del sistema a desarrollar, y se deberá de llevar a cabo alguna reunión mas con los stakeholders para obtener dichas restricciones técnicas. Sin embargo, aqui hemos considerado algunas de ellas que son necesarias para un correcto funcionamiento del sistema.

| **\<id>001** | Compatibilidad con navegadores |
| -- | -- |
| **[Versión]** | 1.0 (12/12/2020)|
| **[Dependencias]** |Ninguna|
| **Descripción** | El sistema deberá de ser compatible con los navegadores Google Chrome, Modzilla Firefox y Safari. |
| **[Importancia]** |Baja |
| **[Prioridad]** |Baja |
| **[Estado]** | Pendiente|
| **Comentarios** | Se considera necesario que el sistema sea compatible con los tres navegadores más utilizados del mercado, debido a que se espera que el sistema sea ejecutado en gran cantidad de dispositivos con distintas configuraciones.|

### 6.6 Requisitos de Integración del Sistema.
En este apartado se habla de los requisitos de integración del sistema, en este caso dado a que no se dispone de la suficiente información acerca de esta parte del sistema se deberán obtener dichos requisitos por medio de distintas reuniones con los stakeholders en futuras iteraciones.

### 6.7 Información sobre trazabilidad.

En este apartado mostraremos una matriz que nos permita visualizar las distintas relaciones y dependencias entre requisitos, para eso tendremos en cuenta las dependecias de cada uno de los requisitos anteriormente citados. La matriz de trazabilidad que mostramos a continuación se corresponde con la matriz de trazabilidad de Casos de Uso frente a requisitos generale.

| Requisitos generales / Casos de Uso | 1.0 Rastreo de contactos y gestion pruebas | 2.0 Cumplimiento cuarentena| 3.0 Gestion informacion y estadísticas|
|-- | -- | -- | -- |
|0.1 Listar ciudadanos por estado|X|X||
|0.2 Informar a ciudadano |X|X||
|1.1 Registrar ciudadano en el sistema|X|||
|1.2 Registrar resultado de la prueba en el sistema|X|||
|1.3 Rastrear contactos directos con el postivo|X|||
|1.4 Adquirir datos de los ciudadanos.|X|||
|1.5 Registrar contactos directos en el sistema.|X|||
|1.6 Registrar cita pruebas en el sistema.|X|||
|1.7 Enviar alerta a las autoridades de incumplmiento de realizarse la prueba.|X|||
|2.1 Control automático por el sistema del cumplimiento cuarentena.(Ciudadanos con móvil).||X||
|2.2 Control humano por las autoridades (Ciudadanos sin móvil)||X||
|2.3 Enviar alerta autoridades incumplimiento cuarentena||X||
|3.1 Informar caso positivo|||X|
|3.2 Generar estadísticas|||X|
|3.3 Informar estadísticas|||X|
|3.4 Informar foco de contagio|||X|