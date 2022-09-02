docker history --no-trunc <Image ID>

nicopaez/passwordapi-java     java8-fabric cuenta con

IMAGE          CREATED       CREATED BY                                      SIZE      COMMENT
c479d0765f34   3 years ago   /bin/sh -c #(nop)  USER 405                     0B        
<missing>      3 years ago   /bin/sh -c #(nop)  EXPOSE 8080                  0B        
<missing>      3 years ago   /bin/sh -c #(nop) COPY file:a6e9b80e7469da50…   25.4MB    
<missing>      3 years ago   /bin/sh -c #(nop)  ARG JAR_FILE                 0B        
<missing>      4 years ago   /bin/sh -c #(nop)  CMD ["/deployments/run-ja…   0B        
<missing>      4 years ago   /bin/sh -c chmod 755 /deployments/run-java.sh   18.6kB    
<missing>      4 years ago   /bin/sh -c #(nop) COPY file:9664759840f7d23e…   18.6kB    
<missing>      4 years ago   /bin/sh -c #(nop)  EXPOSE 8778 9779             0B        
<missing>      4 years ago   /bin/sh -c #(nop) ADD file:19cf38fb1c34ab0eb…   919B      
<missing>      4 years ago   /bin/sh -c mkdir -p /opt/agent-bond  && curl…   869kB     
<missing>      4 years ago   /bin/sh -c #(nop) ADD file:0e4d47c8ceb53292e…   4.04kB    
<missing>      4 years ago   /bin/sh -c apk add --update     curl     ope…   99.1MB    
<missing>      4 years ago   /bin/sh -c #(nop)  ENV JAVA_APP_DIR=/deploym…   0B        
<missing>      4 years ago   /bin/sh -c mkdir -p /deployments                0B        
<missing>      4 years ago   /bin/sh -c #(nop)  USER root                    0B        
<missing>      4 years ago   /bin/sh -c #(nop)  CMD ["/bin/sh"]              0B        
<missing>      4 years ago   /bin/sh -c #(nop) ADD file:25f61d70254b9807a…   4.41MB    

java8-alpine

IMAGE          CREATED       CREATED BY                                      SIZE      COMMENT
22e1f6ea60af   3 years ago   /bin/sh -c #(nop)  CMD ["/usr/bin/java" "-ja…   0B        
<missing>      3 years ago   /bin/sh -c #(nop) COPY file:a6e9b80e7469da50…   25.4MB    
<missing>      4 years ago   /bin/sh -c set -x  && apk add --no-cache   o…   78.6MB    
<missing>      4 years ago   /bin/sh -c #(nop)  ENV JAVA_ALPINE_VERSION=8…   0B        
<missing>      4 years ago   /bin/sh -c #(nop)  ENV JAVA_VERSION=8u171       0B        
<missing>      4 years ago   /bin/sh -c #(nop)  ENV PATH=/usr/local/sbin:…   0B        
<missing>      4 years ago   /bin/sh -c #(nop)  ENV JAVA_HOME=/usr/lib/jv…   0B        
<missing>      4 years ago   /bin/sh -c {   echo '#!/bin/sh';   echo 'set…   87B       
<missing>      4 years ago   /bin/sh -c #(nop)  ENV LANG=C.UTF-8             0B        
<missing>      4 years ago   /bin/sh -c #(nop)  CMD ["/bin/sh"]              0B        
<missing>      4 years ago   /bin/sh -c #(nop) ADD file:25f61d70254b9807a…   4.41MB 


En comun:

<missing>      3 years ago   /bin/sh -c #(nop) COPY file:a6e9b80e7469da50…   25.4MB 
<missing>      4 years ago   /bin/sh -c #(nop)  CMD ["/bin/sh"]              0B        
<missing>      4 years ago   /bin/sh -c #(nop) ADD file:25f61d70254b9807a…   4.41MB 