# You can change this base image to anything else
# But make sure to use the correct version of Java
FROM openjdk:17-jdk-slim


JAVA_HOME = "/usr/lib/jvm/java-17-openjdk-amd64"
PATH = "/usr/lib/jvm/java-17-openjdk-amd64/bin:$PATH"


# Simply the artifact path
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

# This should not be changed
ENTRYPOINT ["java","-jar","app.jar"]

