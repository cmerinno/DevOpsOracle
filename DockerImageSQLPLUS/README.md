
# Generación de imagen SQLPlus 12.2


## Construcción Imagen Oracle Linux SQLPLUS
docker build -t {imagen_sqlplus} .

## Ejecutar contenedor {contenedor_sqlplus} a partir de la imagen {imagen_sqlplus}

docker run -it --name {contenedor_sqlplus} -p 1521:1521 {imagen_sqlplus}

### Ejemplo ejecución de SQLPLUS a base de datos

/instantclient_11_2/sqlplus <user>/<password>@//<host>:<port>/<ssid>

/instantclient_12_2/sqlplus BDSAG/OPTI2018@//10.10.1.21:1521/ORCL