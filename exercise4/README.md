## Para correr la aplicacion local
java -jar passwordapi.jar. Eso levanta una webapi en el puerto 8080 (ver captura de pantalla).

## Para buildear la imagen

docker build -t passwordapi .

## Para correr la imagen exponiendo el puerto 8080

docker run -d -p 8080:8080 passwordapi

## Subir imagen a docker hub

docker tag passwordapi fpannunziobalanz/exercise-4:v1
docker push fpannunziobalanz/exercise-4:v1