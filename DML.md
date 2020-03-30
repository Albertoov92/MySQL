# Apuntes del sublenguaje DML
## Índice
  - [Sentencias DML](#Sentencias-DML)
    - [INSERT](#INSERT)
    - [UPDATE](#UPDATE)
  ## Sentencias DML
  Na linguaxe SQL hai 3 instrucións que compoñen o DML (* Data Manipulation Language*). Son aquelas frases que nos permiten manipular a información que almacenamos nas bases de datos.

  Existen 3 instrucións que nos permitirán inserir datos nunha táboa **(INSERT)** , modificar eses datos **(UPDATE)** e borralos **(DELETE)**.

  ### INSERT
A instrución **INSERT** permite engadir datos a unha táboa
```sql
  INSERT INTO world
  [(name, continent, area)]
  VALUES
  ('SPAIN', 'EUROPE', 100),
  ('PORTUGAL','EUROPE', 10);
```
Como podemos observar na sentencia anterior engadimos dúas tuplas con os valores especificados en **VALUES**, como podemos observar podemos engadir máis de una tupla a vez sempre que sepáresmos as tuplas por coma.

    **NOTA**: Os  valores numéricos non van entre comillas.
### UPDATE
A instrución **UPDATE** permite modificar datos
