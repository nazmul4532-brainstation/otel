FROM openjdk:17-jdk-slim
VOLUME /tmp
COPY target/demo-0.0.1-SNAPSHOT.jar app.jar
COPY opentelemetry-javaagent.jar opentelemetry-javaagent.jar
EXPOSE 8080
ENTRYPOINT ["java", "-javaagent:/opentelemetry-javaagent.jar", "-jar", "/app.jar"]
