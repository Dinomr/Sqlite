# Sqlite

Es una base de datos relacional SQL muy ligera, por lo que es usada para
desarrollo en dispositivos con caracteristicas my limitadas o que no
necesitan un rigor muy alto en este sentido. Su forma de escribir comandos
es la misma que la de SQL, a exepción de algunas características, pero
en teoría son lo mismo.

## UPDATE

La sentencia update nos permite actualizar algun dato que añamos insertado
y va siempre acompañado de la clausula where para saber cual es el registro
o conjunto de registros que debe modificar.

<div style="text-align: center;">
<img src="./images/1.png">
</div>

## .SCHEMA

Esta sentencias nos retorna todas las tablas que hayamos creado junto
sus conlumnas

<div style="text-align: center;">
<img src="./images/2.png">
</div>

## Date and time functions

* date() nos retorna la fecha en el siguiente formato: YYYY-MM-DD.
* time() nos retorna la hora en el siguiente formato: HH:MM:SS.
* datetime() nos retorna la fecha y hora en el siguiente formato: YYYY-MM-DD HH:MM:SS
* julianday() nos retorna la fecha en el calendario juliano
* unixepoch() retorna la fecha en un timestamp de unix
* strftime() retorna la fecha en el formato que sea indicado
    * %d		día en número : 00
    * %f		segundos fraccionales: SS.SSS
    * %H		hora: 00-24
    * %j		día del año: 001-366
    * %J		dia juliano número (fractional)
    * %m		mes 01-12
    * %M		minuto 00-59
    * %s		segundos desde 1970-01-01
    * %S		segundos: 00-59
    * %w		dia de la semana 0-6 with Sunday==0
    * %W		semana del año 00-53
    * %Y		año 0000-9999
    * %%		%

<div style="text-align: center;">
<img src="./images/3.png">
</div>

## Primary key constraint

Es el identificador unico de cada registro, con el podemos hacer las relacuones a las
diferentes tablas de la base de datos. No puede ser un valor nulo ni tampoco estar
duplicado este valor, ya que es el identificador unicó.

<div style="text-align: center;">
<img src="./images/4.png">
</div>

## NOT NULL constraint

Es una restricción que le podemos dar al campo, este not null lo ingresamos en la
creación de una tabla cuando no queremos que dejen vacio ese campo, por lo que lo
hace que sea obligatorio.

<div style="text-align: center;">
<img src="./images/5.png">
</div>

## UNIQUE

Esta restricción impone una unicidad en un campo, pero este no va a ser usado para
realizar relaciones, esto puede ser aplicado a número de documentos, correos,
dirrecciones, etc.

<div style="text-align: center;">
<img src="./images/6.png">
</div>

## DEFAULT

Esta restriccion va a ser que el campo tenga un valor por defecto, por lo que también
se puede usar para evitar valores nulos.

<div style="text-align: center;">
<img src="./images/7.png">
</div>

## CHECK

El check nos permite hacer una restricción mucho mas allá de unique o default, ya que
nosostros podemos establecer la conidición necesaria para que permita ingresar la
información del campo.

<div style="text-align: center;">
<img src="./images/8.png">
</div>

## ALTER TABLE

Nos sirve para modificar la estructura de una tabla, pero no es recomendable hacer esto
cuando ya  tiene registros la base de datos. Nos permite cambiar las restricciones de un campo,
renombrarlo, añadir o eliminarlo.

<div style="text-align: center;">
<img src="./images/9.png">
</div>

## DELETE, DROP

La sentencia delete nos sirve para eliminar un registro y el drop para eliminar una tabla
o columna.

<div style="text-align: center;">
<img src="./images/9.png">
</div>

<div style="text-align: center;">
<img src="./images/10.png">
</div>

## BACKUP, RESTORE

Backuo crea una copia de la base de datos y restore lo que va a hacer es restaurar ese
backup que hicimos, es decir devolver todo como estaba, todo lo que pudimos guardar.

<div style="text-align: center;">
<img src="./images/12.png">
</div>