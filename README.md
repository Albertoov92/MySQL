# Apuntes de SQL para Bases de Datos
## Índice
- [Detalles importantes](#detalles-importantes)
- [Consultas DQL](#consulta_dql)
-- [Ejemplo estructura basica SQL DQL](#ejemplo_estructura_basica_sql_dql)
## Detalles importantes
1. Los strings van siempre entre comillas simples.
2. La \ sirve para dejar un espacio en blanco.
3. Para poner mayor o menor + igual, él = deve de ir despues de < o >.
4. Para indicar que algo es diferente utilizaremos **<>**.
5. Siempre terminaremos una consulta con **;** punto y coma.
6. Para hacer comentarios en una linea usaremos **--** antes del comentario.
7. Para hacer los comentarios en varias lineas usaremos **/* */** poniendo el comentario entre los asteriscos.
8. Las clausulas SELECT, FROM, WERE, HAVING ... iran siempre en mayúsculas.
## Consultas DQL
### Ejemplo estructura basica SQL DQL
```SQL
SELECT Nombre_Columna, Nombre_Columna2 AS [Expresion]
FROM Nombre_Tabla_Vista
WHERE Condiciones
ORDER BY ListaColumnas [ ASC / DESC ];
```
### Practica
