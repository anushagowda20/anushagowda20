FROM openjdk:15.0.2-slim

ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} app.jar

EXPOSE 8080

ENTRYPOINT ["java", \
            "-jar", \
            "-Dfile.encoding=UTF-8", \
            "-Duser.timezone=GMT", \
            "-Djava.security.egd=file:/dev/./urandom -jar", \
            "app.jar"]
