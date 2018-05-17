
# Generación de imagen SQLPlus 12.2


## Construcción Imagen Oracle Linux SQLPLUS
docker build -t {imagen_sqlplus} .

## Ejecutar contenedor oracle12cSQLPlus a partir de la imagen {imagen_sqlplus}

docker run -it --name oracle12cSQLPlus -p 1521:1521 {imagen_sqlplus}

