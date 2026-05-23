FROM maven:3.9.9-eclipse-temurin-23-alpine

WORKDIR /MeteoDatas-SpringApp

COPY MeteoDatas-SpringApp/ .

#COPY ../../.env-local ./src/main/resources/.env.properties

RUN mvn clean install -DskipTests

CMD ["mvn", "-Dspring-boot.run.fork=false" ,"spring-boot:run"]

EXPOSE 8080
