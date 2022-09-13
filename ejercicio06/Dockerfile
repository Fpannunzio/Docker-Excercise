FROM registry.access.redhat.com/redhat-openjdk-18/openjdk18-openshift:1.12-1.1661378017
WORKDIR /app
COPY passwordapi.jar /app
EXPOSE 8080:8080
CMD java $JAVA_OPTIONS -jar passwordapi.jar


