# Paso 1 levantar el container

docker run --name excercise10 -e TELEGRAM_TOKEN='A COMPLETAR' nicopaez/telegrambot:0.0.7

# Paso 2 ejecutar deployment

kubectl apply -f deployment.yml