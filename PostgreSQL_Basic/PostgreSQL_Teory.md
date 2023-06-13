# PostgreSQL
## ¿Qué es PostgreSQL?
Es un motor de base de datos.
* Open Source.
* Basado en SQL.
* Desde 1986(University of California, Berkeley).
* Permite el uso de PostGiS, para no depender de un backend.
* Cumple con el Estandar:
    * A: Atomicity - Atomicity es la idea de que si una transacción falla, no debe ejecutarse ninguna de las operaciones que contenía.
    * C: Consistency - Con consistencia se refiere a que los datos se deben almacenar en la base de datos en el orden y forma que se creó.
    * I: Isolation - Isolación es la idea de que una transacción no puede tener acceso a los datos de otra transacción durante su ejecución.
    * D: Durability - Durabilidad es la idea de que una transacción debe almacenar los datos durante su ejecución y no se va a perder si la base de datos se daña.
## Bash
* \?: Mostrará una lista de comandos disponibles.
* \l: Mostrará las bases de datos creadas.
* \dt: Mostrará las tablas de la base de datos de posgres.
* \c: Se conecta a la base de datos deseada.
* \d: Mostrará las columnas de una tabla.
* \h: Mostrará una lista de comandos SQL disponibles.
* SELECT version();: Mostrará la versión de PostgreSQL instalada.
* \g: Mostrar lista de comandos que se estan ejecutando en la base de datos actual.
* \timing: Mostrará el tiempo que tarda cada comando en ejecutarse.
## Archivos de configuración
Archivos Configuracion
* postgresql.conf
* pg_hba.conf
* pg_ident.conf
Muestra la ruta de nuestros archivos de configuracion
SHOW config_file;
* postgresql.conf: Configuración general de postgres, múltiples opciones referentes a direcciones de conexión de entrada, memoria, cantidad de hilos de pocesamiento, replica, etc.
* pg_hba.conf: Muestra los roles así como los tipos de acceso a la base de datos.
* pg_ident.conf: Permite realizar el mapeo de usuarios. Permite definir roles a usuarios del sistema operativo donde se ejecuta postgres.
