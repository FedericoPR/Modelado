**Requisitos de Fiabilidad**

| **RNF 01** | Copias de seguridad |
| -- | -- |
| **[Versión]** | 1.0 (12/12/2020)|
| **[Dependencias]** |Ninguna|
| **Descripción** |El sistema deberá realizar una copia de seguridad de las bases de datos cada hora. |
| **[Importancia]** |Alta |
| **[Prioridad]** |Alta |
| **[Estado]** | Pendiente|
| **Comentarios** | Se considera que la frecuencia de realización de la copia de seguridad por parte de las bases de datos debe de ser de una hora, dado que se considera que como mucho se puedan perder los datos de nuevos positivos que se registren en el sistema en un periodo de tiempo de una hora. Los periodos de tiempo mayores a una hora se considera que son grandes pérdidas de información.|

<p align="center"> <b>Tabla 16.1: Requisitos no funcionales del sistema</b> <br> </p>

| **RNF 02** | Servidores de respaldo |
| -- | -- |
| **[Versión]** | 1.0 (12/12/2020)|
| **[Dependencias]** |Ninguna|
| **Descripción** |El sistema deberá disponer de varios servidores de respaldo. |
| **[Importancia]** |Alta |
| **[Prioridad]** |Alta |
| **[Estado]** | Pendiente|
| **Comentarios** | Se considera necesario que el sistema deba disponer de varios servidores de respaldo en caso de que un servidor pueda estar colapsado,el sistema deberá de poder seguir dando servicio.|

<p align="center"> <b>Tabla 16.2: Requisitos no funcionales del sistema</b> <br> </p>

| **RNF 03** | Recuperación autónoma ante fallos |
| -- | -- |
| **[Versión]** | 1.0 (12/12/2020)|
| **[Dependencias]** |Requisito no funcional 001 Copias de seguridad.|
| **Descripción** |El sistema deberá poder recuperarse aunte cualquier fallo inesperado de forma autónoma en un tiempo no superior a los 15 minutos. |
| **[Importancia]** |Alta |
| **[Prioridad]** |Alta |
| **[Estado]** | Pendiente|
| **Comentarios** | Se considera necesario que el sistema deba de poder recuperarse al estado anterior a la ocurrencia de cualquier fallo inexperado (volviendo a una copia de seguridad previa a la ocurrencia del fallo), en un tiempo relativamente corto para que no se deje de proporcionar el servicio durante largos periodos de tiempo.|

<p align="center"> <b>Tabla 16.3: Requisitos no funcionales del sistema</b> <br> </p>

**Requisitos de portabilidad**

| **RNF 14** | Fácil instalación |
| -- | -- |
| **[Versión]** | 1.0 (12/12/2020)|
| **[Dependencias]** |Ninguna|
| **Descripción** |El sistema deberá de poder ser instalado en los equipos en un tiempo no superior a 2 horas en el 90% de los casos.|
| **[Importancia]** |Baja |
| **[Prioridad]** |Baja |
| **[Estado]** | Pendiente|
| **Comentarios** | Se considera necesario que el sistema deba de poder ser instalado en los equipos en un tiempo relativamente corto, debido a que se pronostica que deberá ser instalado en un gran número de equipos.|

<p align="center"> <b>Tabla 16.14: Requisitos no funcionales del sistema</b> <br> </p>

| **RNF 15** | Multiplataforma |
| -- | -- |
| **[Versión]** | 1.0 (12/12/2020)|
| **[Dependencias]** |Ninguna|
| **Descripción** |El sistema deberá de poder ser instalado en cualquier equipo con independencia del software y hardware utilizado, es decir, debe de ser multipataforma.|
| **[Importancia]** |Alta |
| **[Prioridad]** |Alta |
| **[Estado]** | Pendiente|
| **Comentarios** | Se considera necesario que el sistema deba de poder ser instalado en distintos equipos con independencia de la plataforma (SO y Hardaware) del equipo. Dado que se pronostica que el sistema será instalado en gran cantidad de equipos con configuraciones muy dispares entre ellos.|

<p align="center"> <b>Tabla 16.15: Requisitos no funcionales del sistema</b> <br> </p>

| **RNF 16** | Coexistencia con distintos sistemas |
| -- | -- |
| **[Versión]** | 1.0 (12/12/2020)|
| **[Dependencias]** |El requisito de conducta El sistema deberá adaptar su comunicación con lo sistemas de información de cada autonomía|
| **Descripción** |El sistema deberá de poder coexistir con los diferentes sistemas sanitarios de las comunidades autónomas.|
| **[Importancia]** |Alta |
| **[Prioridad]** |Alta |
| **[Estado]** | Pendiente|
| **Comentarios** | Se considera necesario que el sistema deba de poder coexistir con los distintos sistemas de información sanitarios de las distintas autonomías dado que cada autonomía dispondrá de un sistema de información propio en el que mantendra los datos relativos a los pacientes de cada comunidad autónoma.|

<p align="center"> <b>Tabla 16.16: Requisitos no funcionales del sistema</b> <br> </p>
