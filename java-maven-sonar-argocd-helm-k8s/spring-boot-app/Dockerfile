# You can change this base image to anything else
# But make sure to use the correct version of Java
FROM openjdk:11-jre-slim

# Simply the artifact path
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

# This copy artifact in app.jar inside the container
COPY ${artifact} app.jar

# This should not be changed as this execute once container starts
ENTRYPOINT ["java","-jar","app.jar"]
