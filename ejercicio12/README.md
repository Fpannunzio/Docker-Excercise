## Para ejecutar el deployment

Primero construir los configmap y despues el archivo secret. Importante, el archivo secret tiene que ser kind Secret y tener su contenido en base 64

Correr los 3 archivos con apply

Una vez corrido ejecutar el deployment principal

Por ultimo, ejecutar el nodeport