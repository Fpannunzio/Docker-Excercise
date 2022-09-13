Para conseguir la imagen

docker pull registry.access.redhat.com/redhat-openjdk-18/openjdk18-openshift:1.12-1.1661378017

## Para buildear la imagen

docker build -t passwordapiredshift .

## Para correr la imagen exponiendo el puerto 8080

docker run -d -p 8080:8080 passwordapiredshift


## Subir imagen a docker hub

docker tag passwordapiredshift fpannunziobalanz/exercise-06:v1
docker push fpannunziobalanz/exercise-4:v1