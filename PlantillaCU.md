#### 6.2.3 Especificación de Casos de Uso del Sistema

| **\<id>999** | \<nombre descriptivo> |  |
| --- | --- | --- |
| **[Versión]** | <nº versión>(<fecha de versión>) |
| **[Dependencias]** | * \<requisitos generales del sistema de los que depende> <br> * \<lista de casos de uso que invoca> <br> * \<otros requisitos de los que depende> <br> * ... |
| **Precondición** | \<precondición del caso de uso del sistema> |
| **Descripción** | El sistema deberá comportarse como se describe en el siguiente caso de uso [abstracto] cuando {\<evento de activación>, sea necesario para la realización de otros casos de uso}. |
| **Secuencia Normal** | **Paso** | **Acción** |
|  | 1 | {El actor <actor del sistema>, El sistema} \<acción/es realizada/s por el actor del sistema> |
|  | 2 | Se realiza el <caso de uso del sistema> |
|  | 3 | Si \<condición>, |
|  | ... | ... |
|  | 3.n. | {El caso de uso termina con éxito, Se cancela el caso de uso} |
|  | ... | ... |
| **Postcondición** | \<postcondición del caso de uso del sistema> |
| **Excepciones** | **Paso** | **Acción** |
|  | P | Si <condición de excepción> |
|  | ... | ... |
|  | E.m | {El caso de uso continua, Se cancela el caso de uso} |
|  | ... | ... |
| **Rendimiento** | **Paso** | **Cota de tiempo** |
| | q | k<unidad de tiempo> |
| | ... | ... |
| **Frecuencia** | \<nº veces / unidad de tiempo> |
| **[Importancia]** | \<importancia del caso de uso para el cliente> |
| **[Prioridad]** | \<prioridad del caso de uso para la dirección del proyecto> |
| **[Estado]** | \<estado del caso de uso según el ciclo de vida adoptado por el proyecto> |
| **Comentarios** | \<comentarios adicionales sobre el caso de uso del sistema> |
