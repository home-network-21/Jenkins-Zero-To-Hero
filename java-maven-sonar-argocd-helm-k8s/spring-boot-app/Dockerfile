# You can change this base image to anything else
# But make sure to use the correct version of Java
FROM adoptopenjdk/openjdk11:alpine-jre

# Simply the artifact path
ARG artifact=target/spring-boot-web.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

# This should not be changed
ENTRYPOINT ["java","-jar","app.jar"]

# summary of dockerfile
# It uses a base image that includes OpenJDK 11 on Alpine Linux (adoptopenjdk/openjdk11:alpine-jre).
# It defines a build-time argument (artifact) which specifies the path of the JAR file (default value is target/spring-boot-web.jar).
# It sets the working directory inside the container to /opt/app.
# It copies the JAR file (specified by the artifact argument) into the /opt/app directory inside the container and renames it as app.jar.
# It sets the ENTRYPOINT to run the application with the command java -jar app.jar.
# java -jar app.jar , this command runs the java application, so the moment container is created from this image, java application starts running.
