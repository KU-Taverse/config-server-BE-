FROM openjdk:17-jdk

ARG JAR_FILE=../../build/libs/*.jar


ARG GIT_ID
ARG GIT_PASS

COPY ${JAR_FILE} app.jar

ENV GIT_ID=${GIT_ID}
ENV GIT_PASS=${GIT_PASS}

ENTRYPOINT ["java", "-jar", "/app.jar"]