FROM maven:3.9.9-eclipse-temurin-23-alpine

WORKDIR /MeteoDatas-SpringApp

COPY ../../spring_app .

COPY ../../.env-local ./src/main/resources/.env.properties

RUN mvn clean install -DskipTests

CMD ["mvn", "spring-boot:run"]

EXPOSE 8080
