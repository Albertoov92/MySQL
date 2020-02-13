# Apuntes de SQL para Bases de Datos
## Índice
- [Detalles importantes](#detalles-importantes)
- [Clausulas](#clausulas)
  - [SELECT](#select)
  - [FROM](#from)
  - [WHERE](#where)
    - [Operadores de WHERE](#operadores-de-where)

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
#### Operadores de WHERE
- El operador **IN** es una abreviatura para múltiples condiciones OR.  
La siguiente instrucción SQL selecciona a todos los clientes que se encuentran en "Germany", "France" o "UK":
```SQL
SELECT *
FROM Customers
WHERE Country IN ('Germany', 'France', 'UK');
```

- El operador **LIKE** se usa para buscar un patrón específico en una columna.  
Hay dos comodines que se usan con frecuencia junto con el operador LIKE:
  - %: El signo de porcentaje representa cero, uno o varios caracteres.
  - _ - El guión bajo representa un solo carácter.

  La siguiente instrucción SQL selecciona a todos los clientes con un CustomerName que comienza con "a":
```SQL
  SELECT *
  FROM Customers
  WHERE CustomerName LIKE 'a%';
  ```
- El operador **BETWEEN** selecciona valores dentro de un rango dado. Los valores pueden ser números, texto o fechas.   
La siguiente instrucción SQL selecciona todos los productos con un precio BETWEEN  10 y 20:
```SQL
SELECT *
FROM Products
WHERE Price BETWEEN 10 AND 20;
```
- Los operadores **<, > o =** se utilzan para comparar datos de las tablas.
```sql
SELECT nombre
FROM world
WHERE population > 200000000;
```
###ORDER
