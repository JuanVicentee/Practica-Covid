1º creamos los ficheros ciudades y paises.
2º Extraemos datos de la api de de 4 meses.
3º Por cada registro de día generado por la api, se generan registros para todas las ciudades aplicando un multiplicador para que los datos sean diferentes.
4º Se formatea la fecha para que tenga el formato aaaa-mm-dd y se crean las columnas año, mes y dia.
5º Se guardan los datos en un carpeta llamada datos_parquet y se organizan en carpetas por pais y después por ciudad.
6º Por último se leen los ficheros parquet y se guardan en una base de datos, junto a los ficheros de ciudades y paises.

Después se han llevado los datos a Power BI desde la base de datos.
Se han creado 4 roles. Uno que vea todos los paises, otro que vea solo dos y otros dos que solo vean un pais.
Se ha añadido un parámetro a la tabla de datos covid para que se muestre los registros que tengan el parametro = 1, por si no se quiere mostrar alguno.
Y también se ha creado un parametro llamado CargarDatos en Power BI donde si está a 0 no se cargue la tabla y si se cambia a 1 se muestren los datos del covid. Esto se puede cambiar si vamos a "Inicio --> Transformar datos --> Editar parámetros" y desde ahí se puede cambiar el parámetro CargarDatos.
Y por último se han creado dos cuadros de mando.