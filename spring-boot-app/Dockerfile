# You can change this base image to anything else
# But make sure to use the correct version of Java
FROM openjdk:17-jdk-slim


ENV JAVA_HOME=/usr/lib/jvm/java-17-openjdk-amd64
ENV PATH="$JAVA_HOME/bin:$PATH"



WORKDIR /opt/app

COPY target/spring-boot-web.jar app.jar

# This should not be changed
ENTRYPOINT ["java","-jar","app.jar"]







