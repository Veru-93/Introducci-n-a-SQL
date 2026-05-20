1. Instala POSTGRESQL, no olvides incluir pgAdmin4 en https://www.enterprisedb.com/downloads/postgres-postgresql-downloads 
2. Abre la bash psql 
Esribe 
psql -U <username> -d <database_name>
Reemplaza <username> por tu nombre de usuarui y <database_name> por postgres 
> Deberías ver: 
>postgres=# 

3. Vamos a crear una base de datos. Escribe
CREATE DATABASE Artisticus

4. Escribe CREATE TABLE Pinturas();

5. Escribe ADD COLUMN Stock;
   Así creamos una columna

6. Escribe ADD COLUMN Color;

7. Para ver tu proceso escribe
SELECT * FROM Pinturas;

> Utilizamos SELECT cuando queremos consultar un dato
> Utilizamos * para ver todo el contenido 
> Después de FROM necesitamos saber a qué tabla estamos consultando, ya que otras veces tendremos muchas tablas relacionadas entre sí y hay que especificar cuál. 
>
Deberías ver la tabla que has creado
7. Continua escribendo 
ALTER TABLE Pinturas (Stock,Color) VALUES (5,'Azul')

Estamos añadiendo valores a nuestra tabla. Le estamos diciendo que en la tabla Pinturas, enlas colmunas de stock y Color le añada los valores 5 y la cadena Azul. Los INTEGER se introducen sin más carácteres, mientras que los datos de tipo VARCHAR deben ir entre comillas. 

8. Si vuelves a realizar la consulta SELEC * FROM Pinturas deberás ver los datos actualizados.


¡Enhorabuena! Has conocido los primeros comandos necesarios para iniciarte en el SQL standar.

