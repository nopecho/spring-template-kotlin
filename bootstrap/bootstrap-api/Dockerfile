FROM amazoncorretto:21-alpine
LABEL org.opencontainers.image.source=https://github.com/nopecho/spring-template-kotlin
LABEL authors=nopecho

ARG FROM_JAR=build/libs/bootstrap-api.jar

WORKDIR /app
COPY $FROM_JAR ./app.jar

EXPOSE $PORT
ENTRYPOINT [ "java", "-jar", "app.jar" ]