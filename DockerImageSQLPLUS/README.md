
# Generación de imagen SQLPlus 12.2


## Construcción Imagen Oracle Linux SQLPLUS
docker build -t {imagen_sqlplus} .

## Ejecutar contenedor {contenedor_sqlplus} a partir de la imagen {imagen_sqlplus}

docker run -it --name {contenedor_sqlplus} -p 1521:1521 {imagen_sqlplus}

