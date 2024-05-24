# Creacion de MOD en SQLite3

1. Crear base en un archivo **.db** nombre: <br> **-MODP.db** <br>
-Nombre de la tabla: **MOD_PB** <br>
-Path: C:\SQLite\MOD\MODP.db

2. Se agregaron todos los registros del archivo "MOD 2022.accdb" en particular la tabla llamada [MOD 2022].

3. Se creo un **backup** de la tabla principal con todos los registros llamada: **Backup_MOD**

4. Se creo una tabla llamada **Original_budgets** con todos los presupuestos de todos los años por medio de la consulta:<br>
*select * from MOD_PB as a where(a.Objetivo <> '');*<br>
El objetivo de esta tabla es que sea un backup de presupuestos y poder analizarla para eliminar los presupuestos de la tabla de transacciones MOD_PB.

5. Creamos el campo Mes_numero, para poder concatenar la fecha en una sola necesitamos que el mes no sea formato de texto.

0. Crear tablas de **Butgets** sera una por Ejecutivos y otra por Estados:<br>
**-Butgets_executive**<br>
**-Butgets_state**

"C:/Users/abia04/Downloads/2019.csv"
