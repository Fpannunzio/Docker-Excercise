## Correr imagen exponiendo el puerto 80 en mi localhost 80
docker run -p 80:80 --name excercise1 -v ${PWD}/html:/usr/share/nginx/html:ro -d nginx