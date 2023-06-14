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
## Archivos de Configuración
* postgresql.conf
* pg_hba.conf
* pg_ident.conf
Muestra la ruta de nuestros archivos de configuracion
SHOW config_file;
* postgresql.conf: Configuración general de postgres, múltiples opciones referentes a direcciones de conexión de entrada, memoria, cantidad de hilos de pocesamiento, replica, etc.
* pg_hba.conf: Muestra los roles así como los tipos de acceso a la base de datos.
* pg_ident.conf: Permite realizar el mapeo de usuarios. Permite definir roles a usuarios del sistema operativo donde se ejecuta postgres.
## Comandos
* SELECT VERSION();
    * PostgreSQL 11.6 (Ubuntu 11.6-1.pgdg18.04+1) on x86_64-pc-linux-gnu, compiled by gcc (Ubuntu 7.4.0-1ubuntu1~18.04.1) 7.4.0, 64-bit
* \h -- ayuda
* \h comnado -- ayuda del comando especifico
* \l -- Listar las bases
* \c base de datos --moverse a una base de datos especifica
* \dt -- listar las tablas de la base actual
* \dn -- listar los esquemas de la base actual
* \dv -- listar las vistas
* \df -- listar las funciones
* \du -- listar los usuarios
* \g -- ejecutar ultimo comando 
* \s -- historial de comandos
* \l nombrearchivo --guardar lista de comandos
* \i nombre archivo -- ejecuta comandos guardados
* \e -- abrir editor 
* \ef -- editor de funciones
* \timming -- activar o desactivar el tiempo de respusta de las consultas
* \q cerra consola
* CREATE DATABASE base; -- crea base
* CREATE TABLE tabla (columnas); crea tabla
* INSERT INTO tabla(columna) VALUES('dato');
* SELECT * FROM tabla;
* UPDATE tabla SET cammpo = dato WHERE condicion;
* DELETE FROM tabla WHERE condicion;
