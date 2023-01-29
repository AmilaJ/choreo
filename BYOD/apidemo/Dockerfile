FROM --platform=linux/amd64 eclipse-temurin:18-jdk-alpine



ENV UID=10001
ENV GID=15011



USER 10001:15011

ARG JAR_FILE=build/libs/apidemo-0.0.1-SNAPSHOT.jar
COPY ${JAR_FILE} app.jar
ENTRYPOINT ["java","-jar","/app.jar"]
#HEALTHCHECK CMD curl --fail http://localhost:3000 || exit 1

EXPOSE 8080
