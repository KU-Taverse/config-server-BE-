FROM openjdk:17-jdk

ARG JAR_FILE=../../build/libs/*.jar


ARG GIT_ID
ARG GIT_PASS
ARG MY_SECRET

COPY ${JAR_FILE} app.jar

ENV GIT_ID=${GIT_ID}
ENV GIT_PASS=${GIT_PASS}
ENV MY_SECRET=${MY_SECRET}

ENTRYPOINT ["java", "-jar", "/app.jar"]