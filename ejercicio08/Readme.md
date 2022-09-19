## documentacion
`https://docs.docker.com/compose/compose-file/`

¿Cuántos contenedores se están ejecutando? (pueden verlo en el archivo docker-compose.yml y también ejecutando docker ps)

Se estan ejecutando dos contenedores, uno web y uno db. Estos estan definidos en la seccion de services.

¿Cuales son las imágenes en las que están basados los mencionados contenedores?

El container web esta basado en la imagen nicopaez/jobvacancy-ruby version 1.3.0
El container db esta basado en la imagen postgres version 14.4-alpine

¿Puedes leer el docker-compose.yml y describir lo que hace cada una de sus lineas?

La linea 1 declara la version del documento de docker compose subido
La linea 2 declara la seccion de contenedores que van a ser levantados
La linea 3 declara el inicio del container definido como web
La linea 4 declara la imagen a partir de la cual se levantara el container
Las linea 5 y 6 declara un link de red a otros contenedores, en este caso e contenedor db
Las linea 7 y 8 define que se expondra el puerto 3000 del contenedor en el puesto 3000 de mi maquina
Las lineas 9, 10, 11 y 12 definen la seccion de variables de entorno, entre ellas el puerto a exponer y la url de la base de datos a la que comunicarse, con sus credenciales y puerto
Las lineas 13 y 14 definen la dependencia del contenedor db, el cual debera estar levantado para levantar este contenedor
A partir de la linea 15 se define el contenedor db
En la linea 16 se define la imagen a partir de la cual se construira
En las lineas 17 y 18 se define la variable de entorno que representara la contraseña de la db

Dado que cada contenedor corre en forma aislada ¿Cómo es posible que esos contenedores se vean entre sí?

Docker compose levanta una red en la cual los contenedores pueden comunicarse, con las lineas 5 y 6 le definimos al container web que existe un container db con el cual puede comunicarse a traves de esa referncia