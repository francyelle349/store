FROM openjdk:21-jdk-slim

WORKDIR /app

COPY gradlew .
COPY gradle ./gradle
COPY build.gradle .
COPY src ./src


RUN ./gradlew build
COPY build/libs/demo-0.0.1-SNAPSHOT.jar app.jar
ENV SPRING_DATA_MONGODB_URI=mongodb://root:root@mongodb:27017/database

EXPOSE 8080

CMD ["java", "-jar", "app.jar"]