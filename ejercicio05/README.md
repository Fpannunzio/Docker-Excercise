HEALTHCHECK: la idea es que cuando se crea un dockerfile usando la sintaxis HEALTHCHECK, al incicializarse la imagen se realizara algun comando, como podria ser un curl a localhost en el puerto 80 en el caso de que se haya levantado un servidor nginx, esto se realizara x veces en un intervalo de n tiempo y si este no responde a todos estos intentos, el estado pasara a ser unhealthy. Si responde bien su estado sera normal. Esto puede ser util para determinar si se entro en un estado de deadlock o en un bucle infinito o no se ejecuto algun comando en particular pero si otros.

ONBUILD: Sirve para lanzar una instruccion que se ejecutara mas tarde, cuando la imagen sea usada como base para realizar un build distinto. El comando ejecutado se lanzara inmediatamente despues del FROM del nuevo dockerfile. Es importante destacar que esto no afectara a la build actual, sino a aquellas que sean construidas usando esta como base.

VOLUME: Sirve para definir un punto de montaje en un contenedor. Esto resulta util para enviar informacion o cualquier tipo de datos de un host a un container corriendo. Entre algunas de sus ventajas se encuentran:
    -Son mas faciles de backupear que los puntos de montaje de estilo bind. 
    -Sirven tanto para contenedores Linux como para contenedores Windows. 
    -Son mas faciles de compartir entre containers.