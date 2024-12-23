FROM eclipse-temurin:17-jdk-alpine
WORKDIR /app
COPY build/libs/cache-aside.jar app.jar
ENV JAVA_OPTS="-XX:MaxRAMPercentage=75.0 -Djava.security.egd=file:/dev/./urandom"
ENTRYPOINT ["sh", "-c", "java $JAVA_OPTS -jar app.jar"]
