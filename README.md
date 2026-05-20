1. Instala POSTGRESQL https://www.enterprisedb.com/downloads/postgres-postgresql-downloads (No olvides guardar tu contraseña en algún lado, en el futuro lo agradecerás)
2. Abre la bash psql del sistema
Click intro al local host, database y usuario. Introduce la contraseña que guardaste (si la perdiste...mira que te avisé ¬¬)

Deberías ver esto:
>postgres=# 

3. Vamos a crear una base de datos. Escribe
CREATE DATABASE Artisticus;

Deberías ver un mensaje CREATE DATABASE

4. Escribe 
\l 

y verás una lista de las base de datos incluidas en Postgres por defecto y también Artisticus

Si no lo ves, mira que no te hayas olvidado el punto y coma ¬¬

5. Escribe CREATE TABLE Maquillaje();
Si entra, verás CREATE TABLE

6. Escribe ALTER TABLE Maquillaje ADD Stock INT;
   Así creamos una columna
Le estamos diciendo que en la tabla Maquillaje, añada una columna llamada Stock de tipo de dato INT, ya que el valor que añadiremos será numérico.
7. Escribe ALTER TABLE Maquillaje ADD Color VARCHAR(15);
Dentro de la tabla Pinturas, añade la columne Color. Tipo de dato VARCHAR.
Recuerda que Varchar lo usamos para cadenas y entre paréntesis colocamos el número de caracteres que soporta.
8. Para ver tu proceso escribe
SELECT * FROM Maquillaje;

> Utilizamos SELECT cuando queremos consultar un dato
> Utilizamos * para ver todo el contenido 
> Después de FROM necesitamos saber a qué tabla estamos consultando, ya que otras veces tendremos muchas tablas relacionadas entre sí y hay que especificar cuál. 

Deberías ver la tabla que has creado

9. Continua escribendo 
INSERT INTO Maquillaje (Stock,Color) VALUES (5, 'Azul');

Estamos añadiendo valores a nuestra tabla. Le estamos diciendo que inserte atributos en la tabla Pinturas, en las colmunas de Stock y Color le añada los valores 5 y la cadena Azul. Los INTEGER se introducen sin más carácteres, mientras que los datos de tipo VARCHAR deben ir entre comillas. 

10. Si vuelves a realizar la consulta SELECT * FROM Pinturas verás tu tabla. Añade todos los valores que quieras.

11. Si te equivocaste en algún paso y quieres empezar de nuevo, escribe;
DROP DATABASE artisticus;

Elimina la database y vuelve al paso 3.

¡Enhorabuena! Has conocido los primeros comandos necesarios para iniciarte en el SQL standar.

