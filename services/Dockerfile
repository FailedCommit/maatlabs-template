FROM eclipse-temurin:17-jre

VOLUME /tmp
ARG JAR_FILE=build/libs/services-*.jar
COPY ${JAR_FILE} services.jar

EXPOSE 9090

ENTRYPOINT ["java", "-jar", "/services.jar"]
