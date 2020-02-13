# Apuntes de SQL para Bases de Datos
## Índice
- [Detalles importantes](#detalles-importantes)
- [Clausulas](#clausulas)

## Detalles importantes
1. Los strings van siempre entre comillas simples.
2. La \ sirve para dejar un espacio en blanco.
3. Para poner mayor o menor + igual, él = deve de ir despues de < o >.
4. Para indicar que algo es diferente utilizaremos **<>**.
5. Siempre terminaremos una consulta con **;** punto y coma.
6. Para hacer comentarios en una linea usaremos **--** antes del comentario.
7. Para hacer los comentarios en varias lineas usaremos **/* */** poniendo el comentario entre los asteriscos.
8. Las clausulas SELECT, FROM, WERE, HAVING ... iran siempre en mayúsculas.

## Clausulas

### SELECT
La instrucción SELECT se utiliza para seleccionar datos de una base de datos.
```SQL
SELECT column1, column2, ...
FROM table_name;
```
Aquí, columna 1, columna2, ... son los nombres de los campos que utilizamos para selecionar los datos que queremos mostrar.
### FROM
La intruccion FROM se utiliza para indicar en que tabla o tablas se encuentran los atributos que selecionamos con en SELECT.
```SQL
SELECT column1, column2, ...
FROM table_name;
```
Aquí, table_name es el nombre de la tabla en la que se encuentra la columnas column1, column2.
### WHERE
La cláusula WHERE se usa para filtrar registros.
```SQL
SELECT *
FROM Customers
WHERE Country='Mexico';
```
En esta instrucción SQL selecciona a todos los clientes del país "México", en la tabla "Customers".
