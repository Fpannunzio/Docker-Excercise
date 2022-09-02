
## Buildear imagen

docker build -t webserver .

## Correr imagen exponiendo el puerto 80 en mi localhost 8080
docker run -it --rm -d -p 8080:80 --name web webserver