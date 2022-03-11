FROM openjdk:8-jdk-alpine
#FROM adoptopenjdk/openjdk11:alpine-jre
ENV SERVER_PORT=8081
ENV DEBUG_PORT=8081
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} hello.jar
EXPOSE $SERVER_PORT
EXPOSE $DEBUG_PORT
ENTRYPOINT ["java","-jar","/hello.jar"]