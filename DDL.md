# Data Definition Language
## Índice
  - [Detalles importantes](#detalles-importantes)
  - [O sublinguaxe DDL](#o-sublinguaxe-ddl)
    - [```CREATE```](#create)
      - [```CREATE (DATABASE|SCHEMA)```](#create-(databse|schema))

### Detalles importantes
  > Cando algo esta entre ```[]``` é opcional.    
  > Cando hai unha ```|``` significa OU.    
  > Recomendase evitar o uso de acentos e espazos nas expresions.

### O sublinguaxe DDL
O sublanguage SQL é usado crear bases de datos, taboas, usuarios ou dominios. Tamen nos permite engadir atributos cun tipos de da tos definidos e establecer restricions e establecer criterios nas taboas interelacionadas. Chámase DDL porque significa linguaxe de definición de datos.





### ```CREATE```
- #### ```CREATE (DATABASE|SCHEMA)```
  Ambos dous teñen a mesma función, declarar a Base de Datos na que engadiremos as táboas, datos e restricións.
  Anque dependendo do xestor utilizado pode variar a función de cada un. En MySQL podemos usar os dous indistintamente. Sen embargo en PostgreSQL. ```ESCHEMA``` é usado como unha capa intermedia entre ```DATABASE``` e as táboas que a compoñen.  
    **FORMULÁ**
  ```SQL
  Create (DATABASE|SCHEMA)
         [IF NOT EXISTS] <nomeBD>
         [CHARACTER SET <nomeDoCharset>]
  ;
  ```
    > Con ```IF NOT EXISTS``` evitamos crear duas bases de datos co mesmo nome.   
    >Con ```CHARACTER SET``` indicamos o CharSet que queremos usar, como UTF-8.
- #### ```CREATE DOMAIN```
